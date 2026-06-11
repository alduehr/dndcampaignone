# RETRIEVAL_GUIDE.md

## Purpose

Tells the AI DM which files to load, when to load them, and how to use them. This is the navigation layer for the campaign repository.

## Current Status

Stages 1–5 and 7 complete. Session load order, contextual load rules, pre-content-generation checks, and secrecy enforcement are operational. Sundering Reach (Stage 3), Caradril city (Stage 4), the Level 1–4 Act 1 play kit (Stage 5), and the three Ring 1 adjacent regions (Stage 7 — Ashgarden Vale, Tollwood, Pale Coast) world content load entries are live below. **Full-World Cartographic Expansion pass:** the World map / cartography section now lists both the **campaign-area** (NW Orrun) and **full-continent** atlas file sets.

---

## Core Principle

**Load only what you need.** Loading everything at once wastes context. Use this guide to load the minimum necessary files for the current scene, then expand if needed.

---

## Session Start Load Order

When starting or resuming a session, load in this order:

1. `02_runtime_state/CURRENT_STATE.md` — where things stand right now
2. `02_runtime_state/CURRENT_LOCATION.md` — where the player is
3. `02_runtime_state/CURRENT_SCENE.md` — what is happening
4. `02_runtime_state/PLAYER_CHARACTER.md` — player stats, resources, condition
5. `02_runtime_state/ACTIVE_QUESTS.md` — live quests
6. `02_runtime_state/NPC_MEMORY.md` — relevant NPC attitudes
7. `02_runtime_state/FACTION_STATE.md` — faction positions
8. `02_runtime_state/WORLD_CLOCKS.md` — escalating threats
9. `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md` — session opening guidance

Then load relevant world files based on current location, active quests, and NPCs present.

---

## New Campaign Start Load Order

When beginning a brand-new campaign:

1. `03_canon/CANON.md`
2. `03_canon/PLAYER_SAFE_CANON.md`
3. `03_canon/DM_ONLY_CANON.md`
4. `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
5. `02_runtime_state/PLAYER_CHARACTER.md`
6. Relevant starting region file
7. Relevant starting settlement file
8. `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`

---

## Contextual Load Rules

### When in a settlement
Load:
- Settlement file
- Region file (if not already loaded)
- NPCs present at current location
- Active quests relevant to this settlement
- Faction state for factions active here

### When in a dungeon or ruin
Load:
- Dungeon/ruin file
- Quest file(s) pointing here
- Any relevant clues or mysteries
- Encounter context for current zone

### When in wilderness or travel
Load:
- Region file
- Travel protocol: `01_runner_protocol/TRAVEL_PROTOCOL.md`
- Relevant encounter table
- Any travel events or faction activity in this zone

### When in a social scene
Load:
- NPC file(s) for present NPCs
- Faction file if faction politics are at stake
- Relevant quest file if the scene advances a quest
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`

### When delivering a clue
Load:
- Relevant clue file
- Mystery file the clue feeds into
- `02_runtime_state/KNOWN_CLUES.md` to check what the player already knows
- `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md`

### When a secret is about to be revealed
Load:
- `03_canon/DM_ONLY_CANON.md` — check what is still hidden
- `02_runtime_state/KNOWN_CLUES.md` — check discovery trail
- `01_runner_protocol/SECRET_REVEAL_PROTOCOL.md`

### At session end
Load:
- `16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`
- All runtime state files that changed this session

---

## Pre-Content-Generation Checks

Before creating any major new content (NPCs, factions, regions, quests, mysteries, monsters, artifacts), check these files first:

| File | What To Check |
|---|---|
| `00_control/CANON_AUTHORITY.md` | Which file wins if there's a contradiction |
| `00_control/GENERATION_GUARDRAILS.md` | Drift prevention — does this new content fit the project? |
| `00_control/NAMING_REGISTRY.md` | Is this name already taken or forbidden? |
| `00_control/RULESET_ASSUMPTIONS.md` | Are mechanics consistent with D&D 5e / 2024? |
| `00_control/DND_MECHANICS_REQUIREMENTS.md` | Does this content meet mechanical completeness requirements? |
| `03_canon/CANON.md` | Does this contradict established canon? |

These checks take seconds and prevent large-scale rework later.

---

## File Priority Levels

| Priority | Meaning | Examples |
|---|---|---|
| Always load | Required for any session | CURRENT_STATE, PLAYER_CHARACTER, CURRENT_LOCATION |
| Load on demand | Load when relevant | NPC files, quest files, dungeon files |
| Load for secrets | DM-only; never surface to player | DM_ONLY_CANON, HIDDEN_CLUES, mystery files |
| Reference only | Load to check standards, not during play | Standards files, AUDIT_STANDARDS |

---

## Secrecy Enforcement

**Never load DM-only files and then summarize their contents to the player.**

- `secrecy:dm-only` files are for AI DM reasoning only.
- `secrecy:player-safe` files can be paraphrased, quoted, or described to the player.
- `secrecy:mixed` files require care — read the individual sections before using.

---

## Stage 3 World Content Load Entries (Sundering Reach)

These files exist and are loadable as of Stage 3. Always load the minimum needed for the current scene.

### Region
- `05_regions/SUNDERING_REACH.md` — full region overview; load when entering a new zone or for travel context

### Settlements
- `06_settlements/HOLLOWMERE.md` — starting town; load every session set here
- `06_settlements/KETTLE_BRIDGE.md` — eastern toll-town
- `06_settlements/SALTMARGIN.md` — western salt-trade town
- `06_settlements/CANDLEWICK.md` — southern village; Concord Script clue gate
- `06_settlements/GREYWATER_HOLM.md` — fen-edge village; cult spread
- `06_settlements/HARROWGAST.md` — heights mining village; Deep Adit entrance
- `06_settlements/REEDFORD.md` — central ford hamlet; low-danger waypoint
- `06_settlements/THE_ASHWALK_REST.md` — Warden waystation; solo-safety sanctuary

### Wilderness Zones
- `05_regions/wilderness/GREYFENS_SITES.md` — fen sites; Gravecaller activity
- `05_regions/wilderness/SUNDER_HEIGHTS_SITES.md` — highlands; old glass; Remnant race
- `05_regions/wilderness/MIREWEND_AND_ROADS_SITES.md` — river and Concord road sites; travel layer
- `05_regions/wilderness/BASIN_SHORE_AND_HOLMS_SITES.md` — basin shore; deep basin gated to endgame

### Dungeons / Ruins
- `10_dungeons_and_ruins/THE_PEAT_CHAPEL.md` — intended first delve; level 1–2
- `10_dungeons_and_ruins/THE_SUNKEN_TOLLHOUSE.md` — river node; level 2–3
- `10_dungeons_and_ruins/THE_WHISPERING_CAIRN.md` — Concord Script gate; level 2–3
- `10_dungeons_and_ruins/THE_LEDGER_VAULT.md` — social/stealth heist in Hollowmere; level 2–4
- `10_dungeons_and_ruins/THE_BARROW_OF_NINE_DOORS.md` — parley-boss barrow; level 3–5
- `10_dungeons_and_ruins/THE_DEEP_ADIT.md` — harvest node; level 4–6; thin-touch risk

### NPCs
- `08_npcs/MAJOR_NPCS.md` — 20 full-profile major NPCs; load when relevant NPC is present
- `08_npcs/SECONDARY_NPCS.md` — ~21 secondary NPCs; load by location
- `08_npcs/MINOR_NPCS.md` — ~35 minor NPCs; load by settlement
- `08_npcs/NPC_INDEX.md` — master lookup table

### Quests
- `09_quests/HOOKS_TABLE.md` — first 10 hooks (Hook 1 = default opener)
- `09_quests/RUMORS_TABLE.md` — first 20 rumors
- `09_quests/hooks_and_rumors/SUNDERING_REACH_HOOKS.md` — hooks H11–H39
- `09_quests/hooks_and_rumors/SUNDERING_REACH_RUMORS.md` — rumors R21–R50
- `09_quests/regional_quests/Q_*.md` — 14 developed quests; load when quest is active

### Encounters
- `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md` — 4 solo-tuned zone tables; load during travel or wilderness scenes

### Clues / Mysteries
- `11_mysteries_and_secrets/CLUE_INDEX.md` — all authored clues with locations and methods (DM-only)
- `02_runtime_state/HIDDEN_CLUES.md` — runtime mirror; tracks discovery status (DM-only)
- `11_mysteries_and_secrets/MYSTERY_WEB.md` — full mystery network (DM-only)

### Factions
- `07_factions/major_factions/` — load relevant faction file when faction is active in current scene
- `07_factions/FACTION_INDEX.md` — master table and relationship map

---

## Stage 4 World Content Load Entries (Caradril — First Major City)

The mid-game hub (~levels 5–12, with level 3–5 on-ramps and level 12+ threads). Load the minimum needed for the current district/scene.

### City Overview
- `06_settlements/CARADRIL.md` — load on arrival and for any city-wide question (government, services, scale, secrets)

### Districts (load the one the player is in)
- `06_settlements/caradril_districts/THE_MAGISTERIUM.md` — government, charter politics, the Watch, the Pale Star base
- `06_settlements/caradril_districts/THE_COUNTING_QUAYS.md` — Cinder Ledger HQ; Vyre; the deal (M3/M6)
- `06_settlements/caradril_districts/THE_LANTERN_REACH.md` — Concord Remnant; Concord Script; the Sealed Archive (M6/M9)
- `06_settlements/caradril_districts/THE_ASHMARKET.md` — relic/salvage trade; quiet-coin (M3)
- `06_settlements/caradril_districts/HIGHMOURN.md` — temples, funerals, healing/rest; the raise-dead cover-up
- `06_settlements/caradril_districts/THE_CRUCIBLE.md` — foundries, gear, relic-smelting (M3)
- `06_settlements/caradril_districts/THE_SILL.md` — poor undercity; the Hush; refugees; the Sealgate
- `06_settlements/caradril_districts/THE_SUNKEN_WARDS.md` — the city's sub-dungeon (Lvl 6–14); load as a dungeon

### City NPCs / Quests / Encounters
- `08_npcs/SECONDARY_NPCS.md` (Caradril section), `MINOR_NPCS.md` (Caradril section) — load by district
- `09_quests/city_quests/` — 11 developed city quests; load when active
- `09_quests/hooks_and_rumors/CARADRIL_HOOKS.md`, `CARADRIL_RUMORS.md` — city hooks/rumors by district
- `13_encounters_and_bestiary/CARADRIL_ENCOUNTERS.md` — district social/intrigue tables + the Sunken Wards dungeon table

### City Clocks / Clue Access
- `02_runtime_state/WORLD_CLOCKS.md` (city clocks C1/C2/C3) and `FACTION_STATE.md` (Caradril city factions) — load for city faction behavior
- `11_mysteries_and_secrets/CLUE_INDEX.md` + `02_runtime_state/HIDDEN_CLUES.md` (Stage 4 Caradril anchors) — DM-only; the city's M2/M3/M4/M6/M8/M9 access points

**Caradril secrecy reminder:** the Sealed Archive (M6/M9) is Act 3 / L9–12; earlier visits give M2/M3 *fragments and demonstrations*. **Never name the Hollow Court (M7) in Caradril.** The Reke "correspondent" thread is a *lead*, not a named second agent — do not pre-resolve it.

---

## Stage 5 Act 1 Load Entries (Levels 1–4 Play Kit)

The open-world Act 1 toolkit. Load when starting a campaign or planning/running any L1–4 session in the Sundering Reach. **Reveal cap for the whole act: R1 only** (the failures have a source and a pattern; the basin is the center) — never surface Remembrance-as-substance, Reke's treachery, the steering employer, the Concord's sin, or the Hollow Court.

### Arc Spine (load at campaign start and when planning an Act 1 session)
- `12_campaign_arc/ACT_1_LEVELS_1_4.md` — the open-world Act 1 spine: the Five Doors + seven faction doors, multi-route to R1, ignore-consequences, Act 2 triggers. The DM's Act 1 map.
- `12_campaign_arc/ACT_1_MILESTONES.md` — explicit L2/3/4 + L4→5 level-up triggers (multiple paths; optional XP guidance). Load when deciding a level-up.
- `12_campaign_arc/ACT_1_FAILURE_STATES.md` — 9 redirect-not-end failure cases. Load when the player fails, flees, is jailed, or burns a bridge.

### Act 1 Quests (load when a faction door is engaged)
- `09_quests/act_1_quests/Q_ACT1_WARDEN_THE_TRUE_RITE.md` — Ashen Wardens (Hook 9 / Wren)
- `09_quests/act_1_quests/Q_ACT1_COMPACT_THE_REEVES_DOUBT.md` — Reachward Compact (Hook 5)
- `09_quests/act_1_quests/Q_ACT1_LEDGER_A_QUIET_SALVAGE.md` — Cinder Ledger (Hook 3)
- `09_quests/act_1_quests/Q_ACT1_MOURNER_SALT_AND_SONG.md` — Mourners' Circle (Hook 2)
- `09_quests/act_1_quests/Q_ACT1_GRAVECALLER_A_LAST_WORD.md` — Gravecallers (Hook 7)
- `09_quests/act_1_quests/Q_ACT1_REMNANT_THE_VISITING_SCHOLAR.md` — Concord Remnant (Hook 8)
- (The Hollow Court has **no** friendly quest by design; Reke's covert steering runs through Hook 4 in `HOOKS_TABLE.md`.)

### Act 1 Threats (load during a L1–4 combat/encounter scene)
- `13_encounters_and_bestiary/ACT_1_THREATS.md` — the 5 recurring early-threat profiles (Restless/Wrathful Remembrance, Frontier Toughs, Cult Radical's Hand, Rival Salvage Crew); full stat profiles, solo-safe, noncombat outs, scaling. Use alongside `SUNDERING_REACH_ENCOUNTERS.md`.

### Act 1 Clue Access (DM-only; load when delivering a clue at L1–4)
- `11_mysteries_and_secrets/ACT_1_CLUE_TRAILS.md` — which existing M1–M9 clues a L1–4 player reaches, the multi-route access to R1, and the three-clue check. **DM-only.** Use with `CLUE_INDEX.md` + `HIDDEN_CLUES.md`.

### Act 1 NPC Casting (load when staffing an Act 1 scene or if the player is stuck)
- `08_npcs/ACT_1_NPC_GUIDE.md` — existing NPCs as Act 1 allies/patrons/rivals/witnesses/complications, with entry conditions and **Safe Re-Entry Points** for a lost player. No new NPCs — points into `MAJOR_NPCS.md`/`SECONDARY_NPCS.md`.

**Act 1 secrecy reminder:** Reke is a *reasonable politician with a project*, not an exposed traitor; the shrine is a *hazard and a shape*, not a named engine; the dead are *drawn to the water* for reasons unknown. Cap every Act 1 reveal at R1.

---

## Stage 7 World Content Load Entries (Ring 1 — Adjacent Regions)

The three regions adjacent to the Reach. Load the relevant region file when the player travels south (Vale), east (Tollwood), or west (Coast), then the specific settlement/wilderness/dungeon for the scene. **All Ring 1 sites feed existing M1–M9 (mostly M2/M3/M5 fragments, gated/oblique M6) — never name the Hollow Court (M7) or the harvest mechanism; cap reveals (R1 at Act-1 levels; R2 at L5+; never R3+ in Ring 1).**

### Travel (load when leaving or crossing between regions)
- `04_world_atlas/TRAVEL_ROUTES_RING1.md` — 6 routes (Reach→each region; each region→Caradril); times, dangers, faction presence, travel events. Use with `TRAVEL_PROTOCOL.md` and the regional encounter tables.

### World map / cartography (load for placement, "what lies beyond," or to generate a map)

**Two scopes:** the **campaign-area** files (NW Orrun cluster — the day-to-day play map) and the **full-continent** files (whole of Orrun — "what lies beyond the frontier"). Load the campaign-area set for ordinary placement and play maps; load the full set when the player asks about the wider continent or you need a whole-world map.

*Campaign-area (NW Orrun cluster):*
- `04_world_atlas/WORLD_MAP_AUTHORITY.md` — **campaign-area cartographic authority.** Load to place any new location within the cluster, confirm travel-time plausibility, or before commissioning a cluster map. Player-safe §11 facts only to the player.
- `04_world_atlas/WORLD_MAP_COORDINATES.md` — campaign-area 0–100 grid (~3× zoom on the NW corner); confidence-rated; DM-only rows flagged.
- `04_world_atlas/WORLD_MAP_LAYERS.md` — 7 campaign-area map layers. **Layers 2 & 7 are DM-only.**
- `04_world_atlas/WORLD_MAP_PROMPTS.md` — 4 campaign-area image prompts. **Prompts 1 & 3 are player-safe.** Recommended first cluster map: Prompt 3 (Reach + Ring 1 regional).

*Full continent (Orrun + Vael landmasses):*
- `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` — **full-continent master reference.** Load to answer "what lies beyond the frontier," place a far region, or before commissioning a whole-world map. NW→SE axis; 18 regions (5 built + 13 placeholder); player-safe §11 only to the player; keep DM-only (Concord Deep, keystone, far-ruin truth) hidden. **Endgame stays vertical under Hollowmere — never a distant land.**
- `04_world_atlas/FULL_WORLD_MAP_COORDINATES.md` — full-continent 0–100 grid (124 entries; embeds the cluster in the NW corner via a documented rescale); confidence-rated; DM-only rows flagged.
- `04_world_atlas/FULL_WORLD_MAP_LAYERS.md` — 8 full-world map layers (incl. a campaign-area inset). **Layers 2, 4, & 7 are DM-only — never render for the player.**
- `04_world_atlas/FULL_WORLD_MAP_PROMPTS.md` — 5 full-world image prompts. **Prompts 1, 3, & 5 are player-safe; Prompt 2 and Prompt 4's DM toggles are DM-only.** Recommended first map overall: Prompt 5 (campaign inset); then Prompt 1 (player-safe continent); then Prompt 3 (parchment artifact).
- `04_world_atlas/REGION_INDEX.md` — index of authored regions + campaign-area + full-continent placeholders (directions, levels, grid, secrecy).

### Ashgarden Vale (S — gentlest Ring 1, Lvl 1–6)
- `05_regions/ASHGARDEN_VALE.md` — region overview
- `06_settlements/ORCHARDMERE.md` (hub) · `SAINT_VEDDOWS_REST.md` (pilgrimage; the node) · `TILBROOK.md` (honest M5 window)
- `05_regions/wilderness/ASHGARDEN_VALE_SITES.md` — 6 sites + 3 hamlets
- Dungeons: `10_dungeons_and_ruins/SAINT_VEDDOWS_TOMB.md` (gated node; L4–6) · `THE_BURIED_CLOISTER.md` (L2–4) · `THE_PELLOW_GRANGE.md` (social; L2–4)
- `13_encounters_and_bestiary/ASHGARDEN_VALE_ENCOUNTERS.md` · `09_quests/hooks_and_rumors/ASHGARDEN_VALE_HOOKS.md`/`_RUMORS.md` · 8 Vale `Q_*` quests
- **Secrecy:** the Vale's "the rites always held" is denial; cap at R1. Saint Veddow's Tomb gives M2/M6 *fragments* only; never the Court.

### Tollwood (E — most dangerous Ring 1, Lvl 2–7)
- `05_regions/TOLLWOOD.md` — region overview
- `06_settlements/HARTFELL.md` (hub) · `COLDHEARTH.md` (deep village; the bargain) · `TOLLSTONE_CROSS.md` (toll-war)
- `05_regions/wilderness/TOLLWOOD_SITES.md` — 6 sites; the deep wood gated
- Dungeons: `10_dungeons_and_ruins/THE_GREENWARD_TOLL_STATION.md` (L2–4) · `THE_HANGING_OAKS.md` (L4–6) · `THE_OLD_MAST.md` (**gated apex, L6–10**)
- `13_encounters_and_bestiary/TOLLWOOD_ENCOUNTERS.md` (deep-wood table is deadliest) · `TOLLWOOD_HOOKS.md`/`_RUMORS.md` · 7 Tollwood `Q_*` quests
- **Secrecy:** the Old Mast's pre-Concord "presence" is a **gated regional landmark-power, NOT the Hollow Court or a new god**; it gives oblique M5/M6 *fragments and dread* only. The deep wood pushes the unworthy out alive (telegraphed).

### Pale Coast (W — sea-and-survival, Lvl 2–7; Saltmargin is the existing gateway)
- `05_regions/PALE_COAST.md` — region overview
- `06_settlements/WRACKMOUTH.md` (hub/port; water-route to Caradril) · `COBBLE_STRAND.md` (honest M5/M2 window; salt-and-tide rite) · `SALTMARGIN.md` *(existing Reach town; the gateway — do not recreate)*
- `05_regions/wilderness/PALE_COAST_SITES.md` — 6 sites; the Skerries gated
- Dungeons: `10_dungeons_and_ruins/THE_DROWNED_LAMP.md` (coastal node; L4–6; tide-locked) · `THE_WRECKERS_CAVES.md` (social/tide; L3–5) · `THE_SKERRY_SHRINE.md` (**gated apex, L6–9**)
- `13_encounters_and_bestiary/PALE_COAST_ENCOUNTERS.md` (Skerries table is deadliest) · `PALE_COAST_HOOKS.md`/`_RUMORS.md` · 5 Coast `Q_*` quests
- **Secrecy:** the lighthouses/sea-shrines were maritime harvest-nodes — gated M2/M5/M6 *fragments* only; never the Court. The tide and weather are the safety valves (telegraph constantly).

### Ring 1 NPCs / Clocks
- `08_npcs/SECONDARY_NPCS.md` (Ring 1 sections) + `MINOR_NPCS.md` (Ring 1 sections) — load by region/settlement
- Regional clocks (add to `02_runtime_state/WORLD_CLOCKS.md` on first engagement): Vale **"The Harvest-Moot's Silence"**, Tollwood **"The Old Mast Stirs"**, Coast **"The Drowned Tide Rises"**. The Tollmen are a minor regional faction (`FACTION_STATE.md` if engaged).
- The Mourner folk-truth network (Wend→Combe→Sennet→Bryd) is a slow, gated M6 thread linking the regions; carrying their messages is the through-line.

**Ring 1 secrecy reminder:** every Ring 1 region has an *honest window* (Tilbrook / Coldhearth-Sennet / Cobble Strand-Bryd) that confirms **the failures spread outward from the Reach (M5)** — that is the intended Ring 1 takeaway. The gated apex sites (Old Mast, Skerry Shrine, deep Saint Veddow's/Drowned Lamp) give *fragments and danger*, never the apex truth. **Never name the Hollow Court or the harvest mechanism in any Ring 1 content.**

---

## Related Files

- [`CONTENT_INDEX.md`](CONTENT_INDEX.md)
- [`TAG_INDEX.md`](TAG_INDEX.md)
- [`01_runner_protocol/AI_DM_CORE_RULES.md`](../01_runner_protocol/AI_DM_CORE_RULES.md)
