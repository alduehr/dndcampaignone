# Onboarding into the DungeonMaster app

This repository is onboardable into [DungeonMaster](https://github.com/alduehr/dungeonmaster) — a
cloud-deployed AI Dungeon Master server with a React Native player app —
via that project's `onboard-campaign` pipeline. This file documents exactly
what was prepared here, why, and the two things still needed from the
DungeonMaster deployment's own operator before a session can actually run.
Written 2026-07-12; updated 2026-08-09 when the location-reference library
moved to `locations/vael/orrun/` and became separately onboardable (see
"Locations — a second, separate onboarding unit" below). See
`ai_solo_campaign/00_control/PROGRESS_LOG.md` for the production-history
entry.

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
| `maps/manifest.json` under the content root, valid JSON | [`locations/vael/orrun/maps/manifest.json`](locations/vael/orrun/maps/manifest.json) — 64 entries, no storage location authored in-repo (see the Maps section below). Moved out of `ai_solo_campaign/maps/` in the 2026-08-09 location-key restructuring; see below |
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

## Locations — a second, separate onboarding unit

As of 2026-08-09, `locations/vael/orrun/` — the spoiler-free world-reference
library previously mirrored at `Locations/Orrun/` — restructured onto a
**canonical-key scheme** (`<world>/<continent>/<kind>/<slug>`, e.g.
`vael/orrun/regions/ashgarden-vale`) so it can be onboarded into
DungeonMaster as an independent **location** unit, separate from this
campaign, and then mounted into a campaign's namespace at runtime.

[`locations/vael/orrun/dm.location.json`](locations/vael/orrun/dm.location.json)
is the location-manifest contract that folder declares for itself
(`locationId`, `displayName`, `world`, `continent`, `contentRoot: "."`,
relative to the manifest's own directory — same convention as
`dm.campaign.json`'s `contentRoot`). `dm.campaign.json` at this repo's root
now also carries a top-level `locations` array, sibling to `contentRoot`,
mounting that location at `locations/vael/orrun`:

```json
"locations": [
  { "locationId": "vael-orrun", "mountPath": "locations/vael/orrun" }
]
```

**This shape is inferred, not copied from a spec** — `dm.location.json` and
the `onboard-location` pipeline don't exist in DungeonMaster yet; they're
defined by `PHASE10.6_PLAN.md` Step 2, which `shared-contract-guardian` is
building to match. Verify the exact field names/shape against that plan (or
the merged app-side schema) before relying on this file for a real
onboarding run; the two sides are meant to land together. `world`/`continent`
are documented as descriptive-only — path/mount resolution comes from
`mountPath` on the campaign side, not from the location's own folder name or
id, so the two stay independent on purpose.

## Maps — prepared, no bucket wiring needed from this repo

`locations/vael/orrun/maps/manifest.json` is fully populated: 64 entries (18
region maps, 1 campaign-area cluster overview, 4 city maps, 40 settlement
maps, 1 full-continent overview), generated from this repo's own authored
map-packet inventory (`04_world_atlas/region_map_packets/`,
`06_settlements/city_map_packets/`, `06_settlements/settlement_map_packets/`,
`04_world_atlas/WORLD_MAP_PROMPTS.md`), one-to-one, with no duplicate ids.
Each entry's `region` field is now a canonical location key (e.g.
`vael/orrun/regions/ashgarden-vale`) rather than a bare slug — see
"Locations" above. As of DungeonMaster's `038a33c` ("Derive maps S3
bucket/key from deployment config, not manifest"), a `MapEntry` carries no
storage location at all — no `s3.bucket`, no `s3.key`. Each entry is pure
campaign-authored metadata: `id` / `file` / `region` / `caption` / `scale` /
`visibility`. The bucket always comes from the deployment's own
`MAPS_BUCKET_NAME`, and the object key is always
`mapObjectKey(campaignId, file)` → `<campaignId>/maps/<file>` — computed at
upload and read time, never authored here. Nothing in this repo needs
editing to point at a real bucket; there is no placeholder left to replace.

**This manifest moved out of `ai_solo_campaign/maps/` on 2026-08-09.** The
two copies were always byte-identical (one authoritative, one a mirror), so
keeping a single copy under `locations/vael/orrun/maps/` — maps are
geography, not campaign-runtime material — removed the duplication.
`dm.campaign.json`'s `contentRoot` is unaffected and still points at
`ai_solo_campaign` for the campaign's own content; maps are reached through
the `locations` mount instead.

**9 of 64 entries currently have a matching local asset** under
`locations/vael/orrun/maps/assets/` (see that folder for the current list).
`upload-maps.ts` skips (doesn't fail) any entry whose asset file isn't
present yet, so partial map coverage is fine — sessions run without maps in
the meantime, same as before.

To actually get maps into a deployment once one exists:

1. **Place generated PNGs** under `locations/vael/orrun/maps/assets/<file>`,
   matching each entry's `file` field (e.g. `settlement-hollowmere.png`) —
   `file` must be a bare filename (no `/`, no path), enforced identically on
   both the upload and `get_map` read sides.
2. Run DungeonMaster's `upload-maps.ts` with `CONTENT_ROOT` pointed at a
   local checkout of `locations/vael/orrun/`, `MAPS_BUCKET_NAME` set to that
   deployment's real bucket, and `CAMPAIGN_ID=the-long-remembering` (now
   required — cross-checked against this repo's own `dm.campaign.json`
   `campaignId`, so a typo'd env var fails loudly instead of uploading to a
   key nothing will ever read). Maps are a separate upload pipeline from
   campaign-content onboarding (different concern entirely, keyed by
   campaign under one shared bucket), so this step happens independently of
   `onboard-campaign` and doesn't require a tagged release — any local
   checkout works, and it's idempotent (re-run any time you add more maps).
   **This CONTENT_ROOT value will need to be revisited** once
   `onboard-location` exists and maps are pulled through the location unit
   rather than a direct local checkout — see the "Locations" section above.

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
changed to prepare the original 2026-07-12 onboarding — every file under
`ai_solo_campaign/` was exactly as authored. The two new top-level files
(`dm.campaign.json`, this file) and the one new subtree
(`ai_solo_campaign/skills/`, 6 files) were additive.

The 2026-08-09 location-key restructuring did move `ai_solo_campaign/maps/`
out entirely (to `locations/vael/orrun/maps/`, see "Maps" above) and added a
`locations` key to `dm.campaign.json` — both changes to the onboarding
surface, not to campaign content or doctrine. `contentRoot` is unchanged;
`ai_solo_campaign/`'s own regions/settlements/NPCs/quests/mysteries content
is unchanged in substance (only how it cites the location library changed,
from relative file paths to canonical keys).
