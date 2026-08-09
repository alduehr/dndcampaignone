# PROGRESS_LOG.md

## Purpose

Chronological record of all meaningful production passes. This is the project history.

---

## 2026-08-08 — locations/vael/orrun Split: Safety Audit + Settlement Public Overview Cleanup (Pass 5)

### Stage
Post-Stage-16 repo-structure pass (user-directed). User asked for a safety audit of Passes 1-4 ("are all the changes safe... make sure nothing important was removed... make sure the remaining information is all campaign specific") before treating the duplication-cleanup task as closed.

### Summary
Full audit of every diff from Passes 1-4 (~79 files, ~90 removed-content hunks across regions, settlements, wilderness, and dungeons/ruins) by cross-checking each removed passage against its `locations/vael/orrun` counterpart. Result: every substantive fact that was removed from `ai_solo_campaign` is confirmed present in `locations/vael/orrun`, generally near-verbatim. One minor loose end found and fixed: `THE_PEAT_CHAPEL.md`'s Entrance trim dropped the specific detail that **Old Sashe** (a named NPC, already the guide at the Barrow of Nine Doors) can also point the way here — Orrun's generic "any local can point out the line" covered the functional fact but not the NPC attribution; restored as a trailing campaign-specific note.

The audit's second half — "is the remaining information all campaign specific" — surfaced a real, previously-unaudited duplication class: the `## Public Overview` section in all 16 standalone settlement files (everything in `06_settlements/` except `CARADRIL.md`, which got this treatment in Pass 2) still substantially restated Orrun's founding/economy/population/governance prose, near-verbatim in several cases (e.g. Kettle Bridge's "the best place in the Reach to hear news and the worst to keep a secret" / Orrun's "the liveliest place in the Reach and the worst place in it to keep a secret"). Pass 2's log only checked First Impression and Laws and Customs for this pattern; Public Overview was missed for the 16 non-Caradril files. Fixed all 16: trimmed to a pointer at the matching `locations/vael/orrun/settlements/*.md` section, preserving only what Orrun genuinely lacks — named individual leadership (Orrun's stated policy is to name no current officeholders), named-faction plot hooks (Concord Remnant's interest in Candlewick's archive-stone, Coldhearth/Greywater Holm sheltering or drifting toward the Gravecallers), and plot-escalation facts tied to DM-Only Truth (Hollowmere's "Wren has come back wrong," Saltmargin's tripled rite-salt demand, Ashwalk Rest's crisis-level traffic).

Also confirmed by design, not fixed: `Named Sites`/`Zone List`, `Hazards`, and `Creatures/Adversaries` sections in wilderness (`05_regions/wilderness/*_SITES.md`) and dungeon (`10_dungeons_and_ruins/*.md`) files retain real overlap with their Orrun counterparts beyond pure atmosphere. This is intentional per `DND_MECHANICS_REQUIREMENTS.md` and `WORLDBUILDING_STANDARDS.md`'s Wilderness/Dungeon Standards, which require hazard DCs, room/zone lists, and encounter stat references to live in the campaign file for mechanical self-containment, and because clue/secret content is interwoven with the physical description sentence-by-sentence in ways that can't be surgically split without risking deletion of campaign-unique material (documented rationale in the Pass 3/4 log entries above). Orrun independently maintains its own spoiler-free version of the same generic content for pure "what does a traveler see" queries — this is accepted, bounded overlap, not missed cleanup.

### Files Changed
- `ai_solo_campaign/10_dungeons_and_ruins/THE_PEAT_CHAPEL.md` — restored the Old Sashe guide detail
- `ai_solo_campaign/06_settlements/*.md` (16: Candlewick, Cobble Strand, Coldhearth, Greywater Holm, Harrowgast, Hartfell, Hollowmere, Kettle Bridge, Orchardmere, Reedford, Saint Veddow's Rest, Saltmargin, The Ashwalk Rest, Tilbrook, Tollstone Cross, Wrackmouth) — Public Overview trimmed to pointers
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md` — "Entering a settlement" bullet now covers Public Overview, not just First Impression/Laws and Customs

### Canon Established
None — no world facts changed, only where existing facts are stored, plus one restored NPC-attribution detail.

### Indexes Updated
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md`

### Gaps Identified
None outstanding. The bounded, by-design overlap in wilderness/dungeon Named Sites/Hazards/Encounters sections (see Summary) is not a gap — it's a documented mechanical-completeness requirement, not missed cleanup.

### Next Recommended Pass
The duplication-cleanup task (Passes 1-5) is now verified complete and safe. Resume normal content production; if new region/settlement/wilderness/dungeon content is added, follow the same split (mechanics/secrets/NPCs in `ai_solo_campaign`, spoiler-free physical/sensory description in `locations/vael/orrun`, cross-pointer both ways) from the start rather than needing a later cleanup pass.

---

## 2026-08-08 — locations/vael/orrun Split: Maps Mirror + Region Duplication Cleanup (Pass 1 of 4)

### Stage
Post-Stage-16 repo-structure pass (user-directed). Follow-up to the 2026-08-01/02 `/Orrun` extraction passes.

### Summary
Three related structural changes, all user-directed: (1) moved `/Orrun` to `locations/vael/orrun` and fixed all cross-references; (2) copied `ai_solo_campaign/maps/` (manifest + 9 image assets) into `locations/vael/orrun/maps/` as a read-only mirror, since `ai_solo_campaign/maps/` stays authoritative for the DungeonMaster app onboarding contract (`dm.campaign.json`'s `contentRoot`); (3) began eliminating content duplication between `ai_solo_campaign` and `locations/vael/orrun` — the user does not want the same geography written twice. Pass 1 covers all 16 region files in `05_regions/`: their `## Geography` and `## Travel Routes` sections (pure physical/climate/culture/route description, already fully — and often more richly — covered in `locations/vael/orrun/regions/`) were replaced with short pointers to the matching Orrun file. Campaign-specific mechanical content inside those sections (DCs, named-NPC tolls, quest-tied access gates, coordinate/cartography-authority pointers to `region_map_packets/`) was preserved, not deleted. Nothing else in the region files (DM-Only Truth, Factions Present, Regional Secrets, Quest Hooks, Level Range And Solo Danger, Encounter And Hazard Mechanics, Regional Clocks, etc.) was touched — those are campaign-specific and not duplicated anywhere in Orrun by design (Orrun strips all secret/clue/hook/NPC material).

Settlements (18 files), wilderness sites (7 files), and dungeons/ruins (41 files) are the same cleanup, scoped by the user, but not yet done — see TODO.md.

### Files Changed
- `locations/vael/orrun/` — moved from `/Orrun` (58 files, git-tracked renames)
- `locations/vael/orrun/maps/manifest.json` + `locations/vael/orrun/maps/assets/*.png` (9 files) — new, mirrored from `ai_solo_campaign/maps/`
- `vael/orrun/README.md` — added "Maps" section documenting the mirror relationship and update order
- `vael/orrun/GAZETTEER_INDEX.md` — added Maps section
- `ai_solo_campaign/00_control/NAMING_REGISTRY.md` — path references updated (`/Orrun` → `locations/vael/orrun`)
- `ai_solo_campaign/05_regions/*.md` (all 16) — Geography + Travel Routes sections trimmed to pointers
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md` — "Entering a region" and "Entering a far-continent region" sections now direct the AI DM to load the matching `locations/vael/orrun/regions/` file for physical geography/climate/culture/travel-times, alongside the campaign region file for everything else

### Canon Established
None — no world facts changed, only where existing facts are stored.

### Indexes Updated
- `vael/orrun/GAZETTEER_INDEX.md`
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md`

### Gaps Identified
- Settlements, wilderness sites, and dungeons/ruins still duplicate geography with `locations/vael/orrun` — scoped for follow-up passes (see TODO.md). These are riskier than regions: clue/secret/hook/NPC content is interwoven sentence-by-sentence with physical/hazard description in the source files, not cleanly sectioned, so the cut has to be judged per file rather than pattern-replaced.

### Next Recommended Pass
Settlements cleanup (18 files, `06_settlements/*.md` vs `locations/vael/orrun/settlements/*.md` — note the Orrun side groups multiple settlements per region file, so mapping is many-to-one, not 1:1 like regions).

---

## 2026-08-08 — locations/vael/orrun Split: Settlement Duplication Cleanup (Pass 2 of 4)

### Stage
Post-Stage-16 repo-structure pass (user-directed). Continuation of the same-day Pass 1 (regions).

### Summary
Trimmed duplication from all 17 standalone settlement files (`06_settlements/*.md`, excluding `_PLACEHOLDER.md`) plus Caradril's main file and all 8 district files (`caradril_districts/*.md`) — 26 files total. Confirmed the same pattern held throughout: `## First Impression` (or, for the dungeon-style Sunken Wards sub-district, `## What The Player Notices First`) is near-verbatim duplicated by the matching `locations/vael/orrun/settlements/*.md` entry, and `## Laws and Customs` is substantially the same baseline. Replaced both with short pointers to the Orrun file/section, keeping any campaign-specific sentence that isn't in Orrun (a named DC, a plot-relevant detail, a faction-tied enforcement note) as a trailing "Campaign-specific:" line rather than deleting it. For Caradril's top-level file specifically, also trimmed `Public Overview`, `Scale and Layout`, `Government and Law Structure`, and `Shops and Services` — Orrun's `CARADRIL.md` covers all of these in comparable or greater depth, since it's a single large city file rather than a grouped regional gazetteer. Everything else in every file (DM-Only Truth, named NPCs/leadership, Factions Present, Current Tensions, Secrets, Quest Hooks, Possible Scenes, Law And Threat Mechanics, Consequences If Ignored) was left untouched — none of it exists in Orrun by design.

Mapping note: Orrun groups multiple settlements per region file (`SUNDERING_REACH_SETTLEMENTS.md` covers 8, `ASHGARDEN_VALE_SETTLEMENTS.md` covers 3, `TOLLWOOD_SETTLEMENTS.md` covers 3, `PALE_COAST_SETTLEMENTS.md` covers 2, `CARADRIL.md` covers Caradril + all 8 districts in one file), so this pass's pointers target a named section inside the group file, not a 1:1 file.

### Files Changed
- `ai_solo_campaign/06_settlements/*.md` (17 standalone settlements + `CARADRIL.md`)
- `ai_solo_campaign/06_settlements/caradril_districts/*.md` (all 8)
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md` — "Entering a settlement (any)" now directs the AI DM to the matching Orrun file/section for sensory description and general customs, alongside the campaign settlement file for everything else

### Canon Established
None — no world facts changed, only where existing facts are stored.

### Indexes Updated
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md`

### Gaps Identified
- Wilderness sites (7 files) and dungeons/ruins (41 files) remain — both riskier than settlements since clue/secret/hook/NPC content is interwoven with hazard/terrain description sentence-by-sentence rather than living in a cleanly separable section. See TODO.md Pass 3/4.

### Next Recommended Pass
Wilderness sites cleanup (7 files, `05_regions/wilderness/*.md` vs `locations/vael/orrun/wilderness/*.md`) — requires per-site, per-sentence judgment rather than a repeatable section-level pattern.

---

## 2026-08-08 — locations/vael/orrun Split: Wilderness Duplication Cleanup (Pass 3 of 4)

### Stage
Post-Stage-16 repo-structure pass (user-directed). Continuation of the same-day Passes 1–2 (regions, settlements).

### Summary
Trimmed all 7 `05_regions/wilderness/*_SITES.md` files — a lighter touch than Passes 1–2, deliberately. Confirmed by direct comparison that only `## What The Player Notices First` (pure atmospheric description, no mechanics, no secrets) is reliably near-duplicated by the matching `locations/vael/orrun/wilderness/*.md` file's `## What A Traveler Notices First` section; replaced it with a pointer, keeping any sentence that's genuinely campaign-unique (a plot-relevant detail like "the water is unnaturally calm, as if it is listening"). Everything else — Named Sites, Hazards (with DCs), Creatures/Adversaries (with stat references), NPCs Present, Secrets, Clues, Hooks, Treasure, Level Range And Solo Danger, Consequences If Ignored — was deliberately left untouched, even where a hazard's DC or a creature's stat-flavor happens to also appear in the Orrun file. Two reasons: (1) `DND_MECHANICS_REQUIREMENTS.md` and `WORLDBUILDING_STANDARDS.md`'s Wilderness Location Standard both require these fields to live in the campaign file itself for self-contained play — a pointer there would break mechanical completeness, not just trim prose; (2) clue/secret/hook content is interwoven into the Named Sites descriptions sentence-by-sentence (not cleanly sectioned), so surgical removal risked deleting campaign-unique content by accident. This scoping was flagged to the user in the Pass-2 handoff and TODO.md before starting.

### Files Changed
- `ai_solo_campaign/05_regions/wilderness/*.md` (all 7)
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md` — "Entering a region" wilderness-file bullet now notes the split (atmosphere in Orrun, mechanics/secrets in the campaign file)

### Canon Established
None.

### Indexes Updated
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md`

### Gaps Identified
- Dungeons/ruins (41 files) remain — same lighter-touch treatment planned (trim only pure atmosphere/"first impression" equivalent sections; leave hazards, traps, puzzles, boss mechanics, secrets, clues, treasure untouched for the same self-containment reasons as wilderness).

### Next Recommended Pass
Dungeons/ruins cleanup (41 files, `10_dungeons_and_ruins/*.md` vs `locations/vael/orrun/sites/*.md`, grouped 4 files covering 34 sites — note D23/D20, the Under-Shrine and Basin Keystone Approach, have no Orrun counterpart by design and should be skipped).

---

## 2026-08-08 — locations/vael/orrun Split: Dungeon/Ruin Duplication Cleanup (Pass 4 of 4 — COMPLETE)

### Stage
Post-Stage-16 repo-structure pass (user-directed). Completes the same-day Passes 1–3 (regions, settlements, wilderness). The `locations/vael/orrun` duplication-cleanup task is now finished across all four scoped categories.

### Summary
Trimmed all 34 dungeon/ruin files that have an `locations/vael/orrun/sites/*.md` counterpart (of 41 total files in `10_dungeons_and_ruins/`; the other 7 are the two DM-only endgame sites with no Orrun counterpart plus 5 meta/index files — see Gaps below). Two campaign templates needed different treatment:

- **Standard/environmental-template files (19 of 34):** the ones with a `## History` (with a "Publicly:"/"(Player-Safe)" clause) and `## Entrance`/`## First Impression`/`## Access / Entrance Routes` section — the Sundering Reach group (8), Ring 1 group (9), and Caradril group (2), plus 2 of the far-continent sites that happen to use this template (the Ruin'd Crown, the Ashfast Deep). These were trimmed exactly like Passes 1–3: the public/atmospheric clause replaced with a pointer into the matching `locations/vael/orrun/sites/*.md` grouped file (`SUNDERING_REACH_SITES.md`, `RING1_SITES.md`, `CARADRIL_SITES.md`, or `FAR_CONTINENT_SITES.md`), campaign-specific telegraph details (named NPCs, quest ties) kept as trailing sentences.
- **The remaining 13 far-continent sites** use a third, more compressed template (`AI Use` / `One-Sentence Identity` / `Map Placement` / `Level Range` / `Purpose` / `Access / Entrance Routes` / `Current Occupants` / `Factions Involved` / `Zone List` / ...) with no separate narrative "History" or "First Impression" prose section at all — they were apparently already written lean and campaign/NPC-focused rather than duplicating Orrun's sensory description. For these, no atmospheric prose needed removing (there wasn't any to remove); instead a one-line pointer was added ahead of the existing `## Access / Entrance Routes` numbered list, crediting Orrun for the full physical approach/entrance description while leaving every campaign-specific, NPC-gated route intact (nothing here was actually duplicative enough to delete).

As with every prior pass, all mechanical/secret content — zone/room lists, encounter lists, hazard/trap DCs, puzzles, treasure, boss/climax mechanics, retreat options, scaling notes, consequences if ignored, state update triggers, and Stage 11 clue/REV cross-links — was left completely untouched in all 34 files, per `DND_MECHANICS_REQUIREMENTS.md`'s self-containment requirement.

### Files Changed
- `ai_solo_campaign/10_dungeons_and_ruins/` — 34 dungeon/ruin files (all files with an Orrun `06_sites` counterpart):
  - Sundering Reach group (8): `THE_PEAT_CHAPEL.md`, `THE_WHISPERING_CAIRN.md`, `THE_SUNKEN_TOLLHOUSE.md`, `THE_LEDGER_VAULT.md`, `THE_DEEP_ADIT.md`, `THE_BARROW_OF_NINE_DOORS.md`, `THE_GREYFENS_DEEP.md`, `THE_CONCORD_RELAY_VAULT.md`
  - Ring 1 group (9): `THE_BURIED_CLOISTER.md`, `THE_PELLOW_GRANGE.md`, `SAINT_VEDDOWS_TOMB.md`, `THE_GREENWARD_TOLL_STATION.md`, `THE_HANGING_OAKS.md`, `THE_OLD_MAST.md`, `THE_WRECKERS_CAVES.md`, `THE_DROWNED_LAMP.md`, `THE_SKERRY_SHRINE.md`
  - Caradril group (2): `THE_SUNKEN_WARDS_DEEP.md`, `THE_CARADRIL_ASHMARKET_UNDERCROFT.md`
  - Far Continent group (15): `THE_NINE_LOCKS_SUNKEN_STAIR.md`, `THE_GLASSMERE_RELIQUARY_VAULTS.md`, `THE_THREE_BRIDGES_COUNTING_DEEP.md`, `THE_OLD_CONCORD_HEARTLANDS_RUIN.md`, `THE_MARROWDOWNS_BARROW_COMPLEX.md`, `THE_SALTMERE_DEEP_TOWNS.md`, `THE_SALLOWMARCH_DROWNED_STEPS.md`, `THE_HOLLOW_GULF_WRECK_REEF.md`, `THE_SUNHOLLOW_GREAT_GROVE.md`, `THE_HETHEWALD_OLD_HOLDS.md`, `THE_KARRAN_OLD_IRON_FORTS.md`, `THE_WENDER_SKY_STONES.md`, `THE_HIGHMARK_FROZEN_WORKS.md`, `THE_EMBERFELL_CALDERA_DESCENT.md`, `THE_CINDERN_WASTE_BURIED_WORKS.md`
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md` — "Entering a dungeon or adventure site" now points to the matching `locations/vael/orrun/sites/*.md` entry for public appearance/history/first impression, and flags that the two endgame files stay fully self-contained by design

### Canon Established
None — no world facts changed, only where existing facts are stored.

### Indexes Updated
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md`

### Gaps Identified
None outstanding for this task. The 7 `10_dungeons_and_ruins/` files intentionally left untouched: `THE_UNDER_SHRINE_APPROACH.md` (D23) and `THE_BASIN_KEYSTONE_APPROACH.md` (D20) — DM-only endgame sites with no Orrun counterpart by design — plus 5 meta/index files (`ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`, `DUNGEON_INDEX.md`, `PUZZLE_DUNGEONS.md`, `RUIN_INDEX.md`, `_PLACEHOLDER.md`), which are indexes rather than site content and have nothing to point at Orrun.

### Next Recommended Pass
The user's four-category duplication-cleanup task (regions, settlements, wilderness, dungeons/ruins) is complete. No further `ai_solo_campaign` ↔ `locations/vael/orrun` duplication cleanup is scoped; future content added to either tree should follow the same split (mechanics/secrets/NPCs in `ai_solo_campaign`, spoiler-free physical/sensory description in `locations/vael/orrun`, cross-pointer both ways) rather than reintroducing duplicated prose.

## 2026-07-28 — DungeonMaster Maps Contract Alignment

### Stage
Post-Stage-16 integration pass. Follow-up to the 2026-07-12 onboarding-prep
pass, prompted by two things: the user placed 9 generated map images into
`ai_solo_campaign/maps/assets/` needing renaming to the manifest convention,
and DungeonMaster's own maps upload contract changed upstream (commit
`038a33c`, "Derive maps S3 bucket/key from deployment config, not manifest")
in direct response to feedback raised during the 2026-07-12 pass review —
that a campaign content repo having to hand-edit a real S3 bucket name into
its own manifest was an infrastructure leak into content that shouldn't
exist. Checked the sibling `dungeonmaster` repo directly (not from memory)
to confirm the fix landed and read its exact new contract before touching
anything here.

### Summary
Renamed the user's 9 map images to the manifest's `<kind>-<slug>.png`
convention and matched them to their manifest entries (8 exact matches; 1,
"Northwest Orrun," had no existing slot — it corresponds to
`WORLD_MAP_PROMPTS.md` Prompt 1, a campaign-area cluster overview one zoom
level wider than a single region — so added a new entry,
`cluster-northwest-orrun`, using that prompt's own scale reference rather
than inventing one). Then confirmed DungeonMaster's `MapEntry` type
(`packages/shared/src/maps/manifest.ts`) now carries no storage location at
all — no `s3.bucket`, no `s3.key` — and stripped the now-obsolete `s3` block
(including the long-standing placeholder `"REPLACE_WITH_MAPS_BUCKET_NAME"`)
from all 64 manifest entries. The bucket now always resolves from the
deployment's own `MAPS_BUCKET_NAME`; the object key from
`mapObjectKey(campaignId, file)`, computed at upload/read time — the
manifest is pure campaign-authored metadata (`id`/`file`/`region`/
`caption`/`scale`/`visibility`) with no infrastructure detail baked in.
Rewrote `ONBOARDING.md`'s Maps section and the top contract table to match
(entry count 63→64, removed the now-wrong "replace the bucket placeholder"
step, added the `CAMPAIGN_ID` env var now required and cross-checked
against this repo's own `dm.campaign.json`). Confirmed `dm.campaign.json`
itself needs no change — its `campaignId` already matches what the upload
script's new cross-check expects.

### Files Changed
- `ai_solo_campaign/maps/manifest.json` — added `cluster-northwest-orrun`
  entry (64 total); stripped the `s3` block from every entry
- `ai_solo_campaign/maps/assets/*.png` — 9 files renamed to manifest
  convention (not tracked in git history — untracked at time of rename)
- `ONBOARDING.md` — Maps section rewritten for the no-bucket-in-manifest
  contract; contract table entry count corrected
- `ai_solo_campaign/00_control/TODO.md` — closed the stale "replace bucket
  placeholder" item; added the schema-alignment item; narrowed the
  remaining open item to "place remaining assets + run upload-maps.ts"

### Canon Established
None — no campaign content changed. This pass is infrastructure only.

### Gaps Identified
55 of 64 manifest entries still have no local asset in
`ai_solo_campaign/maps/assets/`. Not a blocker (`upload-maps.ts` skips
missing assets) but full map coverage needs the remaining images generated
and placed.

### Next Recommended Pass
Once a DungeonMaster deployment exists: place remaining map images, run
`upload-maps.ts` with `MAPS_BUCKET_NAME` + `CAMPAIGN_ID=the-long-remembering`
set (no tagged release needed for this step — independent of
`onboard-campaign`, idempotent, safe to re-run as more maps are added), then
separately cut a tagged release and run `onboard-campaign` for the text
content.

---

## 2026-07-12 — DungeonMaster App Onboarding Preparation

### Stage
Post-Stage-16 integration pass. Prepared this repo to be onboarded into a
separate, sibling project — **DungeonMaster** (`github.com/alduehr/
dungeonmaster`), a cloud-deployed AI DM server + React Native player app —
without changing any authored campaign content. This repo was in fact one of
DungeonMaster's own two reference points for its onboarding contract design.
Full detail lives in the new root-level `ONBOARDING.md`, not duplicated here.

### Summary
DungeonMaster's `content-pull`/`onboard-campaign` pipeline requires a
`dm.campaign.json` manifest and a verification contract (visibility
resolvability, a maps manifest, seed validity, jail-safety, a mandatory
`skills/`-rooted procedure library). Researched the target app's actual
source (server-side visibility enforcement, the frozen system prompt's
8 mandatory skill paths, the seeding fallback behavior, the maps/asset
upload pipeline) directly from its repo rather than guessing, then built:
(1) a root `dm.campaign.json` declaring `path-convention` visibility with an
exact 21-file `playerSafeGlobs` allowlist (verified 1:1 against a live
simulation of the app's own glob-matching code: 21 globs, 21 matches, 0
misses); (2) `ai_solo_campaign/maps/manifest.json`, 63 entries generated
1:1 from the existing region/city/settlement map-packet inventory, with a
clearly-flagged placeholder S3 bucket pending an actual deployment; (3)
`ai_solo_campaign/skills/`, a 6-file overlay reconciling this campaign's own
extensive session/combat/canon doctrine with the app's tool-based runtime —
most notably `procedures/session-end.md`, which translates
`SESSION_END_UPDATE_CHECKLIST.md`'s 16-file human-editing checklist onto the
app's actual state mechanism (`set_state`/`log_event`/`record_canon`/
`update_character`), since the content tree is read-only at runtime and
nothing in that checklist can be literally "updated" as a file in that
context. Deliberately declared no character/state seed — this campaign's
own conversational, session-1 character creation already matches the app's
no-seed fallback behavior exactly. Deliberately left 2 of 8 mandatory skill
paths un-overridden (`checks.md` — this campaign's DC ladder is verbatim
identical to the shared SRD file's; `rules-reference/SKILL.md` — pure SRD,
this campaign doesn't invent replacement rules).

### Files Created
- `dm.campaign.json` (repo root)
- `ONBOARDING.md` (repo root) — the full runbook; decisions, rationale, and
  the two remaining operator-side steps (maps bucket name + asset upload)
- `ai_solo_campaign/maps/manifest.json` — 63 map entries
- `ai_solo_campaign/skills/procedures/{session-start,session-end,travel,
  downtime}.md`, `ai_solo_campaign/skills/combat/SKILL.md`,
  `ai_solo_campaign/skills/canon-and-gaps/SKILL.md`

### Files Changed
- `README.md` — repository-structure block + a pointer to `ONBOARDING.md`

### Canon Established
None — no campaign content changed. This pass is infrastructure only.

### Gaps Identified
Map assets: the manifest is structurally complete but every entry's
`s3.bucket` is a placeholder pending an actual DungeonMaster deployment, and
the actual generated map image files (the user generated these separately,
outside both repos) still need to be placed under `ai_solo_campaign/
maps/assets/` and pushed via DungeonMaster's own `upload-maps.ts`. Logged as
a TODO item.

### Next Recommended Pass
Once a DungeonMaster deployment exists: replace the maps manifest's
placeholder bucket name, place the generated map assets, run `upload-maps.ts`,
cut a tagged release of this repo, and run `onboard-campaign` from the
DungeonMaster side.

---

## 2026-07-11 — Party Mode: Six-Player Conversion Layer

### Stage
Post-Stage-16 enhancement pass. The campaign remains **solo-first** (the user will play it solo initially) and now also scales to a **six-player group** (the user's home table) via a conversion overlay — **no authored file was rebalanced or rewritten**; the ~600 authored files stay the single source of truth for who/where/why/tactics/morale/outs, and three new authority files convert the math at the table.

### Files Created
- `13_encounters_and_bestiary/PARTY_SCALING_6_PLAYERS.md` — combat conversion authority (mirrors `SOLO_ENCOUNTER_SCALING.md`): the inverted action-economy problem, six-player budgets (per-character thresholds ×6, one difficulty step above four-PC math), a role-based conversion ladder for every authored solo encounter shape, chassis-step ladder keyed to the existing anchor table, boss conversion (restore solo HP cuts +25%, 2–3 legendary-style beats from existing signature abilities, adds-per-phase with the stopping-lever as party objective), apex-court note, pacing dials, cheat sheet. What never changes: DCs, morale, telegraphs, retreat, non-combat outs, clue logic.
- `01_runner_protocol/PARTY_MODE_PROTOCOL.md` — the mode itself: declared once at campaign start; three solo authorities explicitly swapped (encounter math, reward pacing, safety net) and everything else used as written; Session-1 adaptation (Sefra recruits the group; the seven Act 1 doors become a per-PC spotlight structure); companions become guides/patrons, never a seventh party member; roster-based `PLAYER_CHARACTER.md`; per-PC NPC memory attribution; party-level clues; shared story-keyed milestones; standard 5e lethality; secrecy/clocks/mysteries untouched.
- `14_treasure_and_artifacts/PARTY_REWARDS_6_PLAYERS.md` — reward conversion: coin ×4–5, consumables ×3–4 (insurance floor deleted), ~1 meaningful item per PC per tier drawn from the **same authored pools** (no new items), signature items and all 12 relics/artifacts singular and gated as written, faction standing party-wide with ranked personal rewards per-PC.

### Files Changed
- `13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md` — cross-link note ("running for a group? use PARTY_SCALING instead") + Related Files entry
- `00_control/RETRIEVAL_GUIDE.md` — new "Running the campaign for a party" load scenario
- `00_control/CONTENT_INDEX.md` (new §Party Mode) · `00_control/TAG_INDEX.md` (party-mode/six-players tag)

### Canon Established
None (no world facts; a table-mode overlay only). Design decision recorded: **party difficulty is delivered by conversion-at-the-table from the solo-authored content, not by maintaining parallel stat blocks** — one source of truth, two reading modes.

### Next Recommended Pass
None required — party mode is complete as an overlay. Optional future nicety: a one-page printable "party mode card" summarizing the conversion ladder + reward card for behind the screen.

---

## 2026-07-11 — Table-Ready Audit + Fix Pass (F1–F8)

### Stage
Post-Stage-16 verification + fix pass answering: "if printed and taken to a table, could a DM run the full campaign without ambiguity?" Scripted full-repo checks 2026-07-10/11; fixes applied 2026-07-11. No new content; no new proper nouns.

### Summary
**Audit (clean):** 2,454 markdown links (0 broken); all backtick file references resolve or are spec/template text; 110 referenced quest IDs = 110 defined (0 orphans); REV_001–010 defined; D01–D36 complete with no phantom IDs; clock T2 properly registered; travel times consistent (Hollowmere→Caradril ~10–12 days ×3 files; Caradril→Glassmere 12–16 days ×4); NW-cluster level ranges coherent; no empty/stub files; no play-file TBDs beyond by-design character-creation fields; apex-secrecy scan found no new leaks. **Findings fixed (F1–F8):** (F1) the level-range cluster — five stale `DEVELOPED_QUESTS_INDEX.md` headings corrected to the authoritative layer (quest frontmatter = NPC file = map packet, verified identical: Glassmere **9–13**, Hollow Gulf **10–15**, Emberfell **12–16**, Sallowmarch **10–14**, Hethewald **7–12**), and the three wrong values the Phase 5 pass had propagated (it trusted the stale headings) corrected in `05_regions/{GLASSMERE_LEAGUE,HETHEWALD_FREE_HOLDS,EMBERFELL_THEOCRACY}.md` (frontmatter/tags/body), `REGION_INDEX.md` (3 rows + corrected intro note), `CONTENT_INDEX.md` (3 rows), with correction notes added to the Phase 5 entries in this log and `CONSISTENCY_AUDIT.md`; (F2) two placeholder `Q_GL_XXX` hook IDs in the Cairnwater/Sennfort settlement packets relabeled as improv-safe local hooks routing to `GLASSMERE_LEAGUE_QUESTS.md`; (F3) `09_quests/_PLACEHOLDER.md` legacy scaffold names replaced with the actual file layout; (F4) `SETTLEMENT_MARROWFEN_STAIR_MAP.md` reclassified `player-safe`→`mixed` (it contains a DM-Only Layer; the only misclassified packet of 62); (F5) `15_random_tables/NPC_PERSONALITY.md` reclassified `player-safe`→`mixed` (contains DM-gating notes); (F6) `RETRIEVAL_GUIDE.md` updated — Current Status through 2026-07-11, far-region entry now loads the `05_regions/` file first, minor-factions line, new random-tables scenario block; (F7) `TAG_INDEX.md` — 2026-07 tag section (`type:random_table`, `far-region`, `minor-faction`, `phase-5`) + RtHW note corrected; (F8) `STAGE_STATUS.md` Current Status brought current through both 2026-07 passes with verdict **TABLE-READY**.

### Files Changed
`DEVELOPED_QUESTS_INDEX.md` · `05_regions/GLASSMERE_LEAGUE.md`, `HETHEWALD_FREE_HOLDS.md`, `EMBERFELL_THEOCRACY.md` · `REGION_INDEX.md` · `CONTENT_INDEX.md` · `SETTLEMENT_CAIRNWATER_MAP.md`, `SETTLEMENT_SENNFORT_MAP.md`, `SETTLEMENT_MARROWFEN_STAIR_MAP.md` · `15_random_tables/NPC_PERSONALITY.md` · `09_quests/_PLACEHOLDER.md` · `RETRIEVAL_GUIDE.md` · `TAG_INDEX.md` · `STAGE_STATUS.md` · this log · `CONSISTENCY_AUDIT.md`

### Canon Established
None. Table-use realities documented (not defects): official rulebooks required at the table for Track-A stat blocks; mixed-secrecy files are DM-eyes-only when printed; session-end bookkeeping is manual at a physical table.

### Next Recommended Pass
Begin Stage 17 (Live Campaign Operation) — Session 1 via `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`. Optional pre-play nicety: a one-page session-zero expectations sheet (grief-horror themes).

---

## 2026-07-07 — External Audit Remediation Pass, Phase 5: Deferred-Items Consolidation (C4/C5/C6; C7/C9/C10 dispositioned)

### Stage
Post-Stage-16 consolidation pass over the external report's deliberately-deferred items. **No new registered proper nouns; no new canon facts** — every name reused from the registry; new secondary/minor NPC names collision-checked. Stage 17 (Live Play) remains next.

### Summary
Executed the deferred items at the scope the repo's own rules support. **(C4)** Built canonical `05_regions/` files for all **12 far-continent regions** (Verdance Reaches, Glassmere League, Marrowdowns, Sallowmarch, Hollow Gulf, Saltmere, Concord Heartlands, Hethewald, Emberfell, Wender Steppe, Karran Marches, Sunmark) — each consolidates its authored layers (map packet, Stage 9.5 NPC roster, Stage 10 quests, Stage 12.5 dungeon, arc pack) into the standard WORLDBUILDING_STANDARDS region format, with each packet's secrecy guardrail (echo-only; never the keystone/Deep/Court) carried into the region file's DM-Only Truth. Settlement gazetteers remain the eagle-test map packets by design; full `06_settlements/` deep-builds stay deferred until play approaches. `REGION_INDEX.md`'s placeholder table replaced with the region-file table. *(Correction 2026-07-11: this pass's level-value "reconciliation" ran in the wrong direction — it trusted stale `DEVELOPED_QUESTS_INDEX` headings over the authoritative quest/NPC/packet layer for three regions. Fixed in the 2026-07-11 table-ready audit fix pass: Glassmere **9–13**, Hethewald **7–12**, Emberfell **12–16**.)* **(C5)** Caradril density expansion: `08_npcs/by_region/CARADRIL_EXPANSION_NPCS.md` (+12 secondary, +24 minor across all 8 districts + the Stillwater; Tier-2/3 fields incl. combat-relevance tags; several gated M3/M5/M6-fringe hooks) — city now ~84 named NPCs, inside the Stage 4 target band (75–100); cumulative totals now 94/380/977. **(C6)** Minor-faction layer begun: `07_factions/minor_factions/THE_TOLLMEN.md` (standalone FACTION_STANDARDS file consolidating Stage 7 canon; clock T2) + folder `README.md` defining the standalone-vs-inline rule; `FACTION_INDEX.md` gains a Minor Factions section. **(C7 — dispositioned, not built)** Per-clue files stay as `CLUE_INDEX.md` rows: ~100 stub files would duplicate index rows, create sync-drift risk, and violate the filler rule; the index is the per-clue store (create a file only if play demands one). **(C9/C10 — by design, untouched)** The player character is created with the player in Session 1; the six empty runtime baselines populate during live play.

### Files Created
- 12 region files in `05_regions/`: `VERDANCE_REACHES.md`, `GLASSMERE_LEAGUE.md`, `MARROWDOWNS.md`, `SALLOWMARCH_PROTECTORATE.md`, `HOLLOW_GULF_PORTS.md`, `SALTMERE_REACHES.md`, `CONCORD_HEARTLANDS.md`, `HETHEWALD_FREE_HOLDS.md`, `EMBERFELL_THEOCRACY.md`, `WENDER_STEPPE.md`, `KARRAN_MARCHES.md`, `SUNMARK.md`
- `07_factions/minor_factions/THE_TOLLMEN.md` + `README.md` (placeholder removed)
- `08_npcs/by_region/CARADRIL_EXPANSION_NPCS.md`

### Files Changed
- `04_world_atlas/REGION_INDEX.md` (far-region table → region files; level reconciliation) · `07_factions/FACTION_INDEX.md` (Minor Factions section) · `08_npcs/NPC_INDEX.md` (density section; totals) · `00_control/NAMING_REGISTRY.md` (Phase 5 pass note) · `00_control/CONTENT_INDEX.md` (far-region, minor-faction, NPC rows) · tracking files below

### Canon Established
- None (consolidation only). The Tollmen's standalone file restates Stage 7 canon; region files restate registry/packet/quest canon.

### Indexes Updated
- `REGION_INDEX.md`, `FACTION_INDEX.md`, `NPC_INDEX.md`, `CONTENT_INDEX.md`, `NAMING_REGISTRY.md`

### Gaps Identified
- Far-region **settlement** deep-builds (`06_settlements/` files) remain the one deliberately-open depth layer — map packets carry them at eagle-test depth; deepen per region when play approaches (unchanged in CONTENT_GAPS).

### Next Recommended Pass
- Map-image generation (external tool; the last open external-report item), or begin Stage 17 (Live Campaign Operation).

---

## 2026-07-07 — External Audit Remediation Pass, Phase 4: Bestiary Verification, RtHW Integration, Random Tables

### Stage
Post-Stage-16 enrichment + integrity pass (external-report items C2, C3, C8, plus a user-directed full monster-source verification). No new proper nouns; no canon contradicted. Stage 17 (Live Play) remains next.

### Summary
Executed the external report's Phase 4 under a strengthened rule from the user: **every beast/monster must come from real published D&D lore — no AI-invented creatures or citations.** (1) **Full Track-A verification:** every official-monster attribution in `13_encounters_and_bestiary/` was checked against the published books. Found and fixed: Oblex/Allip/Soul Monger/Deathlock/Vampiric Mist/Gloom Weaver/Gray Render misattributed to VRGtR (all MToF); Bodak misattributed (VGtM); "Hollow One" from a non-referenced setting book (replaced by the VRGtR **Reborn** lineage); several invented page numbers (removed; a book-only citation-integrity rule now governs); and one creature with **no official 5e printing at all** — "Caller in Darkness" (3e psionics) — replaced by the **Sorrowsworn** (MToF), a verified and thematically superior grief-embodiment. (2) **RtHW integration (C3):** web-verified *Ravenloft: The Horrors Within* as a real book (released 2026-06-16; 51 stat blocks CR 1/2–21, largely VRGtR creatures updated to 2024 rules + new cosmic-horror entries); integrated the verified roster Track-A (Gallows Speaker, Mist Horror, Necrichor, Bodytaker Plant/Podling, Boneless, Jiangshi, Carrionette, Brain in a Jar, Carrion Stalker, Death's Head, Dullahan, Gremishka, Nightgaunt, Gug, Shoggoth, Greater Star Spawn Emissary) into HORROR #H10–H13, BESTIARY_INDEX, MYSTERY_ENCOUNTERS, and 6 deep-horror regional files; **removed all unverifiable placeholders** (Waxworks, "Strahd Skeleton", "Mordenheim's Monster", Elder Thing, Mi-Go, Yithian, Death's Head variants, Mist Wanderer-as-creature) and all 3 NPC placeholders. (3) **Track-B chassis anchoring:** every campaign-original creature is now anchored to a named official stat block ("use X (book), modified") — master table in `BESTIARY_INDEX.md`, per-entry chassis lines in `HORROR_AND_CURSE_THREATS.md`, requirement added to Track-B rules. (4) **Random tables (C2):** built `/15_random_tables/` (TRAVEL_EVENTS, WEATHER, URBAN_EVENTS, NPC_PERSONALITY, RUMOR_SURFACES + README; placeholder removed) — all pointer-heavy, routing to existing authored content. (5) **Quest-title index (C8):** verified already exact (38/38 titles match the authored files 1:1); stale TODO closed with no changes.

### Files Created
- `15_random_tables/README.md`, `TRAVEL_EVENTS.md`, `WEATHER.md`, `URBAN_EVENTS.md`, `NPC_PERSONALITY.md`, `RUMOR_SURFACES.md` (6 files; `_PLACEHOLDER.md` removed)

### Files Changed
- `13_encounters_and_bestiary/CREATURE_SOURCE_REFERENCE.md` — corrected VRGtR list; verified RtHW integration section replaces the pending placeholder; citation-integrity rule; GoS/ToA added to source key; Track-B chassis-anchor requirement
- `13_encounters_and_bestiary/BESTIARY_INDEX.md` — source fixes; loose names exact-named (Gibbering mouther, Dust mephit, Owlbear, Harpy, Ankheg, Couatl, Panther/Lion, real fiends named); deep-water aberration resolved (Chuul/Deep Scion/Morkoth); RtHW rows added; **Track-B Official-Chassis Anchors table** (~31 creatures) added
- `13_encounters_and_bestiary/HORROR_AND_CURSE_THREATS.md` — H1–H9 sources corrected (page numbers removed); H3 rewritten Caller-in-Darkness→Sorrowsworn; chassis anchors added to Track-B entries; new #H10 Gallows Speaker, #H11 Necrichor, #H12 Preserved-Body Horrors, #H13 Mist Horror & Deep Cosmic Terrors (DM-gated)
- `13_encounters_and_bestiary/MYSTERY_ENCOUNTERS.md` — Gallows Speaker + Mist Horror/Necrichor rows added to the cross-mystery table (gated)
- `13_encounters_and_bestiary/{SUNDERING_REACH,CONCORD_HEARTLANDS,SALTMERE_REACHES,DROWNED_STEPS,HETHEWALD,MARROWDOWNS}_ENCOUNTERS.md` — RtHW horror-addition lines (all telegraphed/gated)
- `13_encounters_and_bestiary/README.md` — two-track text updated; RtHW section now "Integrated"
- `15_campaign_arcs/TIER_3_LEVELS_11_16.md` — Caller in Darkness → Sorrowsworn
- Tracking: `TODO.md` (3 Low items + C8 item closed), `CONSISTENCY_AUDIT.md` (2 issues closed; 4 resolved rows added), `CONTENT_GAPS.md` (status + treasure row updated), `OPEN_QUESTIONS.md` (RtHW question answered), `CONTENT_INDEX.md` (random-tables section added)

### Canon Established
- None (no world facts). Sourcing policy strengthened: **book-only citations; no unverified creature references; every Track-B original must carry an official-chassis anchor.**

### Indexes Updated
- `CONTENT_INDEX.md` (new §Random Tables); `BESTIARY_INDEX.md` (rows + anchor table)

### Gaps Identified
- RtHW's 2 magic **items** were not evaluated (creature pass only) — noted Low in `CONTENT_GAPS.md`. Map images (C1) remain the one open Phase 4 item; they require an external image tool.

### Next Recommended Pass
- Generate the map images per the documented prompt order (external tool), or begin Stage 17 (Live Campaign Operation) — the repo has no remaining pre-play content gaps other than optional far-region deepening.

---

## 2026-07-07 — External Audit Remediation Pass (Phases 1–3)

### Stage
Post-Stage-16 interstitial fix pass, driven by an independent external readiness/consistency report (`CAMPAIGN_READINESS_AND_CONSISTENCY_REPORT.md`, dated 2026-07-07, repo snapshot 2026-06-19). No new campaign content generated. Stage 17 (Live Play) remains next.

### Summary
Fixed all defects the external report classified as blocking runtime pointers or stale orientation docs, plus one canon naming split. Ran in three phases: (1) repointed 7 dangling file references in far-region/city map packets and a quest index that would have failed an AI DM mid-session; (2) rewrote the README and CLAUDE.md to reflect actual Stage 0–16 completion (both previously described a Stage-0 repo), added a `/15_campaign_arcs` folder note, reconciled the "18 vs 20 regions" terminology, and standardized "late autumn" → "mid-autumn" (Greyfall is the *middle* of the three autumn months per `CALENDAR.md`'s own table, not the last); (3) standardized the opening's central NPC to a single canonical name, **Wren Brevin**, across all files that previously used "Wren Hollowmere" (matches her husband Tomas Brevin and the Session-1/runtime-layer files; the codex layer was the outlier).

### Files Changed
- **Phase 1 (broken pointers):** `04_world_atlas/region_map_packets/REGION_GLASSMERE_LEAGUE.md`, `REGION_HOLLOW_GULF_PORTS.md`, `REGION_MARROWDOWNS.md`, `REGION_SALLOWMARCH_PROTECTORATE.md`, `REGION_VERDANCE_REACHES.md` (repointed nonexistent `RANDOM_ENCOUNTERS.md` to each region's own `*_ENCOUNTERS.md` + `TRAVEL_ENCOUNTERS.md`); `06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md` (nonexistent `CARADRIL_SOCIAL_ENCOUNTERS.md` → `CARADRIL_ENCOUNTERS.md`); `09_quests/by_type/QUESTS_BY_TYPE.md` (wrong path for `QC4_THE_BASIN_VOTE.md`).
- **Phase 2 (orientation docs):** `README.md` (Current Status rewrite + `/15_campaign_arcs` added to structure); `CLAUDE.md` (Repository Shape: added `/15_campaign_arcs`, documented the dual `15_` prefix); `04_world_atlas/REGION_INDEX.md` (added region-count reconciliation note); `03_canon/CALENDAR.md` + `02_runtime_state/{PLAYER_CHARACTER,NEXT_SESSION_START,CURRENT_STATE,CURRENT_LOCATION}.md` + `16_ai_session_packs/OPENING_SCENES.md` + `01_runner_protocol/TRAVEL_PROTOCOL.md` + `05_regions/{TOLLWOOD,SUNDERING_REACH,PALE_COAST,ASHGARDEN_VALE}.md` ("late autumn" → "mid-autumn", 11 occurrences).
- **Phase 3 (Wren standardization):** `08_npcs/{MAJOR_NPCS,NPC_INDEX,NPC_VOICE_GUIDE,NPC_RELATIONSHIP_WEB}.md`, `11_mysteries_and_secrets/NPC_KNOWLEDGE_MAP.md`, `09_quests/MAJOR_CAMPAIGN_QUESTS.md`, `06_settlements/COLDHEARTH.md`, `06_settlements/settlement_map_packets/SETTLEMENT_COLDHEARTH_MAP.md`, `13_encounters_and_bestiary/HORROR_AND_CURSE_THREATS.md`, `15_campaign_arcs/FINAL_REVELATION_AND_ENDING_PATHS.md`, `03_canon/DM_ONLY_CANON.md`, `00_control/NAMING_REGISTRY.md` ("Wren Hollowmere" → "Wren Brevin", 14 occurrences; registry entry annotated with the prior name for traceability).

### Canon Established
- **Wren Brevin** is the sole canonical name for the opening's returned-dead midwife (previously split between "Wren Brevin" in runtime/session files and "Wren Hollowmere" in the NPC codex). No change to her identity, secret, or role — naming only.
- Greyfall is reaffirmed as the **middle** of the three autumn months (Reaping, Greyfall, Hollowing) per `CALENDAR.md`'s own table; all "late autumn" wording was a cosmetic error and is now "mid-autumn."

### Indexes Updated
- `NAMING_REGISTRY.md` (Wren Brevin entry + Stage 7 disambiguation note updated with the prior styling for traceability).

### Gaps Identified
None new. This pass closes 3 runtime-defect items and 4 documentation-drift items identified in the external report; it does not address the report's non-blocking enrichment items (C1–C3, C8) or deliberately-deferred items (C4–C7, C9–C10), which remain open per the report's own recommendation.

### Next Recommended Pass
Per the external report's Phase 4 (enrichment, non-blocking): run the now-unblocked RtHW bestiary supplement pass, lift exact quest titles into `DEVELOPED_QUESTS_INDEX.md` for the 5 far regions still using descriptive titles, and/or populate `/15_random_tables/`. Map image rendering (C1) remains the largest table-experience gap but requires an external image-generation tool.

---

## 2026-06-18 — Strict Cartography Determinism Cleanup Pass

### Stage
Post-Stage-16 interstitial cartography pass. Pure determinism/taxonomy pass over the cartography layer (no new content, no new proper nouns). Stage 17 (Live Play) remains next.

### Summary
Applied a strict four-status taxonomy (AUTHORITATIVE / DERIVED_CANON / NOT_MAP_AUTHORITATIVE / CARTOGRAPHY_BLOCKER) to every entry in the MAP_FEATURE_REGISTRY — replacing the prior "DERIVED-CANONIZED" confidence tier, eliminating all residual LOW/MEDIUM/HIGH render-confidence labels from map-authoritative rows, and producing a clean, machine-readable status column. Added gap-section statements to the three geometry authority files (ROADS_RIVERS, WATER_AND_SHORELINE, MOUNTAINS_PASSES) confirming zero CARTOGRAPHY_BLOCKERs and classifying the remaining non-blocking items as DERIVED_CANON or NOT_MAP_AUTHORITATIVE. Fixed three far city packets that still said "DERIVED-CANONIZED" → "DERIVED_CANON". Verdict: **MAP READY WITH MINOR NON-BLOCKING GAPS** (0 CARTOGRAPHY_BLOCKERs; 7 NOT_MAP_AUTHORITATIVE items are legitimately non-placeable as fixed player-map points: South Sea Lanes edge-arrow, Star-Stones no-fixed-point, 5 DM-only hidden features).

### Files Changed
- `04_world_atlas/MAP_FEATURE_REGISTRY.md` — four-status taxonomy (AUTHORITATIVE/DERIVED_CANON/NOT_MAP_AUTHORITATIVE/CARTOGRAPHY_BLOCKER) applied to all 136 entries; old "LOW/MEDIUM/HIGH" confidence column removed from taxonomy; final counts: 57 AUTHORITATIVE, 72 DERIVED_CANON, 7 NOT_MAP_AUTHORITATIVE, 0 CARTOGRAPHY_BLOCKER.
- `04_world_atlas/ROADS_RIVERS_AND_ROUTES_AUTHORITY.md` — gap-section added: all route/river features classified; 0 CARTOGRAPHY_BLOCKERs confirmed.
- `04_world_atlas/WATER_AND_SHORELINE_AUTHORITY.md` — gap-section added: all water bodies classified; 0 CARTOGRAPHY_BLOCKERs confirmed.
- `04_world_atlas/MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md` — gap-section added: all terrain zones classified; 0 CARTOGRAPHY_BLOCKERs confirmed.
- `06_settlements/city_map_packets/GLASSMERE_CITY_MAP.md` — layout confidence: "DERIVED-CANONIZED" → "DERIVED_CANON"; explanatory text updated.
- `06_settlements/city_map_packets/CALDERPORT_CITY_MAP.md` — layout confidence: "DERIVED-CANONIZED" → "DERIVED_CANON"; explanatory text updated.
- `06_settlements/city_map_packets/ASHFAST_CITY_MAP.md` — layout confidence: "DERIVED-CANONIZED" → "DERIVED_CANON"; explanatory text updated.
- `18_audits/CARTOGRAPHY_READINESS_AUDIT.md` — Strict Cartography Determinism Cleanup Pass section added; verdict: **MAP READY WITH MINOR NON-BLOCKING GAPS**.
- Tracking: `00_control/STAGE_STATUS.md`, `00_control/CARTOGRAPHY_DETERMINISM_PROGRESS.md`.

### Canon Established
- **Four-status taxonomy** is the authoritative classification system for all map-visible features: AUTHORITATIVE (NW-cluster authored), DERIVED_CANON (far-continent committed geometry), NOT_MAP_AUTHORITATIVE (off-map/background/DM-only), CARTOGRAPHY_BLOCKER (none remain).
- **MAP READY WITH MINOR NON-BLOCKING GAPS** is the correct final verdict: 0 blockers; 7 non-map-authoritative items are legitimately non-renderable as fixed player-map points.

### Indexes Updated
- MAP_FEATURE_REGISTRY (taxonomy column); CARTOGRAPHY_READINESS_AUDIT (pass section); STAGE_STATUS (interstitial passes table, Current Status block).

### Gaps Identified
- None new. The 7 NOT_MAP_AUTHORITATIVE items (South Sea Lanes, Star-Stones, 5 DM-only) are correctly classified and non-blocking.

### Secrecy / Apex Check
- **No apex leak.** D23 (Under-Shrine Approach), the Concord Deep, the Drowned Keystone, and the Hollow Court seat are all classified NOT_MAP_AUTHORITATIVE on player maps. The endgame stays vertical beneath Hollowmere. No new proper nouns.

### Next Recommended Pass
- Generate actual map images from the authority files (the only remaining cartography work). Stage 17 (Live Play) otherwise next.

---

## 2026-06-18 — Cartography Determinism Cleanup Pass

### Stage
Post-Stage-16 interstitial cartography pass. Pure consistency/determinism cleanup over the cartography layer (no new content, no new proper nouns). Stage 17 (Live Play) remains next.

### Summary
A targeted cleanup pass that closed the residual cartography ambiguities left after the Cartography Authority + Exploration-Determinism passes. It resolved the 18-vs-19 region-count question, fixed four region-packet D-site mislabels against the authoritative adventure-site index, formalized Tollreach as a route-waypoint danger marker, introduced an explicit DERIVED-CANONIZED confidence tier and applied it to the three far cities + major far rivers/ranges/routes, corrected a 42→40 settlement-count overclaim, and reconciled all counts across the authority/audit/tracking files. No geometry was overwritten — the existing AUTHORED-CANON waypoints/polygons were already deterministic; this pass added the explicit labeling, fixed the cross-reference errors, and updated tracking. Verdict: **MAP READY.**

### Files Changed
- `04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md` — §10 definitive region-count note (18 standalone; Cindern Waste/Drowned Steps = sub-areas); §16 DERIVED-CANONIZED tier definition + BACKGROUND-ONLY note.
- `04_world_atlas/MAP_FEATURE_REGISTRY.md` — 3 far cities → "LOW (position) / DERIVED-CANONIZED (layout)"; MF-612 Tollreach → danger-marker; Registry Counts clarified (18 regions, packet counts, DERIVED-CANONIZED note).
- `04_world_atlas/ROADS_RIVERS_AND_ROUTES_AUTHORITY.md` — Hethe Tollway: Tollreach formalized as a route-waypoint danger marker (75,37), not a service settlement.
- `04_world_atlas/region_map_packets/REGION_MARROWDOWNS.md` — D-site D30→**D26** (table + DM-only + authority note rewritten).
- `04_world_atlas/region_map_packets/REGION_SALLOWMARCH_PROTECTORATE.md` — D-site D33→**D30** (table + DM-only + authority note rewritten).
- `04_world_atlas/region_map_packets/REGION_HOLLOW_GULF_PORTS.md` — Drowned Steps D33→**D30** (2 references).
- `04_world_atlas/region_map_packets/REGION_WENDER_STEPPE.md` — Sky-Stones table row D25→**D32** (table + authority note rewritten).
- `06_settlements/city_map_packets/{GLASSMERE,CALDERPORT,ASHFAST}_CITY_MAP.md` — added DERIVED-CANONIZED layout-confidence lines.
- `04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` — added deterministic-counts note (18/4/40/36; far cities DERIVED-CANONIZED; Tollreach a danger waypoint).
- `18_audits/CARTOGRAPHY_READINESS_AUDIT.md` — readiness-question region/settlement counts corrected; Tollreach + D-site findings marked RESOLVED; final verdict reworded to 18 regions; new **Cartography Determinism Cleanup Pass (2026-06-18)** section + **MAP READY** verdict.
- Tracking: `00_control/CONSISTENCY_AUDIT.md`, `CARTOGRAPHY_DETERMINISM_PROGRESS.md`, `CONTENT_INDEX.md`, `TODO.md`, `TAG_INDEX.md`, `STAGE_STATUS.md`; `17_generation_backlog/CONTENT_GAPS.md` (Tollreach + D-site gap rows closed).

### Canon Established
- Definitive region count: **18 standalone map-authoritative regions** (each with a packet). **Cindern Waste** = ash-badland terrain sub-zone within the Emberfell Theocracy region; **the Drowned Steps** = submerged-ruin sub-area (adventure site D30) within the Sallowmarch Protectorate — neither is a standalone region.
- D-site IDs (authoritative, now consistent everywhere): **D26** = Marrowdowns Barrow Complex; **D30** = Sallowmarch Drowned Steps; **D32** = Wender Sky-Stones; **D33** = Sunhollow Great Grove.
- **DERIVED-CANONIZED** confidence tier: far-feature layouts derived from registered lore are authoritative for mapping while their geographic positions stay LOW. Applied to the 3 far cities + major far rivers/ranges/routes.
- **Tollreach** is a route-waypoint danger marker at (75,37), not a service settlement.

### Indexes Updated
- MAP_FEATURE_REGISTRY counts; CONTENT_INDEX packet rows; TAG_INDEX pass entry (no new tags); CARTOGRAPHY_READINESS_AUDIT.

### Gaps Closed
- Tollreach packet gap (resolved as danger waypoint). D-site numbering discrepancy (resolved across all 4 region packets).

### Secrecy / Apex Check
- **No apex leak.** D23 (Under-Shrine Approach), the Concord Deep, the Drowned Keystone, and the Hollow Court seat remain DM-only; the endgame stays vertical beneath Hollowmere; far ruins (incl. the corrected D26/D30) remain surface/echo only. No new proper nouns.

### Next Recommended Pass
- Generate the actual map images from the now-fully-reconciled authority files + prompts (the only remaining cartography work). Stage 17 (Live Play) otherwise next.

---

## 2026-06-18 — Exploration-Determinism Pass

### Stage
Post-Stage-16 infrastructure pass. Extends the Cartography Authority Pass (2026-06-16) from "cartography-deterministic" to "exploration-deterministic." Stage 17 (Live Play) remains next.

### Summary
Made the repo exploration-deterministic. The Cartography Authority Pass (2026-06-16) established deterministic coordinate geometry for the continent, all regions, the four major cities, 18 settlements, and all 36 adventure sites. This pass expanded the settlement layer from 18 to 40 settlement map packets (16 NW cluster + 24 far-continent), bringing every reachable settlement to the "eagle-test floor": 4–8 notable areas at fixed local coordinates, services (rest, resupply, healing, info, faction contacts), law/threat DCs, NPC links from authored far-region rosters, 2–3 quest hooks, and encounter/treasure references. Phases 0–5 completed: Phase 0 (geometry reconciliation note removed), Phase 1 (full-continent geometry committed), Phase 2 (all 13 far-region map packets deepened to D&D-usable level-range/encounter/service/NPC depth), Phase 3 (3 far cities deepened to Caradril-style internal-layout depth), Phase 4 (22 new settlement packets; total 40 — initial tracking claimed 42 but a glob-verification completion pass on 2026-06-18 confirmed 7 NW cluster packets were missing and created them; corrected count is 40), Phase 5 (eagle-test audit — continent confirmed exploration-deterministic). **Eagle test PASS:** a player can fly to any point on the continent and the AI DM can (a) render a deterministic map and (b) run arrival and exploration as a scene without inventing geography, settlement layout, available locations, or services. No new campaign content, factions, NPCs, quests, mysteries, gods, artifacts, or proper nouns. All settlement-internal landmark names (inn names, market halls, district quarters, well-houses) are settlement-flavor only, not registered proper nouns.

### Files Created
- `06_settlements/settlement_map_packets/` — 22 new settlement packets (total now 40; 18 from the Cartography Authority Pass + 22 this pass; glob-verified 2026-06-18). Far-continent new: _ORCHARDMERE, _SAINT_VEDDOWS_REST, _WRACKMOUTH, _HARTFELL, _BRASKS_HOLD, _COLD_SPRINGS, _HETHEMOOT, _MARROWMOOT, _REEDMOUTH, _FENWARD, _BRACKHOLD, _CROWNMOUTH, _SUNHOLLOW, _KARRAN_GATE, _GREENWALD, _SPINE_FOOT, _PILGRIM_CAMPS, _GROVE_CAMPS (18 far). NW cluster created in verification/completion pass: _GREYWATER_HOLM, _REEDFORD, _THE_ASHWALK_REST, _TILBROOK, _COBBLE_STRAND, _COLDHEARTH, _TOLLSTONE_CROSS (7 NW; these were incorrectly claimed as done in initial tracking but were missing from disk; created after glob verification confirmed the discrepancy)
- `00_control/CARTOGRAPHY_DETERMINISM_PROGRESS.md` — progress tracker; Phases 0–5 all DONE (51/63); Phase 6 indexes pending

### Files Changed
- `18_audits/CARTOGRAPHY_READINESS_AUDIT.md` — updated from "MAP READY WITH MINOR NON-BLOCKING GAPS" to **CONTINENT IS EXPLORATION-DETERMINISTIC**
- `00_control/RETRIEVAL_GUIDE.md` — Current Status updated to include Exploration-Determinism Pass
- `00_control/STAGE_STATUS.md` — Current Status block + new interstitial pass row added
- `00_control/NAMING_REGISTRY.md` — status note prepended (no new proper nouns)
- `00_control/TODO.md` — pass recorded in Completed Recently; Medium map-image item updated
- `17_generation_backlog/CONTENT_GAPS.md` — two non-blocking gaps noted
- Various indexes (CONTENT_INDEX, TAG_INDEX, REGION_INDEX, MAP_FEATURE_REGISTRY) — updated for new settlement packets

### Canon Established
No new canon. Settlement-internal landmark names are settlement-flavor only; no new NPC, faction, region, settlement, god, artifact, or central-mystery proper nouns coined.

### Indexes Updated
CONTENT_INDEX, TAG_INDEX, REGION_INDEX, MAP_FEATURE_REGISTRY, RETRIEVAL_GUIDE.

### Gaps Identified
- Tollreach (Hethewald; Greenfinger Maddoc's camp) — a `travel_anchor` referenced in Hethemoot/region files; no standalone packet required (low-priority non-blocking).
- Pre-existing D-site numbering discrepancy: Marrowdowns packet says "D30," adventure-site index says D26; Sallowmarch says "D33," index says D30 — non-blocking; tracked in CONTENT_GAPS.

### Next Recommended Pass
Stage 17 (Live Campaign Operation). Begin via `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`. Optional: generate actual map images from the now-exploration-deterministic packets.

---

## 2026-06-16 — Cartography Authority Pass

### Stage
Post-Stage-16 infrastructure pass (no campaign content; resolves existing geography into deterministic cartographic data). Stage 17 (Live Play) remains next.

### Summary
Made the repo cartography-deterministic. Consolidated the existing continent-scale coordinate/anchor/render data into explicit geometry (polylines, polygons, points) and added the missing local-grid layers so a mapper can render player-safe and DM-only maps of the continent, every region, the four major cities, every important settlement, all named routes/water/terrain, and all 36 adventure sites without guessing. Created 5 master authority files, 18 region map packets (all map-authoritative regions; the Cindern Waste is covered within the Emberfell packet), 4 city map packets, 18 settlement map packets, 1 adventure-site cartography index, and 1 readiness audit. No new campaign content, factions, NPCs, quests, mysteries, gods, artifacts, or proper nouns — existing canon resolved into coordinates. Player-safe and DM-only map layers cleanly separated throughout; the DM-only apex (Concord Deep, Under-Shrine / Drowned Keystone, Hollow Court seat, node-network, D23) is marked never-render and the endgame kept vertical beneath Hollowmere. Verdict: **MAP READY WITH MINOR NON-BLOCKING GAPS.**

### Files Created
- `04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md` — master geometry (grid, coastline, rivers, ranges, terrain/region polygons, routes, player-safe/DM-only layers, transform)
- `04_world_atlas/MAP_FEATURE_REGISTRY.md` — single registry of ~136 map-visible features (coords, visibility, confidence)
- `04_world_atlas/ROADS_RIVERS_AND_ROUTES_AUTHORITY.md` — every road/river/sea-lane as ordered waypoints
- `04_world_atlas/WATER_AND_SHORELINE_AUTHORITY.md` — ocean/sea/lake/river/wetland geometry + crossings
- `04_world_atlas/MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md` — range spines, terrain polygons, passes
- `04_world_atlas/region_map_packets/` — 18 region packets (REGION_SUNDERING_REACH, _ASHGARDEN_VALE, _TOLLWOOD, _PALE_COAST, _CARADRIL, + 13 far regions incl. _HIGHMARK_PASSES; Cindern Waste folded into _EMBERFELL_THEOCRACY)
- `06_settlements/city_map_packets/` — 4 city packets (CARADRIL, GLASSMERE, CALDERPORT, ASHFAST)
- `06_settlements/settlement_map_packets/` — 18 settlement packets (9 NW cluster + 9 far light-anchor)
- `10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` — D01–D36 coordinate anchors + surface markers + visibility
- `18_audits/CARTOGRAPHY_READINESS_AUDIT.md` — readiness verdict

### Files Changed
- `00_control/RETRIEVAL_GUIDE.md` — status line + new "Cartography and map rendering" scenario
- `00_control/TAG_INDEX.md` — Cartography Authority Pass entry + new tags
- `04_world_atlas/REGION_INDEX.md` — region/city/settlement packet paths
- `04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`, `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md`, `FULL_WORLD_MAP_COORDINATES.md` — cross-references to the new geometry authority
- `10_dungeons_and_ruins/DUNGEON_INDEX.md` — link to the cartography index; D23-never-render note
- `00_control/CONTENT_INDEX.md`, `00_control/NAMING_REGISTRY.md`, `00_control/TODO.md`, `17_generation_backlog/CONTENT_GAPS.md` — pass recorded

### Canon Established
- No new canon. Coordinate conventions reconciled (render Y=0 top authoritative; SW-origin conversion documented). Far cities given canonical-enough placeholder internal layouts (e.g. Glassmere two-bank from "Three Bridges").

### Indexes Updated
- RETRIEVAL_GUIDE, TAG_INDEX, REGION_INDEX, DUNGEON_INDEX, CONTENT_INDEX.

### Gaps Identified
- Far-continent coastline/river meanders, far-region internal geometry, and far-city interiors remain LOW-confidence placeholders (non-blocking; improv-safe).

### Next Recommended Pass
- Stage 17 (Live Campaign Operation), or — if desired before play — generate actual map images from the now-deterministic packets.

---

## 2026-06-16 — Stage 16: Final Cleanup Pass

### Stage
Stage 16 (Pre-Play Readiness Audit) — final cleanup pass (after the correction pass).

### Summary
A final cleanup pass cleared residual secrecy classifications and stale Stage 14/15 contradictions the correction pass had not reached. No campaign content generated. Eight items fixed: (1) `PLAYER_SAFE_CANON.md` — reduced the Hollow Court secrecy note to a generic DM warning and excised the named DM-only truths (surviving Custodians, the harvest, the Under-Shrine / Drowned Keystone, the Concord Deep) from the player-safe body. (2) The map render manifest and generation packet body text — corrected the contradictory "this file is player-safe / no DM-only geography" wording to state the *output* is player-safe but the *file* is DM-facing (lists hidden "do not render" names) and is never handed to the player. (3) `18_audits/PLAYER_SAFE_FULL_CONTINENT_MAP_AUDIT.md` — reclassified `player-safe` → `dm-facing` with a note. (4) Four `player-safe` files carrying apex/harvest terms reclassified `mixed` with DM secrecy notes (`CREATURE_SOURCE_REFERENCE.md`, `BIOME_ENCOUNTER_MATRIX.md`, `REWARDS_BY_LEVEL.md`, `CONSUMABLES_AND_MINOR_MAGIC.md`). (5) `CONSISTENCY_AUDIT.md` top status corrected so it no longer reads as if Stage 14 is most recent / endgame artifacts pending Stage 15. (6) `REWARD_PLACEMENT_AUDIT.md` — Stage 15/15B update note resolving the "endgame artifact mechanics pending Stage 15" forward note. (7) `CONTENT_GAPS.md` — stale NPC counts corrected to 94 major / 368 secondary / 953 minor and marked resolved. (8) `MANIFEST.md` — added `/15_campaign_arcs` to the folder map and clarified `/12_campaign_arc` as the legacy Act 1 folder. **Verdict stands: READY FOR LIVE PLAY.** Stage 17 may begin.

### Files Created
- None.

### Files Changed
- `03_canon/PLAYER_SAFE_CANON.md` — Hollow Court secrecy note reduced to generic DM warning
- `04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`, `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` — body text made consistent with `dm-facing` classification
- `18_audits/PLAYER_SAFE_FULL_CONTINENT_MAP_AUDIT.md` — reclassified `dm-facing` + note
- `13_encounters_and_bestiary/CREATURE_SOURCE_REFERENCE.md`, `BIOME_ENCOUNTER_MATRIX.md` — reclassified `mixed` + secrecy notes
- `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md`, `CONSUMABLES_AND_MINOR_MAGIC.md` — reclassified `mixed` + secrecy notes
- `14_treasure_and_artifacts/REWARD_PLACEMENT_AUDIT.md` — Stage 15/15B endgame-artifact update note
- `00_control/CONSISTENCY_AUDIT.md` — top status corrected (no stale Stage 14/15 contradiction)
- `17_generation_backlog/CONTENT_GAPS.md` — NPC counts corrected to 94/368/953; entries marked resolved
- `00_control/MANIFEST.md` — `/15_campaign_arcs` added to folder map; `/12_campaign_arc` clarified as legacy
- `00_control/STAGE_16_PROGRESS.md` — Final Cleanup Pass section + status set to COMPLETE — READY FOR LIVE PLAY
- `18_audits/PRE_PLAY_READINESS_AUDIT.md`, `STAGE_16_BLOCKERS_AND_FIXES.md` (C9–C16), `STAGE_16_DM_ONLY_SECRECY_AUDIT.md`, `STAGE_16_RETRIEVAL_AUDIT.md`, `STAGE_16_PRE_PLAY_READINESS_AUDIT.md` — final-cleanup-pass notes
- `00_control/PROGRESS_LOG.md`, `TODO.md`, `STAGE_STATUS.md`, `NAMING_REGISTRY.md` — tracking updated

### Canon Established
- None. No new campaign content or proper nouns.

### Next Recommended Pass
- Stage 17 (Live Campaign Operation): begin Session 1 via `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`.

---

## 2026-06-16 — Stage 16: Correction Pass

### Stage
Stage 16 (Pre-Play Readiness Audit) — targeted correction pass.

### Summary
The prior two Stage 16 passes declared READY but overclaimed on control/retrieval/classification/hygiene — they verified content runnability deeply but missed several navigation, accuracy, and secrecy-classification defects that were not content gaps. This pass found and fixed 8 of them (C1–C8), generating no new campaign content. (1) Rewrote the stale `RETRIEVAL_GUIDE.md` (was Stages 1–5/7 only) into a full per-scenario load map covering every Stage 8–15B system on disk. (2) Updated the stale `MANIFEST.md` (was "Stage 1 complete / Stage 2 next") to Stages 0–16 complete / Stage 17 next, with a corrected stage table and live-play entry pointer. (3) Created the missing master `18_audits/PRE_PLAY_READINESS_AUDIT.md` (Stage 16's named required output) pointing to the six detailed reports. (4) Refreshed stale active-folder `_PLACEHOLDER.md` files to reflect real contents. (5) Reclassified 3 map-render files to `secrecy: dm-facing-player-safe-output` (they name apex secrets only in "do-not-render" lists) and `LANGUAGES.md`/`LEVELING_ASSUMPTIONS.md` to `mixed` (they carried DM-only apex/act labels under a player-safe tag); annotated the `PLAYER_SAFE_CANON.md` Hollow-Court entry. (6) Created `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` (a by-tier forwarding index referenced as "when built" but never created) and repointed stale references. (7) Closed/reclassified stale Medium issues in `CONSISTENCY_AUDIT.md` and `CONTENT_GAPS.md` (REWARDS_BY_LEVEL, Acts 2–5, endgame artifacts, NPC tools; Caradril density → non-blocking optional). (8) Expanded the Stage 16 definition in `DEVELOPMENT_STAGES.md` to match what the stage actually requires. **Verdict stands: READY FOR LIVE PLAY** on a fully reconciled repo; Stage 17 may begin.

### Files Created
- `18_audits/PRE_PLAY_READINESS_AUDIT.md` — master readiness verdict
- `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` — by-tier reward forwarding index

### Files Changed
- `00_control/RETRIEVAL_GUIDE.md` — full rewrite (per-scenario load map through 15B)
- `00_control/MANIFEST.md` — status / stage table / folder summary made current
- `00_control/CONSISTENCY_AUDIT.md` — stale Medium issues closed; Caradril density reclassified
- `00_control/CONTENT_INDEX.md` — added REWARDS_BY_LEVEL + master readiness audit rows
- `00_control/TAG_INDEX.md` — Stage 16 correction-pass entry + `dm-facing-player-safe-output` tag value
- `00_control/STAGE_STATUS.md` — Stage 16 row + most-recent-pass updated
- `00_control/DEVELOPMENT_STAGES.md` — expanded Stage 16 standard
- `00_control/STAGE_16_PROGRESS.md` — correction-pass section + post-correction verdict
- `00_control/NAMING_REGISTRY.md` — status header updated (no new proper nouns)
- `03_canon/PLAYER_SAFE_CANON.md` — Hollow-Court folklore-only secrecy note; status header
- `03_canon/LANGUAGES.md`, `03_canon/LEVELING_ASSUMPTIONS.md` — reclassified `mixed` + secrecy notes
- `04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md`, `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`, `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` — reclassified `dm-facing-player-safe-output` + notes
- 8 `_PLACEHOLDER.md` files (05_regions, 06_settlements, 07_factions/major_factions, 07_factions/minor_factions, 08_npcs, 09_quests, 18_audits, 15_random_tables) — status refreshed
- `18_audits/STAGE_16_BLOCKERS_AND_FIXES.md` — correction-pass section (C1–C8)
- `18_audits/STAGE_16_RETRIEVAL_AUDIT.md`, `STAGE_16_PRE_PLAY_READINESS_AUDIT.md` — correction notes added
- `18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md` — stale items marked resolved
- `17_generation_backlog/CONTENT_GAPS.md` — stale framing corrected; resolved gaps closed
- `10_dungeons_and_ruins/THE_BARROW_OF_NINE_DOORS.md`, `09_quests/regional_quests/Q_RACE_NORTH.md` — REWARDS_BY_LEVEL references repointed

### Canon Established
- None. No new campaign content or proper nouns.

### Next Recommended Pass
- Stage 17 (Live Campaign Operation): begin Session 1 via `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`.

---

## 2026-06-15 — Stage 16: Deep Re-Verification Pass (second run)

### Stage
Stage 16 (Pre-Play Readiness Audit) — full from-scratch re-audit.

### Summary
Re-ran the Stage 16 readiness audit from scratch because the first pass was shallow, this time verifying every claim by reading the actual files rather than trusting index summaries. Reset and re-completed `STAGE_16_PROGRESS.md` with per-category evidence. Read all 8 canon files + 2 arc files and cross-checked the apex chain across all three secrecy tiers; opened all 16 runtime state files (9 seeded, 7 correctly templated); read REVELATION_MAP in full and traced two clue trails to their source clue files; opened the opening NPC cast, one Act 1 dungeon, the DM-only endgame site, one quest, one encounter table, and the 12-artifact index to confirm mechanical completeness and apex gating; grepped the runner protocols for placeholders (none in play-ready content). **Result: 0 new blockers; verdict re-confirmed READY FOR LIVE PLAY on evidence.** No content changes were needed — the prior pass's two hygiene fixes (canon status headers; the `15_campaign_arcs/` arc pointer) were verified still correct. Added deep-re-verification notes to the master audit report and the blockers ledger. One item examined and cleared as a non-defect: the legacy "R1–R8" labels in `SECRET_REVEAL_PROTOCOL.md` map 1:1 to REV_001–010 per REVELATION_MAP, so they are consistent.

### Files Changed (re-verification pass)
- `00_control/STAGE_16_PROGRESS.md` — reset to a real per-category checklist, then re-completed with evidence
- `18_audits/STAGE_16_PRE_PLAY_READINESS_AUDIT.md` — added a deep-re-verification record to the summary
- `18_audits/STAGE_16_BLOCKERS_AND_FIXES.md` — added a deep-re-verification section (0 new blockers)
- `00_control/PROGRESS_LOG.md`, `CONSISTENCY_AUDIT.md` — this entry / re-audit note

---

## 2026-06-15 — Stage 16: Pre-Play Readiness Audit

### Stage
Stage 16 (Pre-Play Readiness Audit).

### Summary
Ran the whole-repository pre-play readiness audit across all 16 Stage 16 categories (canon/contradiction, player-safe vs DM-only, runtime, retrieval, starting play, full arc, regional, quest, mystery/clue, faction, NPC, dungeon, encounter/bestiary, treasure, mechanical, file hygiene). **Verdict: READY FOR LIVE PLAY** — 0 Critical / 0 High / 2 Medium (both fixed in-pass) / 4 Low (non-blocking, documented). The foundation is sound: the opening is immediately runnable from `START_NEW_CAMPAIGN_PROMPT.md`, all 16 runtime state files are present and seeded, the level 1–20 arc is findable/linked, the apex secret (the harvest / deliberate Quietfall / Hollow Court / keystone / steering) never leaks into any player-facing file and is gated behind REV_007 (L13+) and the single DM-only endgame dungeon, REV_001 is reachable via 5 independent clue sources, all 7 factions are clocked, and every major index is present and current. **Two hygiene blockers fixed:** (1) three stale canon "Current Status" headers (`CANON.md`/`PLAYER_SAFE_CANON.md`/`DM_ONLY_CANON.md` said Stage 1/1–5/1–5+7 while the bodies were already current) updated to "Stages 1–15B complete; Stage 16 underway"; (2) added an arc-forwarding pointer from `12_campaign_arc/MAIN_ARC_OVERVIEW.md` to the runnable `15_campaign_arcs/` set. No new campaign content was generated. The campaign may proceed to Stage 17 (Live Campaign Operation).

### Files Created
- `18_audits/STAGE_16_PRE_PLAY_READINESS_AUDIT.md` — master audit (16 categories; severity tables; final verdict)
- `18_audits/STAGE_16_BLOCKERS_AND_FIXES.md` — issue ledger (2 fixed, 5 deferred)
- `18_audits/STAGE_16_PLAYER_SAFE_START_AUDIT.md` — Session-1 runnability checklist
- `18_audits/STAGE_16_DM_ONLY_SECRECY_AUDIT.md` — apex-leak scan (0 leaks) + DM-file marking
- `18_audits/STAGE_16_RETRIEVAL_AUDIT.md` — index inventory + cross-link spot checks
- `18_audits/STAGE_16_FULL_ARC_PLAYABILITY_AUDIT.md` — L1–20 tier coverage + open-world resilience
- `00_control/STAGE_16_PROGRESS.md` — Stage 16 progress tracker (COMPLETE)

### Files Changed
- `03_canon/CANON.md`, `PLAYER_SAFE_CANON.md`, `DM_ONLY_CANON.md` — stale "Current Status" headers corrected
- `12_campaign_arc/MAIN_ARC_OVERVIEW.md` — added the `15_campaign_arcs/` arc-forwarding pointer
- `00_control/CONTENT_INDEX.md` (status header + 6 audit-report rows), `STAGE_STATUS.md` (Stage 16 → complete; Stage 17 ready; row added), `TODO.md` (Stage 16 done; Stage 17 queued), `CONSISTENCY_AUDIT.md` (Stage 16 self-check), `OPEN_QUESTIONS.md` (status), `NAMING_REGISTRY.md` (status header), `17_generation_backlog/CONTENT_GAPS.md` (status)

### Canon Established
None. Audit/cleanup stage — no new world facts, proper nouns, mysteries, factions, gods, or artifacts.

### Indexes Updated
`CONTENT_INDEX.md` (status + audit reports). All per-category indexes verified present and current (no content changes required).

### Gaps Identified
All non-blocking and previously tracked: far-region settlement/NPC deep-builds (optional, deepen on approach); map images not generated; `/15_random_tables/` empty; RtHW pending (2026-06-16).

### Next Recommended Pass
Stage 17 — Live Campaign Operation. Begin Session 1 via `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`; after each session run `SESSION_END_UPDATE_CHECKLIST.md`; run periodic live audits (Stage 18) every 3–5 sessions / after level-ups / before new regions or acts.

---

## 2026-06-15 — Stage 15B: Full Character Arc Playability Fill

### Stage
Stage 15B (Full Character Arc Playability Fill) — a concrete play-layer fill over the Stage 15 frameworks.

### Summary
Stage 15 produced high-level reference frameworks ("see file X"); Stage 15B fills every region and tier with **concrete, named, runnable** content so the AI DM can run sessions in any major region at any appropriate tier without inventing major structure. **First action was a verification audit:** the prior `STAGE_15B_PROGRESS.md` falsely claimed COMPLETE while most target files were missing on disk; the progress file was corrected to reflect reality before any new writing. Then built the 9 missing play-layer files + 6 legacy forwarding stubs, and patched the two pre-existing Stage 15B files. Every situation, event, and consequence names the NPC, faction, location, action, and consequence (no vague summaries). Apex (REV_007/Hollow Court/Custodians/harvest/keystone) kept DM-only and gated to L13+; far sources never deliver it. **No new proper nouns** (verified against `NAMING_REGISTRY.md`); no canon contradicted. Completion audit: PASS.

### Files Created
- `15_campaign_arcs/TIER_3_PLAYABLE_PATHS_LEVELS_11_16.md` — 6 concrete Tier 3 paths (Glassmere, Marrowdowns, Emberfell, Saltmere, Highmark/Steppe, Concord Heartlands).
- `15_campaign_arcs/TIER_4_PLAYABLE_PATHS_LEVELS_17_20.md` — 9 endgame playbooks (Confrontation, Alliance, Artifact, Ritual, Political, Exposure, Sacrifice, Partial/Bittersweet, Catastrophic Failure).
- `15_campaign_arcs/REGION_TO_REGION_TRANSITION_GUIDE.md` — every inter-region route (level/type/time/hook/complication/en-route clue) + "where can I go?" router by tier.
- `15_campaign_arcs/CONTINENTAL_PRESSURE_TIMELINE.md` — 16+ named events as the world moves without the player (all 7 factions, 8+ regions; clocks + rumors).
- `15_campaign_arcs/PLAYER_IGNORES_MAIN_ARC_GUIDE.md` — per-tier named world-states if the arc is ignored; reintroduction techniques; side-content payoff.
- `15_campaign_arcs/PLAYER_GOES_ANYWHERE_GUIDE.md` — off-route arrivals (too early/late, skipping Caradril/Ring 1, low-level far travel, the under-shrine guard rail).
- `15_campaign_arcs/ENDGAME_REGION_PLAYBOOK.md` — per-region Tier 4 state and which endings each region contributes to.
- `15_campaign_arcs/FINAL_REVELATION_AND_ENDING_PATHS.md` — REV_001–010 with 3 route-independent paths each + redundancy table; the 5 endings (requirements/site/resolution/fates).
- `15_campaign_arcs/STAGE_15B_COMPLETION_AUDIT.md` — Stage 15B pass/fail audit (PASS).
- Legacy forwarding stubs: `ACT_2_LEVELS_5_8.md`, `ACT_3_LEVELS_9_12.md`, `ACT_4_LEVELS_13_16.md`, `ACT_5_LEVELS_17_20.md`, `VILLAIN_ESCALATION.md`, `ENDGAME_STATES.md`.

### Files Changed
- `15_campaign_arcs/REGIONAL_ARC_PACKS_LEVEL_5_TO_20.md` — Highmark Passes (§18) expanded to 3 playable situations; added the Cindern Waste sub-region (§12b) with full playable content; clarified the Drowned Steps coverage note in Sallowmarch (§13).
- `15_campaign_arcs/FULL_WORLD_LEVEL_5_TO_20_PLAYABILITY.md` — added the Cindern Waste row to the region×tier matrix.
- `00_control/STAGE_15B_PROGRESS.md` — corrected from false-COMPLETE to verified state, then to final accurate completion.
- `00_control/STAGE_15_PROGRESS.md`, `CONTENT_INDEX.md`, `TAG_INDEX.md`, `TODO.md`, `17_generation_backlog/CONTENT_GAPS.md` — updated for Stage 15B.

### Canon Established
None. Stage 15B is a play-layer fill over existing systems; no new world facts, proper nouns, mysteries, factions, gods, or artifacts.

### Indexes Updated
`CONTENT_INDEX.md` (Stage 15B sub-table + header), `TAG_INDEX.md` (Stage 15B tag entry).

### Gaps Identified
Far-region settlement/NPC deep-builds remain light (the arc packs lean on Stage 9.5 rosters + Stage 12.5 dungeons) — a future deepening, not a playability blocker. Logged in `CONTENT_GAPS.md`.

### Next Recommended Pass
Stage 16 — Pre-Play Readiness Audit (run `AUDIT_STANDARDS.md` repo-wide; produce `18_audits/PRE_PLAY_READINESS_AUDIT.md`; re-verify Stage 15B aligns with the Stage 15 frameworks and `REVELATION_MAP.md`).

---

## 2026-06-15 — Stage 15: Level 5–20 Campaign Arc Expansion

### Stage
Stage 15 (Level 5–20 Arc Expansion).

### Summary
Built the complete level 5–20 campaign arc as 15 structured files in the new `15_campaign_arcs/` folder (distinct from `15_random_tables/`), letting an AI DM run the campaign from level 5 to 20 for one solo player. The pass is a **play-layer pass over existing systems** — it references Stage 8 clocks, Stage 9 NPCs, Stage 10 quests, Stage 11 mysteries (REV_001–010 / M0–M10), Stage 12/12.5 dungeons (D01–D36), Stage 13 bestiary, and Stage 14 treasure **by reference, without rewriting any of them**. Used **tier** language per the spec (Tier 2/3/4 = L5–10/11–16/17–20) and bound it to the existing **act** language (Acts 2–5) via a crosswalk. Open-world (no mandatory quest sequence, no assumed faction, no fixed region order, no single correct ending; every revelation 3+ paths), solo-runnable (per-tier balance + missing-ability fallbacks + boss adjustments), and apex-protected (REV_007 / the Hollow Court gated to L13+ convergence/descent/heretic; far sources never deliver it; player-safe summaries never name the Court/harvest/Custodians/keystone-truth). Ran an internal readiness audit (PASS; 0 Critical/0 High/2 Medium/3 Low).

### Files Created
- `15_campaign_arcs/LEVEL_5_TO_20_OVERVIEW.md` — master overview; tier↔act crosswalk; per-tier entry-state; open-world/secrecy/solo spine.
- `15_campaign_arcs/TIER_2_LEVELS_5_10.md` — Act 2 + lower Act 3; Ring 1 + Caradril + Verdance corridor; REV_002/003/004; factions go regional.
- `15_campaign_arcs/TIER_3_LEVELS_11_16.md` — Act 3 upper + Act 4; far continent; REV_005/006/009; the REV_007 apex gate (L13+); Veyl; REV_010.
- `15_campaign_arcs/TIER_4_LEVELS_17_20.md` — Act 5 endgame; vertical descent; REV_007 owned; REV_008 the choice.
- `15_campaign_arcs/CAMPAIGN_ESCALATION_TIMELINE.md` — chronological clock/world-state escalation by tier; master trajectory; passive failsafe.
- `15_campaign_arcs/MAIN_ARC_REVELATION_SEQUENCE.md` — how M1–M9/REV gates are earned & revealed; 3+ redundant routes; apex protection.
- `15_campaign_arcs/REGIONAL_ESCALATION_PATHS.md` — how each region changes across tiers; player-safe vs DM-only; fall/stabilize/revolt/ally/corrupt.
- `15_campaign_arcs/FACTION_ESCALATION_PATHS.md` — faction escalation/divergence; Q*4 → endgame posture matrix; conflict activation by tier.
- `15_campaign_arcs/VILLAIN_AND_APEX_THREAT_ESCALATION.md` — Hollow Court/Custodians escalation by revelation; Veyl as choice-boss; recurring-villain track (DM-only).
- `15_campaign_arcs/ENDGAME_STRUCTURE.md` — 9 approaches × 5 outcomes (seal/restart/seize/destroy/transform); reachability matrix; faction-outcome sketch; artifact fates.
- `15_campaign_arcs/FAILURE_STATES_AND_WORLD_CONSEQUENCES.md` — ignored-threat/failure consequences by tier; per-threat × per-tier table; passive failsafe.
- `15_campaign_arcs/LEVELING_AND_MILESTONE_GUIDE.md` — milestone leveling 5–20; no-grind; multiple approaches per milestone (DM-only).
- `15_campaign_arcs/SOLO_CAMPAIGN_BALANCE_GUIDE.md` — one-PC balance per tier; missing-ability fallbacks; boss adjustments (DM-only).
- `15_campaign_arcs/OPEN_WORLD_CONTINUITY_GUIDE.md` — non-linear path handling; 5 continuity anchors; anti-stall hooks; state discipline (DM-only).
- `15_campaign_arcs/STAGE_15_READINESS_AUDIT.md` — pre-completion arc audit (PASS).
- `00_control/STAGE_15_PROGRESS.md` — Stage 15 progress tracker.

### Files Changed
- `00_control/CONTENT_INDEX.md` — added the Level 5–20 Arc (Stage 15) sub-section (15 files); updated Current Status.
- `00_control/TAG_INDEX.md` — added the Stage 15 tag note; updated Current Status header.
- `00_control/TODO.md` — Stage 15 marked done; Stage 16 set as next.
- `17_generation_backlog/CONTENT_GAPS.md` — Stage 15 gaps closed/noted.
- `02_runtime_state/WORLD_CLOCKS.md` — Stage 15 tier-entry clock-state reference appended.
- `02_runtime_state/FACTION_STATE.md` — Stage 15 tier-entry faction-posture reference appended.
- `03_canon/CANON.md` — Canon Revision Log line added (Stage 15 = structural play-layer pass; no new world facts).

### Canon Established
- None (no new world facts). Stage 15 is a structural/play-layer pass over existing canon. Recorded as a revision-log line.

### Player-Safe Facts Added
- None new. The tier files surface only already-established player-safe framing.

### DM-Only Facts Added
- None new. Existing DM-only truths are re-sequenced for levels 5–20 with strengthened apex protection.

### Runtime State Updated
- `WORLD_CLOCKS.md` and `FACTION_STATE.md` got Stage 15 tier-entry *reference* sections (no live-state changes; campaign-start baseline preserved).

### Indexes Updated
- `CONTENT_INDEX.md`, `TAG_INDEX.md`.

### Gaps Identified
- (Optional) indexer spot-check that every cited quest ID resolves to a file; (optional) add a forwarding pointer from `12_campaign_arc/MAIN_ARC_OVERVIEW.md` to `15_campaign_arcs/`. Both non-blocking.

### Next Recommended Pass
- **Stage 16 — Pre-Play Readiness Audit.** Run `AUDIT_STANDARDS.md` against the whole repo; produce `18_audits/PRE_PLAY_READINESS_AUDIT.md`; verify the first 10–20 sessions are runnable and the apex stays protected.

---

## 2026-06-15 — Stage 14 bookkeeping and cross-index cleanup pass

### Stage
Interstitial (post-Stage-14 cleanup; Stage 15 is next).

### Summary
Corrected dungeon-reward-hook count from "39 sites" to "36 authored adventure sites" across all tracking files (STAGE_14_PROGRESS, PROGRESS_LOG, TODO, STAGE_STATUS, CONTENT_INDEX, EXPANSION_PLAN, DUNGEON_REWARD_INDEX Coverage section); the DUNGEON_REWARD_INDEX has 36 bullet entries matching the DUNGEON_INDEX (D01–D36). Confirmed custom item count language consistent at "38 custom magic items + 12 artifacts" across all Stage 14 files (no changes needed). Updated OPEN_QUESTIONS status block to show Stage 14 complete / Stage 15 next. Added Stage 14 audit note to CONSISTENCY_AUDIT. Fixed EXPANSION_PLAN Pass-12 entry from "RECOMMENDED NEXT" to "DONE." Added "Reward Links" cross-reference section to QUEST_INDEX; added DUNGEON_REWARD_INDEX cross-reference to DUNGEON_INDEX; added FACTION_REWARDS cross-reference to FACTION_INDEX. Added Stage 14 artifact/relic secrecy note to SECRET_INDEX. Added Stage 14 reward-relic clue-delivery note to CLUE_INDEX (clarifying relics support existing clue paths; all required paths remain in CLUE_INDEX/MYSTERY_WEB).

### Files Changed
- `00_control/OPEN_QUESTIONS.md` — status block updated
- `00_control/CONSISTENCY_AUDIT.md` — Stage 14 audit note prepended
- `17_generation_backlog/EXPANSION_PLAN.md` — Pass-12 entry updated to DONE; Later Expansion list updated; "39 sites" → "36 sites"
- `14_treasure_and_artifacts/DUNGEON_REWARD_INDEX.md` — Coverage section: "39 sites" → "36 authored adventure sites"
- `00_control/STAGE_14_PROGRESS.md` — two "39 sites" → "36 sites"
- `00_control/PROGRESS_LOG.md` — "39 sites" → "36 sites"; this entry added
- `00_control/TODO.md` — two "39 sites" → "36 sites"
- `00_control/STAGE_STATUS.md` — "39 sites" → "36 sites"
- `00_control/CONTENT_INDEX.md` — "39 sites" / "39 dungeons" → "36"
- `09_quests/QUEST_INDEX.md` — Reward Links section + related-files link added
- `10_dungeons_and_ruins/DUNGEON_INDEX.md` — DUNGEON_REWARD_INDEX cross-reference added
- `07_factions/FACTION_INDEX.md` — FACTION_REWARDS cross-reference added
- `11_mysteries_and_secrets/SECRET_INDEX.md` — Stage 14 artifact/relic secrets note added
- `11_mysteries_and_secrets/CLUE_INDEX.md` — Stage 14 reward-relic clue-delivery note added

### Canon Established
None. Bookkeeping only.

### Indexes Updated
QUEST_INDEX, DUNGEON_INDEX, FACTION_INDEX, SECRET_INDEX, CLUE_INDEX — cross-references to Stage 14 reward files added.

### Gaps Identified
None new.

### Next Recommended Pass
Stage 15: Level 5–20 Arc Expansion (Acts 2–5, VILLAIN_ESCALATION.md, ENDGAME_STATES.md).

---

## 2026-06-14 — Stage 14: Treasure, Artifacts, and Rewards

### Stage
Stage 14 (Treasure, Artifacts, and Rewards).

### Summary
Built the complete solo-tuned reward layer: 15 files in `14_treasure_and_artifacts/`. Master `TREASURE_INDEX` routes every reward need; `SOLO_REWARD_BALANCE` is the single-PC pacing governor (breadth over spikes; no flat +X before Rare; recovery/utility/access weighted up; generous consumables; insurance floor; no solve-everything item). **12 named artifacts/relics** (`ARTIFACT_INDEX`, all ORIGINAL CAMPAIGN ITEMS, mystery-gated with DM-only true-nature blocks); **38 custom magic items** (`MAGIC_ITEM_INDEX`, Common→Legendary; 48 originals incl. artifacts); **10 cursed items + 3 endgame cursed-class** (`CURSED_ITEMS`, all telegraphed + recoverable); **6 sentient items** (`SENTIENT_ITEMS`, run as mini-NPCs, incl. 1 DM-only Hollow Court plant). Region/level coverage: `REGIONAL_TREASURE_TABLES` (all 20 regions × 5 level bands), `CONSUMABLES_AND_MINOR_MAGIC`, `ECONOMY_AND_PRICING_GUIDE`. Reward hooks: `FACTION_REWARDS` (7 majors + 4 Caradril blocs, ranked R1–R3 + betrayal; Hollow Court = no clean rewards, all gifts are traps), `QUEST_REWARD_INDEX` (palettes by category, noncombat parity), `DUNGEON_REWARD_INDEX` (36 sites), `NONCOMBAT_REWARDS` (political/social/info/access/relationship/economic/reputation). `REWARD_PLACEMENT_AUDIT` PASS (0 Critical/High/Medium). Two-track source handling: official D&D items = reference-only (name/source/rarity/fit/placement; **no copied text or stats**); custom items = abbreviated 5e prose. **No early apex-truth exposure** — endgame artifacts (Quiet Country Vessel, Harvest Engine Shard, Last Voice) require M6–M9; Remembrance relics are plot-before-power (Thin-touch risk); no easy resurrection items. No new factions/NPCs/regions/mysteries/gods/cosmology; 12 artifact proper nouns registered.

### Files Created
- `14_treasure_and_artifacts/`: `TREASURE_INDEX.md`, `SOLO_REWARD_BALANCE.md`, `MAGIC_ITEM_INDEX.md`, `ARTIFACT_INDEX.md`, `CURSED_ITEMS.md`, `SENTIENT_ITEMS.md`, `CONSUMABLES_AND_MINOR_MAGIC.md`, `REGIONAL_TREASURE_TABLES.md`, `FACTION_REWARDS.md`, `QUEST_REWARD_INDEX.md`, `DUNGEON_REWARD_INDEX.md`, `NONCOMBAT_REWARDS.md`, `ECONOMY_AND_PRICING_GUIDE.md`, `REWARD_PLACEMENT_AUDIT.md`, `README.md` (replaces `_PLACEHOLDER.md`, deleted)
- `00_control/STAGE_14_PROGRESS.md`

### Files Changed
- `00_control/CONTENT_INDEX.md`, `00_control/TAG_INDEX.md`, `00_control/NAMING_REGISTRY.md`, `00_control/STAGE_STATUS.md`, `00_control/TODO.md`, `17_generation_backlog/EXPANSION_PLAN.md`, `17_generation_backlog/CONTENT_GAPS.md`

### Canon Established
- No new world facts. The reward layer formalizes existing Remembrance-relic lore into usable items. 12 artifacts reuse already-registered faction/mystery/cosmology roots; the keystone/Court/harvest stay DM-only and gated.

### Indexes Updated
- CONTENT_INDEX (new Treasure section + status line), TAG_INDEX (Stage 14 bullet + tags), NAMING_REGISTRY (12 artifacts + status block), STAGE_STATUS (Stage 14 → complete, Stage 15 next).

### Gaps Identified
- RtHW (June 16 2026) could add 1–2 Track-A cursed/relic references later (low priority). Endgame artifact mechanics intentionally light pending Stage 15 Act 4–5 builds.

### Next Recommended Pass
- Stage 15: Level 5–20 Arc Expansion (Acts 2–5, villain escalation, endgame states). Pull reward placements from `14_treasure_and_artifacts/`; keep endgame artifacts M6–M9 gated.

---

## 2026-06-14 — Stage 13 Cleanup / Official-Source-Reference / RtHW-Pending Pass

### Stage
Stage 13 (Encounter and Bestiary Expansion) — cleanup and source-reference pass.

### Summary
Closed out Stage 13 in all tracking files and cleaned up source references. Marked Stage 13 **complete (100%)** and Stage 14 (Treasure, Artifacts, Rewards) **next** in STAGE_STATUS, EXPANSION_PLAN, TODO, OPEN_QUESTIONS, CONSISTENCY_AUDIT, and the NAMING_REGISTRY status block. Replaced `13_encounters_and_bestiary/_PLACEHOLDER.md` with a real folder `README.md` (at-a-glance summary, full file list, two-track source approach, RtHW-pending note, in-play navigation). Mapped **Track-A official-monster source shorthands** across `BESTIARY_INDEX.md` (most classic monsters → `2024 MM`; VRGtR/MToF/MotM where applicable; one `source check needed` for the unspecified deep-water aberration). Added a **Horror Expansion Supplement (Pending)** section + ~28 placeholder creatures (each "source check needed — RtHW") to `CREATURE_SOURCE_REFERENCE.md` for *Ravenloft: The Horrors Within* (RtHW, releases June 16 2026 — not yet available). **Corrected stale "no Ravenloft material" claims** in STAGE_13_PROGRESS, CONTENT_INDEX, and this log: VRGtR (2021) *is* referenced as a copyright-safe Track-A horror source (the world is original and is NOT Ravenloft; only published creature references are borrowed, never setting lore). No new factions/NPCs/regions/mysteries/gods/artifacts; no copied stat blocks; apex truth still DM-only/gated.

### Files Created
- `13_encounters_and_bestiary/README.md` (replaces `_PLACEHOLDER.md`, which was deleted)

### Files Changed
- `13_encounters_and_bestiary/BESTIARY_INDEX.md` (Track-A source shorthands; source-key note)
- `13_encounters_and_bestiary/CREATURE_SOURCE_REFERENCE.md` (expanded source key; RtHW pending section + ~28 placeholders; edition-preference rule)
- `00_control/STAGE_STATUS.md`, `00_control/STAGE_13_PROGRESS.md`, `00_control/CONSISTENCY_AUDIT.md`, `00_control/OPEN_QUESTIONS.md`, `00_control/NAMING_REGISTRY.md`, `00_control/CONTENT_INDEX.md`, `00_control/TAG_INDEX.md`, `00_control/TODO.md`, `17_generation_backlog/EXPANSION_PLAN.md`, `17_generation_backlog/CONTENT_GAPS.md`

### Indexes Updated
- CONTENT_INDEX (README row; corrected horror-file summary), TAG_INDEX (`type:encounter` list completed for all Stage 13 files), BESTIARY_INDEX (source column).

### Gaps Identified / Carried
- RtHW bestiary integration pending the June 16 2026 release (low-priority; logged in TODO/CONTENT_GAPS/OPEN_QUESTIONS).

### Next Recommended Pass
- Stage 14: Treasure, Artifacts, and Rewards.

---

## 2026-06-14 — Stage 13 Encounter and Bestiary Expansion

### Stage
Stage 13 (Encounter and Bestiary Expansion).

### Summary
Built 28 newly generated Stage 13 files in `13_encounters_and_bestiary/` (35 total .md files in the folder including README, inherited support files, and pre-existing Ring 1/Caradril encounter files): 13 cross-cutting (encounter index, bestiary index [17 creature categories], copyright-safe source reference, solo scaling rules, 15-biome matrix, 18 tiered bosses, original Remembrance horror/curse bestiary, faction encounters [all 7 majors + city + regional], mystery clue-bearing encounters, travel tables [all terrains × all 5 level-bands 1–20], dungeon support [all 36 dungeons], all-regions master) + 15 new far/mid-continent per-region encounter files. **All 20 regions, all 5 level-bands (1–20), and all 17 required creature categories are now covered.** Official monsters are source-referenced (never stat-block-copied); originals get abbreviated 5e-compatible summaries. Everything is solo-tuned (telegraph, morale, escape, non-combat outs). Horror is built from the original Remembrance cosmology (the world is original and is NOT Ravenloft); for mechanical creature references it draws on the published gothic-horror sourcebook **Van Richten's Guide to Ravenloft (VRGtR, 2021)** as a copyright-safe Track-A source (name + source + role only; no stat blocks; no imported setting lore). *(The cleanup pass above corrected an earlier inaccurate "no Ravenloft material" note in this entry.)* No new factions/NPCs/regions/mysteries/gods/artifacts; far regions corroborate (never relocate) the keystone/Court/endgame; apex truth stays DM-only and gated.

### Files Created
- 13 cross-cutting: `ENCOUNTER_INDEX.md`, `BESTIARY_INDEX.md`, `CREATURE_SOURCE_REFERENCE.md`, `SOLO_ENCOUNTER_SCALING.md`, `BIOME_ENCOUNTER_MATRIX.md`, `BOSS_AND_APEX_THREATS.md`, `HORROR_AND_CURSE_THREATS.md`, `FACTION_ENCOUNTERS.md`, `MYSTERY_ENCOUNTERS.md`, `TRAVEL_ENCOUNTERS.md`, `DUNGEON_ENCOUNTER_SUPPORT.md`, `REGIONAL_ENCOUNTER_TABLES.md`, `00_control/STAGE_13_PROGRESS.md`
- 15 per-region: `VERDANCE_REACHES`, `GLASSMERE_LEAGUE`, `MARROWDOWNS`, `SALLOWMARCH`, `HOLLOW_GULF`, `WENDER_STEPPE`, `KARRAN_MARCHES`, `EMBERFELL`, `SALTMERE_REACHES`, `CONCORD_HEARTLANDS`, `HETHEWALD`, `SUNMARK`, `HIGHMARK_PASSES`, `CINDERN_WASTE`, `DROWNED_STEPS` (`_ENCOUNTERS.md`)

### Files Changed
- `00_control/CONTENT_INDEX.md`, `00_control/TAG_INDEX.md`, `00_control/TODO.md`, `17_generation_backlog/CONTENT_GAPS.md`

### Canon Established
- No new canon facts. The bestiary formalizes existing creature ecology and the Remembrance horror cosmology into encounter-ready form. Far-region threats are echoes/mirrors; the keystone/Court/Under-Shrine remain DM-only and beneath Hollowmere.

### Indexes Updated
- CONTENT_INDEX, TAG_INDEX, ENCOUNTER_INDEX (new), BESTIARY_INDEX (new), REGIONAL_ENCOUNTER_TABLES (new).

### Gaps Identified
- No standalone NONCOMBAT_OBSTACLES library (folded into region/travel files; optional). High-tier villain *full stat blocks* live in NPC files (boss-framing provided here; deepen in Stage 15). Treasure-by-level is Stage 14.

### Next Recommended Pass
- Stage 14: Treasure, Artifacts, and Rewards — tie rewards to these encounters/bosses and the Remembrance-relic lore.

---

## 2026-06-14 — Stage 12.5 Continental Adventure-Site Coverage (interstitial)

### Stage
Stage 12.5 (Continental Adventure-Site Coverage) — interstitial pass between Stage 12 and Stage 13.

### Summary
Built 13 new far-continent adventure sites (D24–D36), bringing the campaign to **36 authored adventure sites** and giving **every map-authoritative far-continent region at least one explorable site** (Glassmere and Emberfell have two). The four previously-deferred optional sites are now built. Every far site is a surface/echo corroboration of the existing mysteries — never the keystone, the live machine, the Concord Deep, or the Hollow Court (each file carries an explicit hard-cap DM gate). No new mystery, faction, god, cosmology, artifact, NPC, or adversary proper noun was created; site names reuse already-registered Stage 9.5 far anchors/map-features (plus one new label, the Hollow Gulf Wreck-Reef). No apex truth appears in any player-safe section.

### Files Created
- `10_dungeons_and_ruins/THE_SALTMERE_DEEP_TOWNS.md` — D24, Saltmere L11-15 (drowned-town dive; pre-Concord echo; C_SR2_001)
- `10_dungeons_and_ruins/THE_HETHEWALD_OLD_HOLDS.md` — D25, Hethewald L9-13 (gated deep-wood ruin; C_HW_001)
- `10_dungeons_and_ruins/THE_MARROWDOWNS_BARROW_COMPLEX.md` — D26, Marrowdowns L8-12 (barrow-crawl; pre-Concord echo; C_MD_001)
- `10_dungeons_and_ruins/THE_KARRAN_OLD_IRON_FORTS.md` — D27, Karran L10-14 (fort+mine node; C_KM_001)
- `10_dungeons_and_ruins/THE_GLASSMERE_RELIQUARY_VAULTS.md` — D28, Glassmere L9-13 (Remnant archive-vault; C_GL_001)
- `10_dungeons_and_ruins/THE_THREE_BRIDGES_COUNTING_DEEP.md` — D29, Glassmere L9-12 (Ledger bank-heist; C_GL_002)
- `10_dungeons_and_ruins/THE_SALLOWMARCH_DROWNED_STEPS.md` — D30, Sallowmarch L10-14 (tidal causeway; pre-Concord echo; C_SM_001)
- `10_dungeons_and_ruins/THE_HOLLOW_GULF_WRECK_REEF.md` — D31, Hollow Gulf L10-15 (maritime salvage; faint echo; C_HG_001)
- `10_dungeons_and_ruins/THE_WENDER_SKY_STONES.md` — D32, Wender L8-13 (NON-Concord shrine; outside view; cosmic echo; C_WS_001)
- `10_dungeons_and_ruins/THE_SUNHOLLOW_GREAT_GROVE.md` — D33, Sunmark L8-13 (living-faith; hope/synthesis-seed; C_SMK_001)
- `10_dungeons_and_ruins/THE_NINE_LOCKS_SUNKEN_STAIR.md` — D34, Verdance Reaches L8-12 (first Ring-2 node; points home; C_VR_001)
- `10_dungeons_and_ruins/THE_HIGHMARK_FROZEN_WORKS.md` — D35, Highmark Passes L12-16 (ice-locked station; clearest far proof; C_HMP_001)
- `10_dungeons_and_ruins/THE_CINDERN_WASTE_BURIED_WORKS.md` — D36, Emberfell L13-16 (ash-drowned works; C_FC_016)

### Files Changed
- `10_dungeons_and_ruins/DUNGEON_INDEX.md` — added D24–D36 rows; updated status + all Organized Views (region/level/type/danger/REV)
- `10_dungeons_and_ruins/RUIN_INDEX.md` — added 7 ruin-type far sites; new ruin-theme notes; level_range to 16
- `10_dungeons_and_ruins/PUZZLE_DUNGEONS.md` — added 13 puzzle/investigation rows + 7 documentary-clue rows
- `10_dungeons_and_ruins/_PLACEHOLDER.md` — site count 23→36; per-region coverage table; file list
- `11_mysteries_and_secrets/CLUE_INDEX.md` — Stage 12.5 subsection (13 new far clues); per-REV three-source verification updated
- `00_control/CONTENT_INDEX.md` — 13 new dungeon rows
- `00_control/TAG_INDEX.md` — type:dungeon/type:ruin far entries; Stage 12.5 tracking line
- `00_control/NAMING_REGISTRY.md` — Stage 12.5 site-names subsection + status note
- `17_generation_backlog/CONTENT_GAPS.md` — 4 deferred sites marked done; far-dungeon gap closed
- `00_control/TODO.md` — Stage 12.5 marked done; Stage 13 flagged next
- `00_control/STAGE_STATUS.md` — Stage 12.5 interstitial row; most-recent-pass updated

### Canon Established
- No new canon facts. 13 far adventure sites added as surface/echo corroboration of existing REVs (REV_001/002/005/006/008/009/010); 13 new hidden far clue IDs. Pre-Concord echoes (Saltmere/Marrowdowns/Sallowmarch) framed as *older, separate* falls; Wender (non-Concord outside view) and Sunmark (living-faith hope) added as thematic contrasts. No new mystery/faction/god/cosmology/artifact.

### Indexes Updated
- DUNGEON_INDEX, RUIN_INDEX, PUZZLE_DUNGEONS, _PLACEHOLDER, CLUE_INDEX, CONTENT_INDEX, TAG_INDEX, NAMING_REGISTRY.

### Gaps Identified
- Remaining far-continent regions are deep-build placeholders (region/settlement gazetteers, NPC density) — site coverage is now complete; deep regional builds remain for Stage 15 / Ring 2+ as play warrants. Overseas Vael landmasses (Surren, Iron Skards, Sundered Isles) remain 1-line placeholders (far-future, not arc-required).

### Next Recommended Pass
- Stage 13: Encounter and Bestiary Expansion (fold in `STAGE_12_ADVERSARIES.md`, now serving all 36 sites; build mid/high-tier bestiary, recurring villains, noncombat obstacles, boss design).

---

## 2026-06-13 — Stage 12 Cleanup Pass

### Stage
Stage 12 (Dungeons, Ruins, Adventure Sites) — cleanup pass.

### Summary
Fixed tracking and index issues before commit. Rewrote `_PLACEHOLDER.md` as a proper folder README. Created `RUIN_INDEX.md` (ruin-type subset index). Fixed DUNGEON_INDEX "By Region" count (Reach was labelled 8; correct is 10). Corrected clue ID range in STAGE_12_PROGRESS (C_SR_039-044 → 039-041). Updated TAG_INDEX with Stage 12 dungeon/ruin/encounter/region entries. Updated current-status language in EXPANSION_PLAN, OPEN_QUESTIONS, CONSISTENCY_AUDIT, and NAMING_REGISTRY (all now reflect Stage 12 complete, Stage 13 next).

### Files Created
- `10_dungeons_and_ruins/RUIN_INDEX.md` — ruin-type subset index (11 sites)

### Files Changed
- `10_dungeons_and_ruins/_PLACEHOLDER.md` — rewritten as folder README (site counts, file list, links to indexes)
- `10_dungeons_and_ruins/DUNGEON_INDEX.md` — Reach count corrected (8→10); RUIN_INDEX.md added to Related Files
- `00_control/TAG_INDEX.md` — current status advanced to Stage 12; type:dungeon/ruin/encounter sections updated with Stage 12 files; region:sundering-reach and region:caradril updated; status:static updated
- `00_control/EXPANSION_PLAN.md` — current status + current stage table + later-expansion list updated to reflect Stage 12 done / Stage 13 next
- `00_control/OPEN_QUESTIONS.md` — current status line updated (Stages 0-11 → 0-12)
- `00_control/CONSISTENCY_AUDIT.md` — current status updated; per-clue-files item updated (post-Stage 12 → Stage 16+)
- `00_control/NAMING_REGISTRY.md` — stage count line updated (Stages 1-11 → 1-12, Stage 12 next → Stage 13 next)
- `00_control/STAGE_12_PROGRESS.md` — clue ID range corrected; RUIN_INDEX added to file list; cleanup-pass checklist item added

### Canon Established
None — cleanup pass only.

### Indexes Updated
- TAG_INDEX (type:dungeon, type:ruin, type:encounter, region:sundering-reach, region:caradril, current status)
- DUNGEON_INDEX (count fix + RUIN_INDEX link)

### Next Recommended Pass
- Stage 13 (Encounter and Bestiary Expansion)

---

## 2026-06-13 — Stage 12: Dungeons, Ruins, and Adventure Sites

### Stage
Stage 12 (Dungeons, Ruins, Adventure Sites) — complete.

### Summary
Built the campaign's adventure-site library: a master index, a puzzle/investigation index, Stage 11 clue cross-links appended to all 15 existing dungeons, 8 new adventure sites filling the level/region gaps (Caradril L6-10, Reach L3-10, the keystone approach L5-9, two far-continent high-tier sites L10-16, and the DM-only endgame L16-20), and a new abbreviated-stat-block adversary file. Every site supports multiple play styles (exploration/social/stealth/puzzle/faction/combat), is solo-tuned and retreat-rich, and has a noncombat path. The apex truth (Hollow Court, harvest mechanism, endgame choice) is confined to the single DM-only file; the keystone stays vertical-under-Hollowmere; the far ruins are surface/mirror echoes, never the live machine. No new central mystery/faction/god/cosmology/artifact.

### Files Created
- `10_dungeons_and_ruins/DUNGEON_INDEX.md` — master adventure-site index (23 sites; by region/level/faction/mystery/type/danger)
- `10_dungeons_and_ruins/PUZZLE_DUNGEONS.md` — puzzle/investigation site index (puzzle types, DCs, solutions, clue deps; the Concord Script gate)
- `10_dungeons_and_ruins/THE_SUNKEN_WARDS_DEEP.md` — Caradril undercity dungeon (L6-10; back-route to the Sealed Archive; 3-faction; C_CAR_016)
- `10_dungeons_and_ruins/THE_CARADRIL_ASHMARKET_UNDERCROFT.md` — Caradril criminal/relic warren (L6-9; trade-ledger C_CAR_017/018; refining-horror)
- `10_dungeons_and_ruins/THE_CONCORD_RELAY_VAULT.md` — Sunder Heights signal-station (L7-10; watchword-guardian; rich M9 frag C_SR_041)
- `10_dungeons_and_ruins/THE_GREYFENS_DEEP.md` — environmental fen dungeon (L3-7; Drift-Line M5 field-proof; Gravecaller cell; C_SR_040; funnels to the Barrow)
- `10_dungeons_and_ruins/THE_BASIN_KEYSTONE_APPROACH.md` — keystone surface/upper works (L5-9; M2/M4/M5 at source + M6 frag C_SR_039; deep stair = gated lethal endgame gate)
- `10_dungeons_and_ruins/THE_OLD_CONCORD_HEARTLANDS_RUIN.md` — far surface ruin / Ruin'd Crown (L10-14; REV_005/006 surface-proof C_FC_001/014; NOT the keystone/Court)
- `10_dungeons_and_ruins/THE_EMBERFELL_CALDERA_DESCENT.md` — far volcanic environmental dungeon (L12-16; harvest-mirror; far REV_002 echo C_FC_004/015)
- `10_dungeons_and_ruins/THE_UNDER_SHRINE_APPROACH.md` — **DM-ONLY endgame** (L16-20; the Drowned Keystone + Hollow Court; REV_007/008/010; the campaign decision)
- `13_encounters_and_bestiary/STAGE_12_ADVERSARIES.md` — 8 abbreviated 5e-compatible dungeon adversary profiles (incl. the DM-only Hollow Court Custodian)
- `00_control/STAGE_12_PROGRESS.md` — Stage 12 working-state tracker (complete)

### Files Changed
- All 15 existing dungeon files (`THE_PEAT_CHAPEL`, `THE_WHISPERING_CAIRN`, `THE_SUNKEN_TOLLHOUSE`, `THE_LEDGER_VAULT`, `THE_DEEP_ADIT`, `THE_BARROW_OF_NINE_DOORS`, `THE_BURIED_CLOISTER`, `THE_PELLOW_GRANGE`, `SAINT_VEDDOWS_TOMB`, `THE_GREENWARD_TOLL_STATION`, `THE_HANGING_OAKS`, `THE_OLD_MAST`, `THE_WRECKERS_CAVES`, `THE_DROWNED_LAMP`, `THE_SKERRY_SHRINE`) — appended `## Stage 11 Clue Cross-Links` + DUNGEON_INDEX link (append-only)
- `11_mysteries_and_secrets/CLUE_INDEX.md` — added the Stage 12 new-dungeon clue IDs subsection (C_SR_039-041, C_CAR_016-018, C_FC_014-015)
- `00_control/CONTENT_INDEX.md` — status line + dungeon table (master index, puzzle index, 8 new sites) + bestiary table (STAGE_12_ADVERSARIES)
- `00_control/NAMING_REGISTRY.md` — Stage 12 site-names subsection
- `00_control/STAGE_STATUS.md` — Stage 12 row -> complete; header advanced to Stage 13
- `00_control/TODO.md`, `17_generation_backlog/CONTENT_GAPS.md` — Stage 12 marked done; optional far sites logged

### Canon Established
- No new world facts. Stage 12 built explorable sites for existing canon. The Under-Shrine Approach is the first file to *render* the apex endgame site (still DM-only, consistent with DM_ONLY_CANON and the vertical-endgame map authority).

### Indexes Updated
- DUNGEON_INDEX (new), PUZZLE_DUNGEONS (new), CLUE_INDEX, CONTENT_INDEX, NAMING_REGISTRY.

### Gaps Identified
- Optional far-continent sites (Saltmere Deep Towns, Hethewald Old Holds, Marrowdowns Barrow Complex, Karran Old Iron Forts) named but not built — logged in CONTENT_GAPS for future far-play depth.
- `14_treasure_and_artifacts/` not yet built — several sites reference tier-3/4 artifact rewards "when built" (Stage 14).

### Next Recommended Pass
- Stage 13 (Encounter and Bestiary Expansion): build out `MONSTER_INDEX`, `ADVERSARY_GROUPS`, `RECURRING_VILLAINS`, `RANDOM_ENCOUNTERS`, `NONCOMBAT_OBSTACLES`, `BOSS_DESIGN`, folding in the Stage 12 adversary profiles.

---

## 2026-06-13 — Cartographic Precision Pass: Full-Continent Settlement/Social Anchors

### Stage
Interstitial cartographic pass (not a development stage). Sits between Stage 11 (complete) and Stage 12 (queued). No new canon geography.

### Summary
Resolved the "settlements bunch in the northwest" problem on full-continent maps by giving every far-continent placeholder region player-safe settlement/social map markers. Assigned full-continent 0–100 coordinates to (a) the canonical NW campaign settlements (mirrored, unchanged) and (b) the already-registered Stage 9.5 light NPC-facing anchors for all 12 placeholder regions. Coined no new proper nouns; created no new regions, factions, gods, artifacts, or central mysteries; exposed no DM-only locations.

### Files Created
- `04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md` — settlement/social-anchor render layer: 17 mirrored NW anchors (Table 1) + 36 far-continent anchors across all 12 regions (Table 2) + 5 non-rendered local anchors (Table 3); 6 anchor types; render-priority + reference/art-map flags; coordinate rules, secrecy rules, density summary, self-audit (8/8 PASS)
- `18_audits/PLAYER_SAFE_FULL_CONTINENT_MAP_AUDIT.md` — 11-check map-distribution audit (11/11 PASS; 0 Critical/High/Medium; 1 Low = no JSON manifest exists)

### Files Changed
- `04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` — added §8.5 "Settlement and Social Anchor Render Layer" (points to the anchors file as source of truth; reference vs art-map render rules; explicit no-NW-bunching rule)
- `04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` — added §D.5 settlement-anchor layer (required NW markers + far-continent anchor table + art-map subset + no-duplicate rule + NW-bunching warning) and 5 new audit checks (§K 16–20)
- `00_control/CONTENT_INDEX.md` — added the anchors file and the map audit
- `00_control/NAMING_REGISTRY.md` — Current Status note: Stage 9.5 light anchors now carry full-continent coordinates; no new names coined
- `00_control/TODO.md` — pass logged complete under Completed Recently; map-image task note updated

### Canon Established
- None. No new world content. Settlement markers are coordinate placements of already-existing, already-registered light anchors.

### Indexes Updated
- CONTENT_INDEX (anchors file + audit). NAMING_REGISTRY status note.

### Gaps Identified
- No machine-readable JSON render manifest exists (`player_safe_full_continent_render_manifest.json`); markdown is the only source. Logged as a Low finding in the map audit — optional, non-blocking.

### Next Recommended Pass
- Generate the actual full-continent map images using the now-complete anchor layer; then proceed to Stage 12 (Dungeons, Ruins, Adventure Sites).

---

## 2026-06-13 — Stage 11 Cleanup Pass

### Stage
Stage 11 — Mystery, Secret, and Clue Expansion (cleanup pass).

### Summary
Post-Stage-11 bookkeeping: updated all stale tracking/status files to reflect Stages 0–11 complete and Stage 12 next; created four DEVELOPMENT_STAGES.md required wrapper files (MYSTERY_CHAINS.md, FALSE_LEADS.md, REVEAL_TIMING.md, PROPHECIES_AND_OMENS.md); mirrored the new region-coded clue ID ranges into HIDDEN_CLUES.md Stage 11 anchor section; added the four wrapper files to CONTENT_INDEX.md and TAG_INDEX.md; updated NAMING_REGISTRY.md Current Status note.

### Files Created
- `11_mysteries_and_secrets/MYSTERY_CHAINS.md` — navigation index/wrapper for the full mystery chain infrastructure
- `11_mysteries_and_secrets/FALSE_LEADS.md` — alias/wrapper pointing to FALSE_LEADS_AND_MISDIRECTIONS.md
- `11_mysteries_and_secrets/REVEAL_TIMING.md` — phase gate quick-reference chart (REV_001–010)
- `11_mysteries_and_secrets/PROPHECIES_AND_OMENS.md` — omen delivery policy file

### Files Changed
- `00_control/CONTENT_INDEX.md` — added 4 wrapper file entries to mysteries section
- `00_control/TAG_INDEX.md` — Current Status updated; type:mystery, type:npc-codex, type:quest sections added; Stage 11 dm-only entries added
- `00_control/NAMING_REGISTRY.md` — Current Status updated to Stages 0–11 complete
- `00_control/CONTENT_GAPS.md` — Current Status updated (Stages 0–11 complete)
- `00_control/EXPANSION_PLAN.md` — Current Stage updated to Stage 12 next
- `00_control/CONSISTENCY_AUDIT.md` — Stage 11 self-check prepended
- `00_control/OPEN_QUESTIONS.md` — Status line updated to Stages 0–11 complete
- `02_runtime_state/HIDDEN_CLUES.md` — Stage 11 region-coded clue layer anchor section added

### Canon Established
- None. Cleanup pass only — no new world content created.

### Indexes Updated
- CONTENT_INDEX (4 new entries), TAG_INDEX (full Stage 11 update).

### Gaps Identified
- None new. Stage 11 gaps (mirror clue IDs) resolved in this pass.

### Next Recommended Pass
- Stage 12 — Dungeons, Ruins, and Adventure Sites.

---

## 2026-06-13 — Stage 11: Mystery, Secret, and Clue Expansion

### Stage
Stage 11 — Mystery, Secret, and Clue Expansion.

### Summary
Built the campaign's discoverability machinery on top of the existing (well-protected) Stage-1 mystery web. Added a formal revelation map (REV_001–REV_010, each with at least three independent clue sources spanning different regions, NPCs, and approaches), a region-coded clue layer, a seven-layer mystery hierarchy, six regional clue trails, faction and NPC knowledge maps, nine fair false leads, ten-playstyle discovery paths, a DM-only secret protection matrix, and a blank live-play mystery-state tracker. Cross-linked the Stage 10 major quests to revelation/clue IDs. Ran a secrecy audit (0 Critical / 0 High). Preserved all established canon (M0–M10, the harvest, the deliberate Quietfall, the Hollow Court keystone); no apex truth leaks into any player-safe file.

### Files Created
- `11_mysteries_and_secrets/by_region/SUNDERING_REACH_CLUES.md`, `CARADRIL_CLUES.md`, `ASHGARDEN_VALE_CLUES.md`, `TOLLWOOD_CLUES.md`, `PALE_COAST_CLUES.md`, `FAR_CONTINENT_ECHO_CLUES.md` — six regional clue trails
- `11_mysteries_and_secrets/by_faction/FACTION_KNOWLEDGE_MAP.md` — all 7 factions (Hollow Court section apex-DM-only)
- `11_mysteries_and_secrets/NPC_KNOWLEDGE_MAP.md` — ~60 NPCs by knowledge tier
- `11_mysteries_and_secrets/FALSE_LEADS_AND_MISDIRECTIONS.md` — 9 fair, recoverable false leads
- `11_mysteries_and_secrets/DISCOVERY_PATHS.md` — 10 playstyles + anti-railroad redirect rules
- `11_mysteries_and_secrets/SECRET_PROTECTION_MATRIX.md` — DM-only; 7 apex secrets, safe/unsafe wording + gates
- `11_mysteries_and_secrets/MYSTERY_STATE_TRACKER_TEMPLATE.md` — blank runtime tracker
- `18_audits/STAGE_11_MYSTERY_SECRECY_AUDIT.md` — secrecy audit report
- `00_control/STAGE_11_PROGRESS.md` — progress tracker

### Files Changed
- `11_mysteries_and_secrets/REVELATION_MAP.md` — formal REV_001–REV_010 layer; dependency graph; per-REV 3+ sources
- `11_mysteries_and_secrets/CLUE_INDEX.md` — region-coded clue layer + per-REV three-source verification
- `11_mysteries_and_secrets/MYSTERY_WEB.md` — 7-layer mystery hierarchy + far-continent echo cross-reference
- `11_mysteries_and_secrets/SECRET_INDEX.md` — Stage 11 REV cross-reference
- `09_quests/MAJOR_CAMPAIGN_QUESTS.md` — Clues-and-Revelations cross-link table
- `00_control/STAGE_STATUS.md`, `CONTENT_INDEX.md`, `TODO.md` — Stage 11 complete; Stage 12 flagged next

### Canon Established
- No new canon. M0–M10 and all DM-only truths preserved; the new files are discoverability/retrieval infrastructure over existing canon.

### Indexes Updated
- CLUE_INDEX, MYSTERY_WEB, REVELATION_MAP, SECRET_INDEX, CONTENT_INDEX, STAGE_STATUS.

### Gaps Identified
- (Medium) Mirror region-coded clue IDs into runtime `HIDDEN_CLUES.md` for 1:1 REV tracking (non-blocking; logged in TODO + audit).
- (Medium) Light confirming read of 11 far-quest files in Stage 12 (grep-clean; non-blocking).

### Next Recommended Pass
- Stage 12 — Dungeons, Ruins, and Adventure Sites (keystone drowned-shrine / Under-Shrine; cross-link existing dungeons to the new region-coded clue layer).

---

## 2026-06-12 — Stage 9: NPC Codex Expansion (Pass 1 + Pass 2 — Complete)

### Stage
Stage 9 — NPC Codex Expansion

### Summary
Expanded the NPC codex from the 20-major / 64-secondary / ~92-minor baseline to **50 major / ~200 secondary / ~506 minor**, meeting all Stage 9 targets. Created three missing infrastructure files (NPC_RELATIONSHIP_WEB.md, NPC_SECRET_LEDGER.md [DM-only], NPC_VOICE_GUIDE.md). Pass 1 added 12 new majors (fen-warlord Drane; 3 elevated Ring-1 Mourner anchors; 8 Caradril majors) and large secondary/minor waves. Pass 2 added 18 more majors in `STAGE_9_MAJOR_NPCS.md` (M33–M48 + M49b/M50b), filling thin Reach settlements, Caradril district gaps, third-majors for thin factions, and social/cross-pressure/moral-dilemma figures. Faction ladders complete across all 7 major factions; Hollow Court secrecy preserved throughout; no new factions, gods, mysteries, or artifacts created.

### Files Created
- `ai_solo_campaign/08_npcs/NPC_RELATIONSHIP_WEB.md` — faction/settlement clusters, leverage map, death/exposure reactions
- `ai_solo_campaign/08_npcs/NPC_SECRET_LEDGER.md` — DM-only: per-NPC secret, secrecy tier, reveal gate, mystery fed
- `ai_solo_campaign/08_npcs/NPC_VOICE_GUIDE.md` — voice handles, regional/faction speech tendencies, sample lines
- `ai_solo_campaign/08_npcs/by_region/CARADRIL_MAJOR_NPCS.md` — 8 Caradril majors (C25–C32)
- `ai_solo_campaign/08_npcs/by_region/STAGE_9_SECONDARY_NPCS.md` — ~136 new secondaries (waves 1–7)
- `ai_solo_campaign/08_npcs/by_region/STAGE_9_MINOR_NPCS.md` — ~387 new minors (waves 1–6)
- `ai_solo_campaign/08_npcs/by_region/FAR_CONTINENT_NPCS.md` — ~27 placeholder-region horizon figures
- `ai_solo_campaign/08_npcs/by_region/STAGE_9_MAJOR_NPCS.md` — 18 pass-2 majors (M33–M48 + M49b/M50b)
- `ai_solo_campaign/00_control/STAGE_9_PROGRESS.md` — Stage 9 production tracker

### Files Changed
- `ai_solo_campaign/08_npcs/MAJOR_NPCS.md` — +4 pass-1 majors (Drane; elevated Combe/Sennet/Bryd); Stage 9 secret-ref table
- `ai_solo_campaign/08_npcs/NPC_INDEX.md` — codex file map + Stage 9 tables + updated counts and links (50 major total)
- `ai_solo_campaign/00_control/NAMING_REGISTRY.md` — 21 new major NPC names registered (12 pass-1 + 9 pass-2 inc. disambiguation blocks)
- `ai_solo_campaign/00_control/CONTENT_INDEX.md` — NPC rows updated with correct counts and new files
- `ai_solo_campaign/00_control/STAGE_STATUS.md` — Stage 9 → complete 100%; Active stage → Stage 10

### Canon Established
- 50 named major NPCs, each with full profile, secret, and mechanical tier
- ~200 named secondary NPCs across all authored regions
- ~506 named minor NPCs (all settlements populated)
- NPC secret ledger: every major NPC's secret tiered and mystery-linked (DM-only)
- Voice guide: every major NPC has a voice handle and sample line

### Indexes Updated
- `08_npcs/NPC_INDEX.md` — master NPC table (50 major + file map)
- `00_control/CONTENT_INDEX.md` — all Stage 9 NPC files
- `00_control/NAMING_REGISTRY.md` — all new major NPC names

### Gaps Identified
- Relationship web covers majors + key secondaries only (by design; minors intentionally not webbed)
- Secret ledger "Stage 9 Additions" mirror table is partial (new NPCs tagged inline in profiles; full consolidation is optional pre-Stage-11 work)
- Recommend a canon-continuity audit over Stage 9 by_region/ files before Stage 10 (naming-collision sweep, secret-exposure check)

### Next Recommended Pass
Stage 10 — Quest Library Expansion (target: 25–40 main campaign quests; 75–150 developed regional/faction quests; 300–600 hooks/rumors/jobs). Optionally run a Stage 9 continuity audit first (`canon-continuity-auditor` agent).

---

## 2026-06-12 — Cartographic Consistency and Render-Control Audit Pass

### Stage
Between Stage 8 (complete) and Stage 9 (queued). Cartographic precision pass — no new canon geography.

### Summary
Audited and tightened full-continent player-safe map generation instructions across seven files. Removed contradictory inset guidance (Layer 8 renamed from "Inset Map" to "Standalone Zoom Map"; all six target files updated). Fixed Verdance river geometry (no longer implies it flows to the Calm Reach; correctly routed to the Pale Sea south of the Pale Coast). Resolved six co-located terrain/region label pairs with explicit priority and stacking rules (Wender Steppe → one label only; Hethewald/Hethewood, Sunmark/Sunmark Wilds, Sallowmarch/Sallow Marches → political first; Emberfells/Emberfell Theocracy → terrain first; Saltmere sea/Saltmere Reaches → two distinct positions). Standardized Concord Heartlands as the primary display label with optional subtitle. Promoted water.saltmere to required priority. Created a self-contained generation packet for external image models. Added generation-mode routing rule to FULL_WORLD_MAP_PROMPTS.md. No new geography, factions, secrets, or lore.

### Files Created
- `ai_solo_campaign/04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` — self-contained copy-paste prompt for external image generators (Sections A–K; derived from the render manifest)

### Files Changed
- `ai_solo_campaign/04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` — river.verdance corrected; all six terrain/region co-located pairs resolved with priority rules in §4; water.saltmere upgraded to required; region.saltmere_reaches render_as updated to text-over-terrain; Concord Heartlands display_label standardized; terrain.wender_steppe_terrain set to omit (visual fill only); §7 co-located pair table added with resolved rules
- `ai_solo_campaign/04_world_atlas/FULL_WORLD_MAP_PROMPTS.md` — generation-mode routing rule added before Prompt 1; Concord Heartlands label corrected in Prompt 1 body; both changes to Prompt 1 from the previous render-manifest pass retained
- `ai_solo_campaign/04_world_atlas/FULL_WORLD_MAP_LAYERS.md` — Layer 8 renamed to "Standalone Zoom Map"; inset-on-Prompt-1 language removed; layer-to-prompt mapping updated; clarifying note added
- `ai_solo_campaign/04_world_atlas/WORLD_MAP_PROMPTS.md` — scope note corrected (removed "embeds this map as its NW inset"; replaced with standalone zoom language)
- `ai_solo_campaign/00_control/CONTENT_INDEX.md` — FULL_WORLD_MAP_LAYERS and FULL_WORLD_MAP_PROMPTS entries corrected (inset → standalone zoom map)
- `ai_solo_campaign/00_control/RETRIEVAL_GUIDE.md` — both full-world map entries corrected (inset → standalone zoom map)
- `ai_solo_campaign/00_control/TODO.md` — map generation TODO updated to reference generation packet and standalone zoom language

### Canon Established
- No new canon. Precision and consistency pass only.

### Indexes Updated
- CONTENT_INDEX.md (entry wording)
- RETRIEVAL_GUIDE.md (entry wording)

### Gaps Identified
- None new.

### Next Recommended Pass
- Stage 9: NPC Codex Expansion.

---

## 2026-06-11 — Stage 8: Faction Deepening

### Stage
Stage 8 — Faction Deepening.

### Summary
Made all seven major factions fully operational campaign engines. Built a 4-quest chain for every faction (intro hook → trust-building → moral complication → internal-conflict decision point), added a "Combat Capability And Stat References" section with rank-and-file adversary profiles to every faction file, authored two new cross-faction files (a full pairwise relationship map including the Hollow Court's hidden ties, and between-session faction-turn rules), and wired the chains into the runtime clocks and state. The Hollow Court keeps its DM-only secrecy: no early recruit quest by design — its chain is an opposition-and-revelation arc paced to the main-arc reveal schedule. No new proper nouns, central mystery, major faction, god, cosmology, or artifact were created; all content reuses existing NPCs, clocks (#1–#10, C1–C3, regional), and mysteries (M1–M9), with reveals capped per the revelation map.

### Files Created
- `07_factions/FACTION_RELATIONSHIP_MAP.md` — full pairwise relationship map (every open-faction pair + the Court's hidden ties + blocs/triangles for faction turns)
- `07_factions/FACTION_TURN_RULES.md` — when/how the AI DM runs faction turns between sessions; clock advancement; rumor generation; state updates; solo-play guardrails; per-faction cheat-sheet
- `09_quests/faction_quests/ASHEN_WARDENS/` — `_CHAIN_INDEX.md` + QW1 The Empty Cloak, QW2 Salt and Ash, QW3 The Rite That Won't Take, QW4 The Oath and the Doubt
- `09_quests/faction_quests/CINDER_LEDGER/` — `_CHAIN_INDEX.md` + QL1 The Debt of the Drowned, QL2 The Quiet Buyer, QL3 What the Vault Remembers, QL4 The Factor's Conscience
- `09_quests/faction_quests/MOURNERS_CIRCLE/` — `_CHAIN_INDEX.md` + QM1 The Unwashed Dead, QM2 The Old Songs, QM3 The Buyer at the Graveside, QM4 Salt, Oil, and Iron
- `09_quests/faction_quests/REACHWARD_COMPACT/` — `_CHAIN_INDEX.md` + QC1 The Watch Can't Spare a Man, QC2 The Doctored Survey, QC3 The Reed Holms Eviction, QC4 The Basin Vote
- `09_quests/faction_quests/GRAVECALLERS/` — `_CHAIN_INDEX.md` + QG1 A Knock in the Dark, QG2 The Tallow Man's Word, QG3 What the Dead Want, QG4 The Breaking-Tools
- `09_quests/faction_quests/CONCORD_REMNANT/` — `_CHAIN_INDEX.md` + QR1 The Visiting Scholar's Errand, QR2 The Reader of Ruins, QR3 The Idealist and the Archivist, QR4 The Reclaimers' Gambit
- `09_quests/faction_quests/HOLLOW_COURT/` — `_CHAIN_INDEX.md` + QH1 The Hand That Moves the Vote, QH2 The Probe's Own Strings, QH3 The Court Beneath, QH4 The Fate of the Remembrance (all **DM-only**)

### Files Changed
- All 7 `07_factions/major_factions/*.md` — added "Combat Capability And Stat References" sections (rank-and-file adversary profiles + scaling) and "Faction Quest Chain (Stage 8)" cross-links
- `07_factions/FACTION_INDEX.md` — Stage 8 companion-files section; per-faction "Player can" + quest-chain columns; related-files links
- `02_runtime_state/FACTION_STATE.md` — Stage 8 note (chains/relationship-map/turn-rules wired in); related-files links
- `02_runtime_state/WORLD_CLOCKS.md` — Stage 8 faction-chain levers table (which Q*4 decision-point sets which clock); related-files links
- Tracking: `CONTENT_INDEX.md`, `TAG_INDEX.md`, `STAGE_STATUS.md`, `TODO.md`, `CONTENT_GAPS.md`, `NAMING_REGISTRY.md`, `RETRIEVAL_GUIDE.md`

### Canon Established
- No new world facts. Faction motives, relationships, and clocks unchanged from established canon — only deepened with authored quest structure and rank-and-file mechanical profiles. Hollow Court remains DM-only with no early recruit path.

### Indexes Updated
- `CONTENT_INDEX.md` (faction-quest-chains section + status), `TAG_INDEX.md` (new files + `faction-quest`/`quest-chain`/`faction-turn`/`relationships` tags), `FACTION_INDEX.md`, `STAGE_STATUS.md`, `RETRIEVAL_GUIDE.md`.

### Gaps Identified
- Ring 1 regions remain below the per-region NPC target (carried to Stage 9). Faction-quest chains reference existing named members; broadening the supporting cast is Stage 9 work.

### Next Recommended Pass
- Stage 9 — NPC Codex Expansion (broaden secondary/minor NPCs toward targets; NPC relationship web + secret ledger; Ring 1 cast).

---

## 2026-06-11 — Full-World Cartographic Expansion Pass

### Stage
Interstitial cartographic pass (not a development stage). Expands the map-authority layer from the NW campaign quarter to the **full continent of Orrun**.

### Summary
Expanded the cartographic layer from the **northwestern campaign quarter** to a **true full continent of Orrun**, without changing any world fact, contradicting any travel time, or moving the climax. Authored 4 full-continent atlas files. Decided the primary map is **all of Orrun** (Vael's other landmasses placed at placeholder level only: Surren, the Iron Skards, the Sundered Isles). Established the continent's dominant **NW (cold-poor frontier) → SE (warm-rich settled)** axis; named all major continental water, mountain ranges (incl. the continent-splitting Greatspine/Sundering Wall cordillera and a **volcanic** SE highland, the Emberfells), forests, deserts/badlands, marshes, steppe, downs, and island chains; defined **13 placeholder political/cultural regions** spanning a city-league, manorial holds, a protectorate, port city-states, a nomadic confederacy, ungoverned marches, a volcanic theocracy, salt-clan holds, a **fallen-realm Concord surface ruin**, forest free-holds, and sacred tribal land (variety over symmetry; no biome-per-direction; no all-kingdoms). Embedded the existing campaign cluster in the NW corner via a **documented coordinate rescale** (campaign grid → full-grid X 8–40, Y 8–42). Defined 8 full-world map layers (incl. a campaign-area inset) and 5 image prompts (3 player-safe, 2 DM-only). Clarified the existing `WORLD_MAP_*` files as the **campaign-area** authority. **The endgame stays vertical (beneath Hollowmere); the new far ruins are surface/pre-Concord echoes, never the keystone or the Hollow Court's seat. No new factions, gods, cosmology, central mysteries, or artifacts; placeholders are not deep-built.**

### Files Created
- `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` — full-continent master cartographic reference
- `04_world_atlas/FULL_WORLD_MAP_COORDINATES.md` — full-continent normalized 0–100 grid (124 entries; rescale documented)
- `04_world_atlas/FULL_WORLD_MAP_LAYERS.md` — 8 full-world map layers
- `04_world_atlas/FULL_WORLD_MAP_PROMPTS.md` — 5 full-world image-generation prompts

### Files Changed
- `04_world_atlas/WORLD_MAP_PROMPTS.md` — re-scoped/clarified as campaign-area (NW Orrun) prompts; cross-linked to the full-world prompts
- `04_world_atlas/REGION_INDEX.md` — added full-continent placeholder-region table
- `00_control/NAMING_REGISTRY.md` — registered all new continental/landmass geographic names
- `03_canon/CANON.md` — revision-log entry
- `03_canon/PLAYER_SAFE_CANON.md` — "The Wider Continent of Orrun" player-safe geography
- `03_canon/DM_ONLY_CANON.md` — full-world geographic DM context (far ruins ≠ keystone; reach of factions; secrecy)
- `00_control/CONTENT_INDEX.md`, `TAG_INDEX.md`, `RETRIEVAL_GUIDE.md`, `TODO.md`, `17_generation_backlog/CONTENT_GAPS.md` — indexed/registered the 4 new files and the campaign-area vs full-continent split

### Canon Established
- Orrun's full shape: large continent, NW→SE cold-to-warm axis; the campaign is its NW corner; Caradril is a frontier-edge city at continental scale.
- All major continental bodies of water, ranges, forests, badlands, wetlands, steppe, downs, and islands named and positioned.
- 13 placeholder political/cultural regions + 3 overseas Vael landmasses, all placeholder-level.
- Documented coordinate rescale embedding the campaign cluster in the full-continent NW corner.

### Indexes Updated
- CONTENT_INDEX, TAG_INDEX, RETRIEVAL_GUIDE, REGION_INDEX, NAMING_REGISTRY.

### Gaps Identified
- The 13 continental placeholder regions and 3 overseas landmasses are named/positioned but not deep-built; map images not yet generated; ~86 low-confidence full-continent coordinates pending build-time refinement. (Logged in CONTENT_GAPS/TODO.)

### Next Recommended Pass
- Generate map images (FULL_WORLD_MAP_PROMPTS Prompt 5 → Prompt 1 → Prompt 3). Continue the planned stage roadmap (Stage 8 Faction Deepening). Deep-build a continental placeholder region only when play actually approaches it. Note: the campaign-area map (Prompt 5) is a separate standalone zoom map, not an inset embedded into the player-safe full-continent map (Prompt 1) — see the 2026-06-12 cartographic consistency pass.

---

## 2026-06-11 — World Map Authority Pass (cartographic canon)

### Stage
Interstitial cartographic pass (not a development stage). Establishes the map-authority layer over the existing world.

### Summary
Authored the **master cartographic reference** for Vael/Orrun's mapped NW quarter so an AI DM (and future image-generation) can place, navigate, and draw the world without inventing geography. Recorded the spatial frame the existing travel times already imply (Hollowmere center; Vale S, Tollwood E, Coast W, Caradril SE, Sunder Heights N, Pale Sea W), added a normalized 0–100 coordinate grid (77 entries; confidence-rated), defined 7 map layers (player-safe → DM-only hidden-truth), and wrote 4 image-generation prompts (2 player-safe, 2 DM-only). Named 4 supporting geographic features (Pale Sea, Highmark Spine, Verdance Reaches, the DM-only Concord Deep) and placed map-authoritative **placeholders** for midgame (Verdance Reaches; deep Sunder Heights), late-game (Concord Deep; Highmark passes), and endgame (the Under-Shrine/Drowned Keystone — placed **vertically beneath Hollowmere**, consistent with the existing arc). **No travel times or region descriptions contradicted; no new factions, gods, cosmology, central mysteries, or artifacts.**

### Files Created
- `04_world_atlas/WORLD_MAP_AUTHORITY.md` — master cartographic reference
- `04_world_atlas/WORLD_MAP_COORDINATES.md` — normalized 0–100 grid
- `04_world_atlas/WORLD_MAP_LAYERS.md` — 7 map layers
- `04_world_atlas/WORLD_MAP_PROMPTS.md` — 4 image-generation prompts
- `04_world_atlas/REGION_INDEX.md` — region index incl. placeholders

### Files Changed
- `03_canon/CANON.md` — revision-log entry; `PLAYER_SAFE_CANON.md` — "Known Geography" section; `DM_ONLY_CANON.md` — "World Map Authority Pass (Geographic Truths)"
- `00_control/NAMING_REGISTRY.md` — registered 4 new geographic names
- `00_control/CONTENT_INDEX.md`, `TAG_INDEX.md`, `RETRIEVAL_GUIDE.md` — indexed the 5 new files
- `00_control/TODO.md`, `17_generation_backlog/CONTENT_GAPS.md` — map follow-ups/gaps

### Canon Established
- The mapped world is the NW quarter of Orrun; Hollowmere is the spatial keystone; the land drains toward the basin (player-observable; cause gated).
- New geographic names: the Pale Sea, the Highmark Spine, the Verdance Reaches, the Concord Deep (DM-only).
- The endgame is **vertical** (down through the keystone beneath Hollowmere), not a distant forbidden region.

### Indexes Updated
- CONTENT_INDEX, TAG_INDEX, RETRIEVAL_GUIDE, REGION_INDEX (new), NAMING_REGISTRY.

### Gaps Identified
- Placeholder regions (Verdance Reaches, deep Sunder Heights, Highmark passes) need deep-build before Ring 2 play.
- The map images are not yet generated (prompts are ready).
- Low-confidence grid coordinates need pinning down as those regions are built.

### Next Recommended Pass
- Generate the regional reference image (Prompt 3) first, then the player-safe world map (Prompt 1).
- When the player commits past Caradril, deep-build the Verdance Reaches (Ring 2).

---

## 2026-06-10 — Stage 7: Regional Expansion Ring 1

### Stage
Stage 7 — Regional Expansion Ring 1 (complete)

### Summary
Deep-built the three regions adjacent to the Sundering Reach so the player can travel outward in multiple directions: **Ashgarden Vale** (south — gentle farmland/shrine-towns; the region of *denial*, where the rites "always held" and now quietly fail; capped Concord shrine under the Saint Veddow's pilgrimage), **Tollwood** (east — deep old-growth forest and Concord toll-roads; a gated pre-Concord landmark-power in the deep Old Mast that the Concord built its roads *around*; bandit toll-war), and **Pale Coast** (west — fishing/salt-trade; ruined Concord lighthouses that were maritime harvest-nodes; the "drowned-tide"; Saltmargin reused as the existing gateway). Each region has an *honest window* settlement (Tilbrook / Coldhearth / Cobble Strand) that confirms the failures **radiate outward from the Reach keystone** (M5 corroboration) — the intended Ring 1 takeaway. All three regions, plus the Coast's sea-route, funnel to Caradril (the mid-game hub), with a dedicated travel-routes file. Every dungeon/encounter is solo-tuned and telegraphed; the three apex sites (Old Mast, Skerry Shrine, and the deep node-levels of Saint Veddow's Tomb / the Drowned Lamp) are explicitly gated and capped to *fragments and danger*, never the apex truth. **No new central mystery, major faction, god, cosmology, or legendary artifact was created;** new sites feed existing M2/M3/M5 (gated/oblique M6), and the Hollow Court (M7) is never named in any Ring 1 content.

### Files Created
- Regions: `05_regions/ASHGARDEN_VALE.md`, `TOLLWOOD.md`, `PALE_COAST.md`
- Settlements (8): `06_settlements/ORCHARDMERE.md`, `SAINT_VEDDOWS_REST.md`, `TILBROOK.md`, `HARTFELL.md`, `COLDHEARTH.md`, `TOLLSTONE_CROSS.md`, `WRACKMOUTH.md`, `COBBLE_STRAND.md`
- Wilderness (3): `05_regions/wilderness/ASHGARDEN_VALE_SITES.md`, `TOLLWOOD_SITES.md`, `PALE_COAST_SITES.md`
- Dungeons (9): `10_dungeons_and_ruins/SAINT_VEDDOWS_TOMB.md`, `THE_BURIED_CLOISTER.md`, `THE_PELLOW_GRANGE.md`, `THE_GREENWARD_TOLL_STATION.md`, `THE_HANGING_OAKS.md`, `THE_OLD_MAST.md` (gated), `THE_DROWNED_LAMP.md`, `THE_WRECKERS_CAVES.md`, `THE_SKERRY_SHRINE.md` (gated)
- Encounters (3): `13_encounters_and_bestiary/ASHGARDEN_VALE_ENCOUNTERS.md`, `TOLLWOOD_ENCOUNTERS.md`, `PALE_COAST_ENCOUNTERS.md`
- Hooks/Rumors (6): `09_quests/hooks_and_rumors/{ASHGARDEN_VALE,TOLLWOOD,PALE_COAST}_{HOOKS,RUMORS}.md` (66 hooks + 60 rumors)
- Developed quests (20): 8 Vale + 7 Tollwood + 5 Coast in `09_quests/regional_quests/`
- Travel: `04_world_atlas/TRAVEL_ROUTES_RING1.md` (6 routes)

### Files Changed
- `08_npcs/SECONDARY_NPCS.md` (+20 Ring 1 secondary NPCs + combat-reference rows + metadata), `MINOR_NPCS.md` (+20 Ring 1 minor NPCs + metadata), `NPC_INDEX.md` (Ring 1 secondary table + minor count)
- `03_canon/CANON.md` (geography + revision-log entry), `PLAYER_SAFE_CANON.md` (Ring 1 player-safe facts)
- `00_control/NAMING_REGISTRY.md` (Ring 1 places, NPCs, the Tollmen, terms, disambiguation notes), `CONTENT_INDEX.md`, `TAG_INDEX.md`, `RETRIEVAL_GUIDE.md`, `STAGE_STATUS.md`, `STAGE_7_PROGRESS.md`
- `17_generation_backlog/CONTENT_GAPS.md`, `EXPANSION_PLAN.md`, `TODO.md`, `CONSISTENCY_AUDIT.md`

### Canon Established
- Ring 1 geography (3 regions, 8 settlements, sites, dungeons, travel routes) registered; 1 minor regional faction (the Tollmen); 3 regional clocks; new setting terms (saint's relics, the forest-rules/the bargain, the grey lords, the salt-and-tide rite, sea-relics, the drowned-tide).
- DM-only: the Vale's Saint Veddow's and the Coast's lighthouses are harvest *cousin-nodes*; the Tollwood's Old Mast is a *gated pre-Concord landmark-power* (not the Court/a god) — all corroborate M2/M3/M5 obliquely from outside the Reach, never the apex.

### Indexes Updated
NAMING_REGISTRY, CONTENT_INDEX, TAG_INDEX, RETRIEVAL_GUIDE, NPC_INDEX.

### Gaps Identified
- Ring 1 has no standalone bestiary entries yet (encounter tables use stat-references; full bestiary = Stage 13).
- Ring 1 faction-deepening (regional faction clocks formalized in `WORLD_CLOCKS.md`/`FACTION_STATE.md`) belongs to Stage 8 and live-state seeding.
- Treasure/rewards are described inline; level-banded reward tables = Stage 14.

### Next Recommended Pass
Stage 8 (Faction Deepening): formalize the three regional clocks and the Tollmen into `WORLD_CLOCKS.md`/`FACTION_STATE.md`, and extend the major factions' Ring 1 presence (Ledger Vale/Coast arms, the Mourner folk-truth network, the Gravecaller wood/cove currents) with full clocks and quest chains.

---

## 2026-06-10 — Stage 6: First Full Audit (Stages 1–5 AI-Readiness)

### Stage
Stage 6 — First Full Audit (complete)

### Summary
Ran the first full AI-readiness and continuity audit of "The Long Remembering" across all ten `AUDIT_STANDARDS.md` categories (canon consistency, secret separation, retrieval quality, NPC connectivity, quest usability, mystery solvability, faction agency, solo-play safety, state tracking, index completeness), spanning Stages 1–5. **Foundation verified sound: 0 Critical, 1 High, 4 Medium, 5 Low.** The single High finding was a broken-link defect — the Act 1 arc spine (`ACT_1_LEVELS_1_4.md`) cross-referenced two quest files that do not exist on disk (a phantom Sashe/fens quest and a phantom Hollow Court quest); both were repaired inline (Door 4 repointed to Hook 6 + the existing `Q_SASHES_WARNING.md`; Door 7 repointed to Hook 4 in `HOOKS_TABLE.md` with an explicit "no Act 1 quest by design" note, consistent with every other file). All four Medium findings (Caradril NPC density below target, no standalone bestiary, no treasure-by-level, no Acts 2–5 arc files) are expected forward-stage gaps already tracked for Stages 9/13/14/15. Secret separation is exemplary — the apex secret (Hollow Court / M7) is never named in any Act 1 or player-facing content, the R1 reveal cap is enforced in every Act 1 file, and player-safe vs. DM-only is cleanly segregated throughout. The three-clue rule is satisfied with margin (every mystery 3–4 routes; R1 reachable 4 ways). Solo-play safety (telegraphing, noncombat outs, retreat, no cheap death, failure-redirects) is a clear strength. State tracking carries per-quest update instructions. Indexes are current and the quest-file glob matches the index listings exactly. **Outward scaling to Stage 7 approved.**

### Files Created
- `18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md` — formal audit report (scope, summary, severity tables, orphaned content, exposed secrets, solo-play/mystery risk sections, recommended fix order)

### Files Changed
- `12_campaign_arc/ACT_1_LEVELS_1_4.md` — fixed two broken quest-file cross-references (the High finding)
- `00_control/CONSISTENCY_AUDIT.md` — status updated to Stages 0–6 complete; audit-pending items closed; current Medium/Low issue list refreshed; High finding + audit logged in Resolved Issues
- `00_control/TODO.md` — Stage 6 marked complete; Stage 7 promoted to High; bestiary/treasure/Acts 2–5 added as Medium
- `17_generation_backlog/CONTENT_GAPS.md` — audit gap closed; status header updated to Stage 6 complete
- `00_control/STAGE_STATUS.md` — Stage 6 → complete (100%); active stage → Stage 7
- `17_generation_backlog/EXPANSION_PLAN.md` — current stage advanced to Stage 7; Pass 3 marked done
- `00_control/STAGE_6_PROGRESS.md` — all audit categories checked off; severity counts and findings filled in

### Canon Established
- None — audit pass; no new world facts created. One broken cross-link repaired.

### Indexes Updated
- None required (no new content files beyond the audit report, which is a tracking artifact).

### Gaps Identified
- High (fixed): broken Act 1 arc-spine quest pointers.
- Medium (tracked): Caradril NPC density (Stage 9), standalone bestiary (Stage 13), treasure-by-level (Stage 14), Acts 2–5 arc files (Stage 15).
- Low (tracked): per-clue files, random tables, NPC relationship/secret/voice tools, QUEST_INDEX.

### Next Recommended Pass
- Stage 7 — Regional Expansion Ring 1 (`world-atlas-builder`): build the Ashgarden Vale, Tollwood, and Pale Coast so the world opens outward.

---

## 2026-06-10 — Stage 5: Level 1–4 Play Arc (Act 1)

### Stage
Stage 5 — Level 1–4 Play Arc (complete)

### Summary
Built the open-world **Level 1–4 play kit** for "The Long Remembering" — an Act 1 toolkit (not a railroad) that lets an AI DM run levels 1–4 across many possible early paths atop the deep-built Sundering Reach. The kit reuses existing mysteries (M1–M9), existing major/secondary NPCs, existing factions and clocks, and existing dungeons; it created **no new central mystery, faction, god, cosmology, or artifact**, and caps every Act 1 reveal at **R1** (the failures have a source and a pattern, centered on the basin) per `REVELATION_MAP.md`. Completing work begun earlier in the stage (the arc spine `ACT_1_LEVELS_1_4.md` and the six `act_1_quests/` faction-alignment quests already existed), this pass added the five remaining pillars: (1) `ACT_1_THREATS.md` — five recurring early-threat profiles (Restless Remembrance, Wrathful Remembrance, Frontier Toughs, the Cult Radical's Hand/Cole Ashby, Rival Salvage Crews) with full D&D 5e/2024-compatible adversary profiles, solo-safe design (telegraph + morale + escape + a noncombat out for each), faction links kept DM-only, and scaling; (2) `ACT_1_CLUE_TRAILS.md` — a DM-only overlay mapping which existing clues a L1–4 player reaches, with 3–4 independent routes to R1 (personal/wilderness/political/exploration), per-mystery Act 1 ceilings, and the three-clue check, inventing no new clues; (3) `ACT_1_FAILURE_STATES.md` — nine failure cases (unresolved opening crisis, dead/lost patron, burned faction bridge, imprisonment, fleeing town, failed-dungeon retreat, antagonizing authorities, caught with the Gravecallers, lost opening clue), each redirecting play with immediate consequence + path forward + clocks advanced + NPC reactions, never ending the campaign; (4) `ACT_1_MILESTONES.md` — explicit L2/L3/L4 and L4→5 triggers earnable by multiple paths (combat never required) plus optional XP-style parity guidance, narrative unlocks, and faction-notice-by-level; (5) `ACT_1_NPC_GUIDE.md` — a casting guide pointing to existing NPCs as Act 1 allies/patrons/rivals/witnesses/complications with entry conditions and Safe Re-Entry Points for a lost player, creating no new NPCs. The Hollow Court correctly has no friendly faction quest (it is the apex villain); Reke appears only as a reasonable politician steering the player via Hook 4, never exposed. Runtime ACTIVE_QUESTS and OPEN_THREADS seeded with Act 1 quests/threads marked available/pre-play. Anti-railroad verified: the DM can run L1–4 with no fixed quest order; 4+ prepared routes beyond the default; every important conclusion has 3+ clue paths; ignoring the obvious hook still reaches prepared content; social/stealth/exploration/research/faction/dungeon/combat all supported; no single NPC/clue/dungeon/quest is mandatory; all L1–4 content is mechanically complete with no TBD stats.

### Files Created
- `12_campaign_arc/ACT_1_FAILURE_STATES.md`
- `12_campaign_arc/ACT_1_MILESTONES.md`
- `13_encounters_and_bestiary/ACT_1_THREATS.md`
- `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md`
- `08_npcs/ACT_1_NPC_GUIDE.md`
- (earlier in Stage 5) `12_campaign_arc/ACT_1_LEVELS_1_4.md`; `09_quests/act_1_quests/` (6 faction quests)

### Files Changed
- `02_runtime_state/ACTIVE_QUESTS.md` — Act 1 faction + regional quests added as available/pre-play
- `02_runtime_state/OPEN_THREADS.md` — Act 1 faction-doors + geography-of-failure threads added (pre-play)
- `00_control/CONTENT_INDEX.md`, `TAG_INDEX.md`, `RETRIEVAL_GUIDE.md` — all 5 new files + 6 quests indexed; `act:1` tag; Stage 5 load entries; status advanced to Stage 5 complete
- `00_control/NAMING_REGISTRY.md` — Stage 5 note: no new proper nouns
- `03_canon/CANON.md` (revision log) + `PLAYER_SAFE_CANON.md` (player-safe Act 1 arc facts)
- `00_control/STAGE_STATUS.md`, `TODO.md`, `CONSISTENCY_AUDIT.md`, `17_generation_backlog/CONTENT_GAPS.md`, `EXPANSION_PLAN.md` — tracking advanced to Stage 5 complete; correspondent-thread TODO noted as Act 2/Stage 15
- `00_control/STAGE_5_PROGRESS.md` — checkboxes completed; final state

### Canon Established
- No new world facts. Durable additions are *structural/play-layer only*: the Act 1 arc shape (Five Doors + faction doors), the L1–4 milestone triggers, the Act 1 failure-redirect playbook, the five recurring Act 1 threat profiles, and the R1 clue-access overlay. All consistent with Stages 1–4; recorded as a Stage 5 revision-log line in `CANON.md`. Player-safe arc facts (what the world looks like at campaign start) added to `PLAYER_SAFE_CANON.md`.

### Indexes Updated
- `CONTENT_INDEX.md` (arc, quest, mystery, encounter, NPC tables), `TAG_INDEX.md` (type tags + new `act:1` block + level:1-4 + region:sundering-reach), `RETRIEVAL_GUIDE.md` (Stage 5 Act 1 load entries)

### Gaps Identified
- The "Magisterium correspondent" thread (Reke ↔ a Caradril magister) remains an intentional open lead for Act 2 / Stage 15 (must not pre-reveal the Court).
- Act 1 dungeon-reward items and `REWARDS_BY_LEVEL.md` still pending (Stage 14); the keystone drowned-shrine dungeon still deferred (Stage 12). Neither blocks Act 1 play.

### Next Recommended Pass
- **Stage 6 — First Full Audit** over Stages 1–5 (canon consistency, secret separation, R1 gating in Act 1 content, three-clue solvability, solo-play safety, state tracking, index completeness). Do not scale outward (Stage 7+) until the audit clears.

---

## 2026-06-10 — Stage 4: First Major City Deep Build (Caradril)

### Stage
Stage 4 — First Major City Deep Build (complete)

### Summary
Built **Caradril**, the first major city, as a dense, politically alive mid-game hub (~levels 5–12, with level 3–5 on-ramps and level 12+ endgame threads), without inventing any new central mystery, faction, god, cosmology, or artifact. Caradril is an independent inland city-state on the Verdance/Stillwater, ~10–12 days SE of Hollowmere — the headquarters of the Cinder Ledger (the Ledger Keep) and the seat of the Concord Remnant (the Lamplighters' Hall + the Sealed Archive), governed by the Tidewater Council of merchant magisters (the Charter Houses) under First Magister Halloran Voss and policed by the Tide-Watch. Created a full city overview and 8 district files — the Magisterium (government/charter politics), the Counting-Quays (Ledger HQ; the Vyre–Quorrin deal), the Lantern Reach (scholars; the Concord Script gate; the Sealed Archive holding the clearest M6/M9 proof), the Ashmarket (relic black market; quiet-coin M3), Highmourn (temples/cemetery; the raise-dead cover-up; a city solo-safety hub), the Crucible (foundries; relic-smelting M3), the Sill (poor undercity; the Hush; thin-born refugees; the Sealgate), and the Sunken Wards (a flooded sub-dungeon, a *minor dormant cousin* of the Reach nodes, NOT the keystone, levels 6–14). Added 15 city secondary NPCs (Voss, Sefa Dann, Esren Tolm, Yorell Kade, Anneth Vell, Coll Riis, Tamsin Orr, Wessel Dree, Mother Ysarra, Lon Quayle, Beck Harrow, "Tidewife" Sorrel, the Bellman, Renna Sill, Old Pater Dunk) with full Tier-2 profiles and DM secrets separated from player-safe roles, plus 25 city minor NPCs by district. Authored 11 developed city quests in full QUEST_STANDARDS form (Sealed Letter, Open Charter, Quay Charter, Lantern and the Lamp, Sealed Archive, Quiet Coin, Funeral That Wouldn't Take, Smelting, Bellman's Price, Below the Stilling, Tide Turns), 36 city hooks and 30 city rumors all pointing to authored content, and a city encounter/social-scene table (8 district tables + a Sunken Wards dungeon table), social-default and stat-referenced. Established 4 city-internal factions (Tidewater Council/Charter Houses, Tide-Watch, Salt Syndicate, the Hush) and 3 city faction clocks (C1 The Deal Closes, C2 The Council Sleeps, C3 The City's Denial Cracks) anchored to the existing master clocks. Anchored existing M2/M3/M4/M6/M8/M9 clue paths to city access points (the Sealed Archive as the clearest M6/M9 cache; quiet-coin/smelting/deep-vault/Wards as M3; the charter-registry as a city M4 echo; the Magisterium correspondent as an M8 *lead, never a named second agent*; Highmourn/Sill as city M1/M5/M10 echoes). Solo play preserved throughout: Caradril is a safe-rest hub where danger is social, political, and underground; combat is concentrated in the Sunken Wards (retreat-rich, parley-able) and telegraphed faction reprisals; the city's deepest truths are Act-3 / level-9–12 gated; **the Hollow Court (M7) is never named in Caradril**; the "Stilling = harvest's pause" theme is a late, earned key. Player-safe vs. DM-only strictly separated in every file.

### Files Created
- City overview (1): `06_settlements/CARADRIL.md`
- Districts (8): `06_settlements/caradril_districts/THE_MAGISTERIUM.md`, `THE_COUNTING_QUAYS.md`, `THE_LANTERN_REACH.md`, `THE_ASHMARKET.md`, `HIGHMOURN.md`, `THE_CRUCIBLE.md`, `THE_SILL.md`, `THE_SUNKEN_WARDS.md`
- City quests (11): `09_quests/city_quests/Q_THE_SEALED_LETTER.md`, `Q_THE_OPEN_CHARTER.md`, `Q_THE_QUAY_CHARTER.md`, `Q_THE_LANTERN_AND_THE_LAMP.md`, `Q_THE_SEALED_ARCHIVE.md`, `Q_QUIET_COIN.md`, `Q_THE_FUNERAL_THAT_WOULDNT_TAKE.md`, `Q_THE_SMELTING.md`, `Q_THE_BELLMANS_PRICE.md`, `Q_BELOW_THE_STILLING.md`, `Q_THE_TIDE_TURNS.md`
- Hooks/Rumors (2): `09_quests/hooks_and_rumors/CARADRIL_HOOKS.md`, `CARADRIL_RUMORS.md`
- Encounters (1): `13_encounters_and_bestiary/CARADRIL_ENCOUNTERS.md`

### Files Changed
- `08_npcs/SECONDARY_NPCS.md` — 15 Caradril city NPCs + combat-relevance rows + metadata
- `08_npcs/MINOR_NPCS.md` — 25 Caradril minor NPCs by district + metadata
- `08_npcs/NPC_INDEX.md` — Caradril secondary table + minor count
- `00_control/NAMING_REGISTRY.md` — all new Caradril place, faction, NPC, and term proper nouns registered
- `00_control/CONTENT_INDEX.md`, `TAG_INDEX.md`, `RETRIEVAL_GUIDE.md` — all new files indexed; Stage 4 status; region:caradril block; load entries
- `03_canon/CANON.md` (geography + revision log), `PLAYER_SAFE_CANON.md` (Caradril facts), `DM_ONLY_CANON.md` (Stage 4 city DM context)
- `04_world_atlas/WORLD_OVERVIEW.md` — Caradril marked deep-built
- `07_factions/FACTION_INDEX.md` — 4 city factions + city relationships; `CINDER_LEDGER.md` & `CONCORD_REMNANT.md` — Caradril HQ/seat cross-links
- `11_mysteries_and_secrets/MYSTERY_WEB.md`, `CLUE_INDEX.md`; `02_runtime_state/HIDDEN_CLUES.md` — Caradril city clue access (extends M2/M3/M4/M6/M8/M9; no new mysteries)
- `02_runtime_state/WORLD_CLOCKS.md`, `FACTION_STATE.md` — 3 city clocks + 4 city factions
- `00_control/STAGE_STATUS.md`, `TODO.md`, `CONSISTENCY_AUDIT.md`, `17_generation_backlog/CONTENT_GAPS.md`, `EXPANSION_PLAN.md` — tracking advanced to Stage 4 complete

### Canon Established
- Caradril as the first major city: its geography (Verdance/Stillwater), the Tidewater Council/Charter Houses/Tide-Watch government, the "Stilling," 8 districts, the Ledger HQ + Remnant seat, the Sunken Wards as a *minor dormant cousin* of the Reach nodes (player-safe city facts). DM-only: the Vyre–Quorrin deal is negotiated in the city, the Sealed Archive holds the clearest M6/M9 proof, the Stilling prosperity is the harvest's pause, and the Magisterium correspondent thread (a lead, never a named second agent). New terms: Charter, the Stilling, quiet-coin.

### Indexes Updated
- CONTENT_INDEX, TAG_INDEX, RETRIEVAL_GUIDE, NPC_INDEX, FACTION_INDEX, NAMING_REGISTRY, CLUE_INDEX, MYSTERY_WEB.

### Gaps Identified
- Caradril combat-relevant NPC stat profiles are abbreviated/reference-style (sufficient for play; full custom stat blocks deferred to Stage 13 as with the Reach). The Sealed Archive and Sunken Wards are richly specced as district/quest content but a full dungeon-file build (room-by-room) is deferred to Stage 12 by design (mirrors the keystone shrine deferral). The "Magisterium correspondent" is intentionally an open thread for Stage 5/15 to resolve in play.

### Next Recommended Pass
- **Stage 5 — Level 1–4 Play Arc** (shape Act 1 atop the deep Reach), then **Stage 6 — First Full Audit** across Stages 1–5 (now including Caradril).

---

## 2026-06-09 — Stage 3: Starting Region Deep Build

### Stage
Stage 3 — Starting Region Deep Build (complete)

### Summary
Expanded the Sundering Reach from a frame into a full open-world solo sandbox supporting 10–20 sessions of play, without inventing any new central mystery, faction, god, cosmology, or legendary artifact. Added 7 new settlements (8 total) anchored to the existing map (Kettle Bridge E, Saltmargin W, Candlewick S, Greywater Holm SE, Harrowgast N, Reedford central ford, The Ashwalk Rest crossroads sanctuary), each in full settlement-standard form with leadership, NPCs, services, tensions, secrets, rumors, hooks, law/threat mechanics, and ignore-consequences. Created 4 wilderness zone-files (~25 named sites) for the Greyfens, Sunder Heights, Mirewend/Concord roads, and the basin shore, each with hazards/DCs, stat-referenced adversaries, level range, solo danger, clues, and ignore-consequences. Built 6 dungeons/ruins in full dungeon-standard (Peat Chapel = intended first delve; Sunken Tollhouse; Whispering Cairn = Concord Script gate; Ledger Vault = social/stealth heist; Barrow of Nine Doors = parley-boss; Deep Adit = secondary harvest node) with encounter lists, trap/puzzle DCs, boss mechanics with non-combat win conditions, retreat options, treasure, and scaling. Wrote ~21 secondary NPCs (including all five Stage-1-registered placeholders: Warden Pell, Tallytooth Ren, Bann Oester, Pevin Oss, Custodian Orre) and ~35 minor NPCs by location, all with combat-relevance fallbacks and DM-only secrets separated from player-safe roles. Authored 12 developed quests in full QUEST_STANDARDS form (level range, DC bands, combat + noncombat options, rest/time pressure, rewards, failure states, scaling, state-update triggers), 29 more hooks (39 total) and 30 more rumors (50 total) all pointing to authored content, and 4 solo-tuned zone encounter tables with D&D-compatible stat references. Anchored the existing M1–M9 clue paths and the 5+ relevant faction clocks to concrete new sites (no new mysteries/clocks created). Solo play preserved throughout: every dangerous encounter telegraphed, non-combat alternatives present, retreat available, the deep basin/under-shrine explicitly gated as endgame-tier, a custom reversible thin-touch mechanic instead of cheap death, and the Ashwalk Rest + Old Sashe + Candlewick chapel as solo-safety pillars. Player-safe vs. DM-only strictly separated in every file.

### Files Created
- Settlements (7): `06_settlements/KETTLE_BRIDGE.md`, `SALTMARGIN.md`, `CANDLEWICK.md`, `GREYWATER_HOLM.md`, `HARROWGAST.md`, `REEDFORD.md`, `THE_ASHWALK_REST.md`
- Wilderness (4): `05_regions/wilderness/GREYFENS_SITES.md`, `SUNDER_HEIGHTS_SITES.md`, `MIREWEND_AND_ROADS_SITES.md`, `BASIN_SHORE_AND_HOLMS_SITES.md`
- Dungeons/ruins (6): `10_dungeons_and_ruins/THE_PEAT_CHAPEL.md`, `THE_SUNKEN_TOLLHOUSE.md`, `THE_WHISPERING_CAIRN.md`, `THE_LEDGER_VAULT.md`, `THE_BARROW_OF_NINE_DOORS.md`, `THE_DEEP_ADIT.md`
- NPCs (2): `08_npcs/SECONDARY_NPCS.md`, `08_npcs/MINOR_NPCS.md`
- Quests (14): `09_quests/regional_quests/Q_*.md` (Salt Run, Broken Arch, Light on the Scale, Holm That Won't Bury Its Dead, Sold Stone, Race North, Bailiff's Ladder, Reed Holms, Sashe's Warning, Grey Woman at the Ford, Second Mark, Pell's Doubt, Scholar's Request, Failing Funeral)
- Hooks/Rumors (2): `09_quests/hooks_and_rumors/SUNDERING_REACH_HOOKS.md`, `SUNDERING_REACH_RUMORS.md`
- Encounters (1): `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md`

### Files Changed
- `05_regions/SUNDERING_REACH.md` — settlements/wilderness/dungeons/quests sections rewritten; Level Range & Solo Danger and Encounter & Hazard Mechanics sections added; related-files expanded
- `08_npcs/NPC_INDEX.md` — secondary + minor NPC sections populated
- `00_control/NAMING_REGISTRY.md` — all new place, NPC, and term proper nouns registered
- `00_control/CONTENT_INDEX.md`, `TAG_INDEX.md` — all new files indexed; Stage 3 status lines; new wilderness/encounter sections + tags
- `03_canon/CANON.md` — settlements added to geography; revision-log entry
- `03_canon/PLAYER_SAFE_CANON.md` — known towns/landmarks of the Reach
- `03_canon/DM_ONLY_CANON.md` — Stage 3 region context (conduits, minor/secondary nodes, thin-touch, geography of failure) — extends, never contradicts, the core secret
- `11_mysteries_and_secrets/CLUE_INDEX.md`, `02_runtime_state/HIDDEN_CLUES.md` — Stage 3 clue access anchors
- `02_runtime_state/WORLD_CLOCKS.md` — region anchors for the 10 clocks
- `00_control/STAGE_STATUS.md`, `TODO.md`, `CONSISTENCY_AUDIT.md`, `17_generation_backlog/CONTENT_GAPS.md`, `EXPANSION_PLAN.md` — tracking advanced to Stage 3 complete

### Canon Established
- Eight Reach settlements and their relations (player-safe); the Concord roads/Star-Stones as the harvest network and minor/secondary nodes (DM-only, consistent with the keystone being central not unique); the reversible **thin-touch** custom mechanic; the geography of rite-failure (worse near the basin) as M5 field-proof.

### Indexes Updated
- `NAMING_REGISTRY.md`, `CONTENT_INDEX.md`, `TAG_INDEX.md`, `NPC_INDEX.md`, `CLUE_INDEX.md`.

### Runtime State Updated
- `HIDDEN_CLUES.md` (region anchors; all still hidden), `WORLD_CLOCKS.md` (region anchors; positions unchanged). No live-play state changed (play has not begun).

### Gaps Identified
- The keystone drowned-shrine dungeon remains for Stage 12 (intentionally deferred).
- Treasure-by-level and the magic items referenced in dungeon rewards (e.g. the Barrow item) await Stage 14 (`REWARDS_BY_LEVEL.md`).
- Random tables (`/15_random_tables/`) still pending (Stage 3+ low priority; encounter tables now cover most travel needs).
- No formal audit yet (Stage 6).

### Next Recommended Pass
- Stage 4 (First Major City — Caradril) or Stage 5 (Level 1–4 Play Arc). Per `EXPANSION_PLAN.md`, Stage 5 (Act 1 arc + first major dungeon) is the higher-value next pass now that the region is deep; Stage 6 audit should follow Stages 4–5.

---

## 2026-06-09 — Stage 2: Cleanup Pass (Tracking Fixes + Index Gaps)

### Stage
Stage 2 — AI Runtime Foundation (post-completion cleanup; no new world content)

### Summary
Fixed stale tracking files that lagged behind the actual Stage 1–2 content and filled two known index gaps before committing Stage 2 as complete. No new world lore, NPCs, places, secrets, or plot were created. Rewrote `CONTENT_GAPS.md` (was claiming no regions/settlements/factions/NPCs/quests/arc existed) to reflect Stages 0–2 complete and the real Stage 3+ gaps by category and severity. Rewrote `EXPANSION_PLAN.md` (was Stage 0 complete / Stage 1 not started) to mark Stages 0–2 complete, Stage 3 next, with the next five production passes laid out. Rewrote `CONSISTENCY_AUDIT.md` current status (was "no campaign content exists") and logged current issues with severity plus a Resolved section for the items fixed this pass. Populated `CLUE_INDEX.md` from the authored mystery web — every clue path extracted, given a clue ID, mystery, discovery method, and status (all hidden), with a three-clue-rule check table. Seeded `02_runtime_state/HIDDEN_CLUES.md` with the same clues as undiscovered at campaign start (location + discovery trigger + act gate); left `KNOWN_CLUES.md` empty by design. Applied `DND_MECHANICS_REQUIREMENTS.md` to the five content-standards templates: added field-level mechanical requirements to `NPC_STANDARDS.md`, `QUEST_STANDARDS.md`, `CONTENT_STANDARDS.md`, `FACTION_STANDARDS.md`, and `WORLDBUILDING_STANDARDS.md`, clearing the long-standing Critical TODO (real changes were made).

### Files Created
- None.

### Files Changed
- `17_generation_backlog/CONTENT_GAPS.md` — full rewrite to reflect Stages 0–2 complete; real gaps by category/severity
- `17_generation_backlog/EXPANSION_PLAN.md` — full rewrite; Stages 0–2 complete, Stage 3 next, next 5 passes
- `00_control/CONSISTENCY_AUDIT.md` — current status + issue list rewritten; Resolved section added
- `11_mysteries_and_secrets/CLUE_INDEX.md` — populated with all authored clues (IDs, method, status=hidden) + three-clue check
- `02_runtime_state/HIDDEN_CLUES.md` — seeded with all undiscovered clues at campaign start
- `00_control/NPC_STANDARDS.md` — Mechanical Requirements section + mechanical fields in Major/Secondary/Minor templates
- `00_control/QUEST_STANDARDS.md` — Mechanical Requirements section + DC/danger/rest/reward/scaling fields in template
- `00_control/CONTENT_STANDARDS.md` — Mechanical Completeness Rule (per-type field table)
- `00_control/FACTION_STANDARDS.md` — Mechanical Requirements section + Combat Capability field in template
- `00_control/WORLDBUILDING_STANDARDS.md` — Mechanical Requirements section + level/danger/hazard fields in region/settlement/wilderness templates
- `00_control/TODO.md` — Critical task cleared to Completed; CLUE_INDEX follow-up updated
- `00_control/STAGE_STATUS.md` — Stage 2 row notes the cleanup pass
- `00_control/CONTENT_INDEX.md` — CLUE_INDEX / HIDDEN_CLUES statuses updated (placeholder → populated/seeded)
- `00_control/TAG_INDEX.md` — CLUE_INDEX moved out of status:placeholder; status line updated

### Canon Established
- None. No new world facts; tracking, runtime clue-state, and standards templates only.

### Player-Safe Facts Added
- None.

### DM-Only Facts Added
- None new. Existing authored clues were indexed/mirrored into DM-only files; no new secrets.

### Runtime State Updated
- `02_runtime_state/HIDDEN_CLUES.md` seeded (all clues hidden at campaign start). `KNOWN_CLUES.md` intentionally left empty.

### Indexes Updated
- `CONTENT_INDEX.md`, `TAG_INDEX.md`, `CLUE_INDEX.md`.

### Gaps Identified
- No formal AI-readiness audit yet (Stage 6) — tracking is self-reported.
- Per-clue files remain optional/deferred (Stage 11).
- Secondary/minor NPCs referenced in faction files still need entries (Stage 3/9).

### Next Recommended Pass
- Begin Stage 3: Starting Region Deep Build (per `EXPANSION_PLAN.md` Pass 1).

---

## 2026-06-09 — Stage 2: AI Runtime Foundation

### Stage
Stage 2 — AI Runtime Foundation (complete)

### Summary
Made the Stage 1 campaign foundation runnable by a future AI DM. No new world content was created; all material was drawn from existing Stage 1 files. Converted all 17 runner-protocol placeholder files in `01_runner_protocol/` into full operational content a future AI DM can follow directly (solo play, session loop, scene framing, player choice, rolls, combat, social, exploration, travel, downtime, clue delivery, secret reveal, failure, tone/narration, when to ask, when to improvise, session end). Wrote the two session-launch prompts (START/RESUME) as complete, self-contained, DM-only procedures, and finalized the three session-pack templates (state update, compact context, DM hidden recap) from placeholder to ready. Seeded eight runtime state files from Stage 1 content (current state, current location, current scene, active quests, open threads, faction state, next session start, plus the player-character scaffold with opening condition notes). Protocols are solo-first throughout, enforce the three-clue rule, protect hidden truths (the harvest, the Hollow Court, the steering), and reflect the locked folk-horror/frontier-grief/slow-dread tone. Start and resume prompts are DM-only and contain no player-facing spoilers.

### Files Created
- None (all target files already existed as Stage 0 placeholders; this pass populated them).

### Files Changed
- `01_runner_protocol/SOLO_PLAY_PRINCIPLES.md` — full solo-play doctrine, scaling, companions, solo-safe failure
- `01_runner_protocol/SESSION_LOOP.md` — start/during/end loop tied to runtime state filenames
- `01_runner_protocol/SCENE_FRAMING.md` — Sense/Situation/Pressure framing and transitions
- `01_runner_protocol/PLAYER_CHOICE_PROTOCOL.md` — choice-through-fiction, anti-railroad, third options
- `01_runner_protocol/ROLL_AND_CHECK_PROTOCOL.md` — three roll conditions, DC scale, success-with-cost
- `01_runner_protocol/COMBAT_PROTOCOL.md` — solo combat, telegraphing, morale, retreat, cheap-death prevention
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md` — NPC voice, attitude, lies, secret-gating
- `01_runner_protocol/EXPLORATION_PROTOCOL.md` — search resolution, environmental clues, telegraphed traps
- `01_runner_protocol/TRAVEL_PROTOCOL.md` — purposeful travel, route gates, clocks-on-time-pass
- `01_runner_protocol/DOWNTIME_PROTOCOL.md` — downtime activities, clock advancement, meaningful rest
- `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md` — three-clue rule enforced, missed-clue procedure
- `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md` — pre-reveal checklist, load order, partial/early-guess handling
- `01_runner_protocol/FAILURE_AND_CONSEQUENCES.md` — failure-changes-situation, cheap-death rules, delayed consequences
- `01_runner_protocol/TONE_AND_NARRATION.md` — locked tone with sentence-level campaign-voice examples
- `01_runner_protocol/WHEN_TO_ASK_QUESTIONS.md` — ask/decide boundaries, no-menu nudges
- `01_runner_protocol/WHEN_TO_IMPROVISE.md` — three-tier improvise boundary tied to canon categories
- `01_runner_protocol/SESSION_END_PROTOCOL.md` — closing beat + full state-update + handoff procedure
- `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md` — complete DM-only Session-1 prompt (load order, character creation, opener, what-not-to-reveal)
- `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md` — complete DM-only Session-2+ prompt (context reconstruction, away-player handling, opening beats)
- `16_ai_session_packs/STATE_UPDATE_TEMPLATE.md` — finalized (placeholder → ready)
- `16_ai_session_packs/COMPACT_CONTEXT_TEMPLATE.md` — finalized (placeholder → ready)
- `16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md` — finalized (placeholder → ready)
- `02_runtime_state/CURRENT_STATE.md` — seeded campaign-start baseline
- `02_runtime_state/CURRENT_LOCATION.md` — seeded starting location (Hollowmere / Mourner's Green)
- `02_runtime_state/CURRENT_SCENE.md` — seeded opening scene (Opener A) with DM-only notes
- `02_runtime_state/ACTIVE_QUESTS.md` — seeded Hook 1 active + Hooks 5–7 available
- `02_runtime_state/OPEN_THREADS.md` — seeded 5 opening loose ends (player-known vs. DM-only separated)
- `02_runtime_state/FACTION_STATE.md` — seeded all 7 factions at Stage 1 baseline posture
- `02_runtime_state/NEXT_SESSION_START.md` — seeded ready-to-run Session-1 opener with hidden notes
- `02_runtime_state/PLAYER_CHARACTER.md` — scaffold + opening condition notes (class/level TBD by player)
- `00_control/STAGE_STATUS.md`, `CONTENT_INDEX.md`, `TAG_INDEX.md`, `TODO.md`, `PROGRESS_LOG.md` — tracking updates

### Canon Established
- None. No new world facts created; runtime layer only.

### Player-Safe Facts Added
- None new (state seeds reuse existing player-safe Stage 1 facts).

### DM-Only Facts Added
- None new (protocols and prompts reference existing DM-only canon; secrecy preserved).

### Runtime State Updated
- 8 state files seeded from Stage 1 content (`CURRENT_STATE`, `CURRENT_LOCATION`, `CURRENT_SCENE`, `ACTIVE_QUESTS`, `OPEN_THREADS`, `FACTION_STATE`, `NEXT_SESSION_START`, `PLAYER_CHARACTER` scaffold). `WORLD_CLOCKS` already populated in Stage 1.

### Indexes Updated
- `CONTENT_INDEX.md` — protocol + session-pack statuses updated from placeholder to complete/ready/seeded
- `TAG_INDEX.md` — status tags moved (placeholder → complete/static/template/runtime); removed from `status:placeholder`

### Gaps Identified
- Stage 3 (starting region deep build) not yet started — the campaign is runnable for the opening sessions but the Reach beyond Hollowmere needs settlements, wilderness sites, dungeons, and encounter/rumor tables.
- `INVENTORY_AND_REWARDS`, `RELATIONSHIPS`, `NPC_MEMORY`, `KNOWN_CLUES`, `HIDDEN_CLUES`, `CONSEQUENCES`, `SESSION_RECAP` remain at empty-start baselines by design (populated in play); they did not require Stage-1 seeding.
- Full encounter tables (Stage 13) and the drowned shrine dungeon (Stage 12) still pending for deeper play.

### Next Recommended Pass
- Begin Stage 3: Starting Region Deep Build (settlements, wilderness locations, local dungeons/ruins, regional quest/encounter/rumor tables) so the Sundering Reach can support 10–20 sessions of open-world play.

---

## 2026-06-09 — Stage 1: Campaign Foundation

### Stage
Stage 1 — Campaign Foundation (complete)

### Summary
Established the full campaign foundation for an original folk-horror frontier campaign, "The Long Remembering," set on the continent of Orrun in the world of Vael. Created and populated all Stage 1 required outputs: canon (player-safe and DM-only), supporting canon (history, cosmology, gods, magic, calendar, languages, leveling), world atlas, level 1–20 main arc and progression, the mystery web (M0–M10 with 3+ clue paths each), revelation map (R1–R8), secret index (20 secrets), seven major factions (each with public face, hidden agenda, leader, members, resources, and an escalation clock), twenty major NPCs (each with a secret and a motivation), the starting region (Sundering Reach) and settlement (Hollowmere), ten session-sized hooks, twenty rumors, three opening scenes with a recommended default, a solo-play safety mechanism, and ten populated world clocks (master clock: The Harvest Restarts). Registered all names in NAMING_REGISTRY, updated both indexes, MANIFEST, STAGE_STATUS, and TODO. World is 100% original; player-safe and DM-only content strictly separated.

### Files Created
- `07_factions/major_factions/ASHEN_WARDENS.md`
- `07_factions/major_factions/CINDER_LEDGER.md`
- `07_factions/major_factions/MOURNERS_CIRCLE.md`
- `07_factions/major_factions/REACHWARD_COMPACT.md`
- `07_factions/major_factions/GRAVECALLERS.md`
- `07_factions/major_factions/CONCORD_REMNANT.md`
- `07_factions/major_factions/HOLLOW_COURT.md` (dm-only)
- `07_factions/FACTION_INDEX.md`
- `08_npcs/MAJOR_NPCS.md` (20 major NPCs)
- `08_npcs/NPC_INDEX.md`
- `05_regions/SUNDERING_REACH.md`
- `06_settlements/HOLLOWMERE.md`
- `09_quests/HOOKS_TABLE.md` (10 hooks)
- `09_quests/RUMORS_TABLE.md` (20 rumors)
- `16_ai_session_packs/OPENING_SCENES.md` (3 openers + default)
- `16_ai_session_packs/SOLO_SAFETY_START.md`

### Files Changed (placeholders populated)
- `03_canon/CANON.md`, `PLAYER_SAFE_CANON.md`, `DM_ONLY_CANON.md`, `CAMPAIGN_IDENTITY_LOCK.md` (locked)
- `03_canon/WORLD_HISTORY.md`, `COSMOLOGY.md`, `GODS_AND_FAITHS.md`, `MAGIC_RULES.md`, `CALENDAR.md`, `LANGUAGES.md`, `LEVELING_ASSUMPTIONS.md`
- `04_world_atlas/WORLD_OVERVIEW.md`, `MAP_DESCRIPTION.md`
- `12_campaign_arc/MAIN_ARC_OVERVIEW.md`, `LEVEL_1_TO_20_PROGRESSION.md`
- `11_mysteries_and_secrets/MYSTERY_WEB.md`, `REVELATION_MAP.md`, `SECRET_INDEX.md`
- `02_runtime_state/WORLD_CLOCKS.md` (10 clocks populated)
- `00_control/NAMING_REGISTRY.md`, `CONTENT_INDEX.md`, `TAG_INDEX.md`, `MANIFEST.md`, `STAGE_STATUS.md`, `TODO.md`

### Canon Established
- Campaign: "The Long Remembering"; world Vael / continent Orrun; current year AQ 101.
- The Quietfall (~century-ago collapse of the Custodian Concord) as the world's founding trauma.
- The Three Thresholds faith; the Quiet Country afterlife; Remembrance as a setting force layered on 5e.
- Starting region (Sundering Reach) and settlement (Hollowmere) with full DM-only truth.
- Full hidden truth chain (DM-only): the Concord harvested the dead; the Quietfall was deliberate; the Hollow Court is restarting the harvest.

### Player-Safe Facts Added
- World/continent names, the Quietfall, the failing death-rites, the five named regions, the public faces of all seven factions, the calendar, common faith and folk customs.

### DM-Only Facts Added
- The full harvest/Quietfall/Hollow Court truth; 20 secrets; every NPC secret; every faction hidden agenda; the player-steering thread; mystery answers.

### Runtime State Updated
- `02_runtime_state/WORLD_CLOCKS.md` — 10 campaign clocks established at Stage 1 baseline.

### Indexes Updated
- `CONTENT_INDEX.md`, `TAG_INDEX.md`, `NAMING_REGISTRY.md`, plus new `FACTION_INDEX.md` and `NPC_INDEX.md`.

### Gaps Identified
- Stage 2 (AI runtime protocols + start/resume prompts + remaining runtime state seeding) not yet done.
- `CLUE_INDEX.md` individual clue files deferred to Stage 3.
- Secondary/minor NPCs referenced in faction files (Pell, Tallytooth Ren, Bann Oester, Pevin Oss, Custodian Orre) need full entries in Stage 3/9.
- The drowned shrine dungeon needs a full build (Stage 12); endgame act files and bestiary (Stages 13/15).

### Next Recommended Pass
- Begin Stage 2: AI Runtime Foundation. Populate the 17 runner protocols, START/RESUME prompts, and seed the remaining runtime state files (CURRENT_STATE, PLAYER_CHARACTER scaffolding, NEXT_SESSION_START) from the Stage 1 opening scenes and clocks.

---

## 2026-06-09 — Stage 0: Full Index Reconciliation Pass

### Stage
Stage 0 — Repository Setup (index reconciliation)

### Summary
Performed a comprehensive gap analysis of CONTENT_INDEX.md and TAG_INDEX.md against all files in the repository. Found 70+ files that existed but were not indexed. Fully rewrote TAG_INDEX.md to register all 90 files across correct type, secrecy, status, and function tags. Rewrote CONTENT_INDEX.md bottom half to add 7 new sections (Campaign Arc, World Atlas, Mystery Infrastructure, Canon Files, Runtime State, expanded Protocol, Generation Backlog) and expand two existing sections. Both indexes now reflect the full Stage 0 scaffold.

### Files Created
- None.

### Files Changed
- `00_control/CONTENT_INDEX.md` — major expansion; all 90 repository files now indexed
- `00_control/TAG_INDEX.md` — full rewrite; all files registered across type/secrecy/status/function tags

### Canon Established
- None.

### Indexes Updated
- `CONTENT_INDEX.md`
- `TAG_INDEX.md`

### Gaps Identified
- Stage 1 campaign world content still does not exist.
- Runner protocol placeholder files (17) still need real content in Stage 2.
- Session pack prompt files (2) need real content once Stage 1 is complete.

### Next Recommended Pass
- Begin Stage 1: Campaign Foundation.

---

## 2026-06-09 — Stage 0: Cleanup Pass (New Control Files)

### Stage
Stage 0 — Repository Setup (cleanup pass)

### Summary
User added four new control/canon files: `CANON_AUTHORITY.md`, `GENERATION_GUARDRAILS.md`, `NAMING_REGISTRY.md` (all in `00_control/`), and `RULESET_ASSUMPTIONS.md` (in `00_control/`). Updated `CLAUDE.md` to reference these files in Non-Negotiable Rules and Required Work Pattern. This pass registered all four files in indexes, fixed a path mismatch in `CLAUDE.md` (`03_canon/RULESET_ASSUMPTIONS.md` → `00_control/RULESET_ASSUMPTIONS.md`), added a Purpose/Status header to `NAMING_REGISTRY.md`, added a God/Artifact name section to `NAMING_REGISTRY.md`, expanded `RETRIEVAL_GUIDE.md` with a pre-content-generation checks table, updated `CONTENT_INDEX.md` and `TAG_INDEX.md`, and corrected a bad file reference in `TODO.md` (non-existent `ENCOUNTER_DESIGN_FOR_SOLO_PLAY.md` → `RULESET_ASSUMPTIONS.md`).

### Files Created
- none (user created the four new files)

### Files Changed
- `CLAUDE.md` — fixed path: `03_canon/RULESET_ASSUMPTIONS.md` → `00_control/RULESET_ASSUMPTIONS.md`
- `00_control/NAMING_REGISTRY.md` — added Purpose/Status header and God/Artifact name sections
- `00_control/CONTENT_INDEX.md` — added entries for CANON_AUTHORITY, GENERATION_GUARDRAILS, NAMING_REGISTRY, RULESET_ASSUMPTIONS, DND_MECHANICS_REQUIREMENTS
- `00_control/TAG_INDEX.md` — added all four new files to `status:complete`
- `00_control/MANIFEST.md` — noted cleanup pass
- `00_control/RETRIEVAL_GUIDE.md` — added Pre-Content-Generation Checks table
- `00_control/TODO.md` — fixed bad file reference in critical task

### Canon Established
- None.

### Indexes Updated
- `CONTENT_INDEX.md`
- `TAG_INDEX.md`

### Gaps Identified
- The critical TODO task (add mechanical completeness requirements to content templates) remains unstarted.

### Next Recommended Pass
- Begin Stage 1: Campaign Foundation.

---

## 2026-06-09 — Stage 0: Repository Scaffold

### Stage
Stage 0 — Repository Setup

### Summary
Created the complete repository scaffold for the AI solo campaign. All required folders, placeholder files, tracking files, runtime state placeholders, canon placeholders, index files, and control files are now in place. No campaign world content has been generated yet. The project is ready to begin Stage 1 content generation.

### Files Created

**Control files:**
- `00_control/MANIFEST.md` — project identity and folder map
- `00_control/STAGE_STATUS.md` — stage completion tracker
- `00_control/PROGRESS_LOG.md` — this file
- `00_control/TODO.md` — prioritized work queue
- `00_control/OPEN_QUESTIONS.md` — unresolved design questions
- `00_control/CONSISTENCY_AUDIT.md` — running issue tracker
- `00_control/CONTENT_INDEX.md` — global content inventory
- `00_control/TAG_INDEX.md` — retrieval tag index
- `00_control/RETRIEVAL_GUIDE.md` — AI DM file load guide

**Runner protocol placeholders:**
- `01_runner_protocol/SOLO_PLAY_PRINCIPLES.md`
- `01_runner_protocol/SESSION_LOOP.md`
- `01_runner_protocol/SCENE_FRAMING.md`
- `01_runner_protocol/PLAYER_CHOICE_PROTOCOL.md`
- `01_runner_protocol/ROLL_AND_CHECK_PROTOCOL.md`
- `01_runner_protocol/COMBAT_PROTOCOL.md`
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`
- `01_runner_protocol/EXPLORATION_PROTOCOL.md`
- `01_runner_protocol/TRAVEL_PROTOCOL.md`
- `01_runner_protocol/DOWNTIME_PROTOCOL.md`
- `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md`
- `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md`
- `01_runner_protocol/FAILURE_AND_CONSEQUENCES.md`
- `01_runner_protocol/TONE_AND_NARRATION.md`
- `01_runner_protocol/WHEN_TO_ASK_QUESTIONS.md`
- `01_runner_protocol/WHEN_TO_IMPROVISE.md`
- `01_runner_protocol/SESSION_END_PROTOCOL.md`

**Runtime state placeholders:**
- `02_runtime_state/CURRENT_STATE.md`
- `02_runtime_state/PLAYER_CHARACTER.md`
- `02_runtime_state/CURRENT_LOCATION.md`
- `02_runtime_state/CURRENT_SCENE.md`
- `02_runtime_state/ACTIVE_QUESTS.md`
- `02_runtime_state/OPEN_THREADS.md`
- `02_runtime_state/KNOWN_CLUES.md`
- `02_runtime_state/HIDDEN_CLUES.md`
- `02_runtime_state/NPC_MEMORY.md`
- `02_runtime_state/FACTION_STATE.md`
- `02_runtime_state/WORLD_CLOCKS.md`
- `02_runtime_state/INVENTORY_AND_REWARDS.md`
- `02_runtime_state/RELATIONSHIPS.md`
- `02_runtime_state/CONSEQUENCES.md`
- `02_runtime_state/SESSION_RECAP.md`
- `02_runtime_state/NEXT_SESSION_START.md`

**Canon placeholders:**
- `03_canon/CANON.md`
- `03_canon/PLAYER_SAFE_CANON.md`
- `03_canon/DM_ONLY_CANON.md`
- `03_canon/WORLD_HISTORY.md`
- `03_canon/COSMOLOGY.md`
- `03_canon/GODS_AND_FAITHS.md`
- `03_canon/MAGIC_RULES.md`
- `03_canon/CALENDAR.md`
- `03_canon/LANGUAGES.md`
- `03_canon/LEVELING_ASSUMPTIONS.md`

**World atlas placeholders:**
- `04_world_atlas/WORLD_OVERVIEW.md`
- `04_world_atlas/MAP_DESCRIPTION.md`

**Campaign arc placeholders:**
- `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
- `12_campaign_arc/LEVEL_1_TO_20_PROGRESSION.md`

**Mystery placeholders:**
- `11_mysteries_and_secrets/MYSTERY_WEB.md`
- `11_mysteries_and_secrets/REVELATION_MAP.md`
- `11_mysteries_and_secrets/CLUE_INDEX.md`
- `11_mysteries_and_secrets/SECRET_INDEX.md`

**Session pack placeholders:**
- `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`
- `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`
- `16_ai_session_packs/STATE_UPDATE_TEMPLATE.md`
- `16_ai_session_packs/COMPACT_CONTEXT_TEMPLATE.md`
- `16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`

**Generation backlog:**
- `17_generation_backlog/CONTENT_GAPS.md`
- `17_generation_backlog/EXPANSION_PLAN.md`

**Folder structure established:**
- `05_regions/` — empty, ready for region files
- `06_settlements/` — empty, ready for settlement files
- `07_factions/major_factions/` — empty, ready for faction files
- `07_factions/minor_factions/` — empty, ready for faction files
- `08_npcs/` — empty, ready for NPC files
- `09_quests/` — empty, ready for quest files
- `10_dungeons_and_ruins/` — empty, ready for dungeon files
- `13_encounters_and_bestiary/` — empty
- `14_treasure_and_artifacts/` — empty
- `15_random_tables/` — empty
- `18_audits/` — empty

### Files Changed
- `README.md` — updated from package instructions to repo readme

### Canon Established
- None. No world content exists yet.

### Player-Safe Facts Added
- None.

### DM-Only Facts Added
- None.

### Runtime State Updated
- None. All runtime state files are empty placeholders.

### Indexes Updated
- `CONTENT_INDEX.md` — created with empty tables and control file entries
- `TAG_INDEX.md` — created with full tag vocabulary, no content entries yet

### Gaps Identified
- All campaign world content (Stage 1 and beyond)
- All runner protocol content (Stage 2)
- Runtime state requires player character and campaign start before it can be populated

### Next Recommended Pass
- Begin Stage 1: Campaign Foundation
- Use prompt in README.md or TRACKING_SYSTEM.md
- Establish campaign premise, central conflict, hidden truth, 5–8 factions, 20 major NPCs, 20 secrets, starting region, starting settlement, 10 hooks, 20 rumors, opening scenes
