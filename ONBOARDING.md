# Onboarding into the DungeonMaster app

This repository is onboardable into [DungeonMaster](https://github.com/alduehr/dungeonmaster) — a
cloud-deployed AI Dungeon Master server with a React Native player app —
via that project's `onboard-campaign` pipeline. This file documents exactly
what was prepared here, why, and the two things still needed from the
DungeonMaster deployment's own operator before a session can actually run.
Written 2026-07-12; see `ai_solo_campaign/00_control/PROGRESS_LOG.md` for the
production-history entry.

The DungeonMaster app is a **different system** from Claude Code — it is a
standing server that runs this campaign as a stateful agentic loop over the
Claude API for a phone app, independent of any Claude Code session. This
repository was in fact one of the two reference points the DungeonMaster
project's own onboarding contract (`PROTOCOL.md`, "Campaign content
onboarding contract") was designed against.

## What onboarding needs, and what's here

The DungeonMaster onboarding pipeline (`content-pull` → `onboard-campaign`)
requires an onboardable campaign repo to declare a `dm.campaign.json`
manifest at its root and pass a verification contract. Everything that
contract checks is now in place:

| Contract requirement | What's here |
|---|---|
| `dm.campaign.json` manifest at repo root | [`dm.campaign.json`](dm.campaign.json) — `campaignId: "the-long-remembering"`, `contentRoot: "ai_solo_campaign"` |
| A resolvable visibility strategy | `path-convention`, with an exact 21-file `playerSafeGlobs` allowlist — see below |
| `maps/manifest.json` under the content root, valid JSON | [`ai_solo_campaign/maps/manifest.json`](ai_solo_campaign/maps/manifest.json) — 63 entries (see the Maps section below for what's still needed) |
| Seed files (optional) parse correctly | None declared — deliberate, see below |
| No path escapes the content root | N/A — nothing here does |
| Every mandatory skill-consultation path resolves post-merge | `ai_solo_campaign/skills/` overlay — 6 of the 8 mandatory paths overridden, 2 fall through to the shared floor |

## Decision 1 — Visibility: `path-convention`, not `front-matter`

This campaign's own metadata standard (`CONTENT_STANDARDS.md`) tags every
file's secrecy level as `secrecy: player-safe | dm-only | mixed` in front
matter. The DungeonMaster runtime's visibility model is **binary**
(`player-safe` | `dm-only`, under a differently-named `visibility:` key) and
fails closed to `dm-only` for anything untagged or unrecognized.

Rather than hand-rewrite front matter across 574 files to add a second key
with a narrower vocabulary, `dm.campaign.json` declares the `path-convention`
strategy — exactly what `PROTOCOL.md`'s own onboarding-contract section
recommends for a repo shaped like this one. Onboarding derives and injects
`visibility:` automatically at pull time; nothing in this repo's own front
matter needed to change.

The allowlist is the **exact** 21 files currently tagged `secrecy:
player-safe` in this repo (verified 1:1 against a live simulation of the
onboarding pipeline's own glob-matching code — 21 globs, 21 matches, zero
misses, zero false positives). Every `secrecy: dm-only` file, every `secrecy:
mixed` file (420 of them — files that interleave player-facing and DM-only
content in the same document), and every untagged control/tracking file
(mostly `00_control/` and `02_runtime_state/`, which were never meant to be
player-facing) fails closed to `dm-only`. This is the **correct** mapping,
not just the safe one: DungeonMaster's system prompt has a non-negotiable
rule that "content marked dm-only must never be quoted verbatim to the
player," and a `mixed` file's raw text literally contains hidden truth
inline — quoting it verbatim would leak a spoiler regardless of what the
binary tag says. `dm-only` files remain fully readable by the DM agent via
`read_file`; the tag governs narration discipline, not access.

**If a file's secrecy is later changed** in this repo, `dm.campaign.json`'s
glob list needs a matching edit before the next onboarding pull — it is not
automatically kept in sync.

## Decision 2 — No character/state seed

`dm.campaign.json` declares no `seed` block. This is deliberate, not an
oversight: this campaign's own design has character creation happen
*conversationally*, in the first session, not from a pre-built sheet — see
`ai_solo_campaign/16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md` Step 3.
The DungeonMaster server's own `getOrCreateCharacter` already falls back to
an empty default character shell when no seed exists, which the DM agent
then fills in via `update_character` during the session-1 conversation — the
app's actual behavior matches this campaign's design exactly with no seed
file needed.

## Decision 3 — The `skills/` overlay

DungeonMaster's frozen system prompt mandates the agent read 8 specific
`skills/`-rooted files before certain actions (combat, checks, travel,
downtime, session start/end, canon-and-gaps, rules-reference). This repo's
own extensive `01_runner_protocol/`, `16_ai_session_packs/`, and
`00_control/` doctrine is **not** automatically consulted at those paths —
per `PROTOCOL.md`, a campaign that wants its own procedures followed has to
provide them at the `skills/` overlay paths, which win on collision over the
shared generic floor.

`ai_solo_campaign/skills/` now overrides **6 of the 8** mandatory paths:

- `procedures/session-start.md` — adds this campaign's own first-session
  character-creation flow and its index-first retrieval discipline
  (`00_control/RETRIEVAL_GUIDE.md`)
- `procedures/session-end.md` — the most load-bearing override: translates
  this repo's own 16-file `SESSION_END_UPDATE_CHECKLIST.md` (written for a
  human hand-editing markdown between sessions) onto the app's actual,
  durable state mechanism (`set_state`/`log_event`/`record_canon`/
  `update_character`) — the content tree is read-only at runtime, so nothing
  in that checklist can be literally "updated" as a file
- `canon-and-gaps/SKILL.md` — layers this campaign's finer authored-file
  precedence order (`CANON_AUTHORITY.md`) and its reveal-gating discipline
  (`REVELATION_MAP.md`, `SECRET_REVEAL_PROTOCOL.md` — mysteries are earned
  through play, not narrated because the DM read the file) on top of the
  shared 3-tier authority model
- `combat/SKILL.md` — keeps the shared file's exact mechanical backbone
  (initiative, turn structure, adjudication, ending combat) and adds this
  campaign's solo-safety spine (telegraph before lethal, active morale,
  guaranteed retreat, wounded-PC caution) — every encounter in this
  repo is already solo-tuned; the override makes the DM agent honor that
- `procedures/travel.md` / `procedures/downtime.md` — point at this
  campaign's own routes, hazard DCs, random tables, and faction-turn
  consequences instead of inventing them generically

**Not overridden:** `procedures/checks.md` (this campaign's own DC ladder —
10/15/20/25/30 — is verbatim identical to the shared SRD file's; nothing to
add) and `rules-reference/SKILL.md` (pure SRD mechanics; this campaign
deliberately doesn't invent replacement rules — see `RULESET_ASSUMPTIONS.md`).
Both resolve from the shared floor at pull time, same as any campaign that
ships no overlay for them.

## Maps — prepared, with one step still needed from you

`ai_solo_campaign/maps/manifest.json` is fully populated: 63 entries (18
region maps, 4 city maps, 40 settlement maps, 1 full-continent overview),
generated from this repo's own authored map-packet inventory
(`04_world_atlas/region_map_packets/`, `06_settlements/city_map_packets/`,
`06_settlements/settlement_map_packets/`), one-to-one, with no duplicate ids
or region keys.

**What it can't know yet:** the actual S3 bucket a real DungeonMaster
deployment's maps live in. Every entry's `s3.bucket` is currently the literal
placeholder `"REPLACE_WITH_MAPS_BUCKET_NAME"` — `get_map` will refuse any
lookup against it until it's corrected (a clean, loud failure, not a silent
one; sessions run fine without maps in the meantime). Two things to do once
you have a deployment and the map images you generated separately:

1. **Replace the placeholder** in every entry with that deployment's actual
   `MAPS_BUCKET_NAME` (a single find-and-replace across the file).
2. **Place your generated PNGs** under `ai_solo_campaign/maps/assets/<file>`,
   matching each entry's `file` field (e.g. `settlement-hollowmere.png`),
   then run DungeonMaster's `upload-maps.ts` pointed at this content root —
   maps are a separate upload pipeline from campaign-content onboarding
   (different S3 bucket entirely), so this step happens independently of
   `onboard-campaign`. `upload-maps.ts` skips (doesn't fail) any entry whose
   asset file isn't present yet, so partial map coverage is fine.

If your generated files use different names than this manifest's `file`
convention (`<kind>-<slug>.png`), either rename the files or edit the
matching `file` field — either is a small, low-risk edit.

## Running the onboarding pipeline (operator/CI side, not from this repo)

This repo doesn't run its own onboarding — it's pulled by DungeonMaster's
own tooling. From that repo:

1. Cut a tagged release of this repo (e.g. `v1.0.0`) — onboarding pulls a
   specific tag, not a moving branch.
2. Run `npm run onboard-campaign` with `CAMPAIGN_ID=the-long-remembering`,
   `CONTENT_SOURCE_OWNER`/`CONTENT_SOURCE_REPO` pointed at this repo,
   `CONTENT_SOURCE_TAG` set to that release tag, and the deployment's
   `CONTENT_BUCKET_NAME`/`DYNAMODB_TABLE_NAME` set — see that project's
   `scripts/onboard-campaign.ts` header comment for the full env-var list.
3. Once onboarded, the campaign is selectable via `GET /campaigns` /
   `POST /session/start`'s `campaignId` field.

## What was intentionally left alone

Nothing about this campaign's own content, structure, canon, or doctrine was
changed to prepare this onboarding — every file above the repo root
(`ai_solo_campaign/`) is exactly as authored. The two new top-level files
(`dm.campaign.json`, this file) and the one new subtree
(`ai_solo_campaign/skills/`, 6 files) are additive. `ai_solo_campaign/
maps/manifest.json` is new (the folder didn't exist before) but was required
by the onboarding contract regardless of which app pulls this content.
