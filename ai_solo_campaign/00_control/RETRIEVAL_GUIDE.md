# RETRIEVAL_GUIDE.md

## Purpose

Tells the AI DM which files to load, when to load them, and how to use them. This is the navigation layer for the campaign repository.

## Current Status

**Current through Stage 15B (full level 1–20 arc) + Stage 16 correction pass + Cartography Authority Pass (2026-06-16).** The repo is built and audited for live solo play, and is now cartography-deterministic (continent, regions, cities, settlements, routes, water, terrain, and all 36 adventure sites are coordinate-anchored). The Cartography Authority Pass created the master geometry/registry/route/water/terrain authority files in `04_world_atlas/`, 18 region map packets (`04_world_atlas/region_map_packets/`), 4 city map packets + 18 settlement map packets (`06_settlements/city_map_packets/`, `06_settlements/settlement_map_packets/`), and the adventure-site cartography index (`10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`). All of the following authored systems exist and are loadable: canon (player-safe / DM-only split), runtime state, AI DM protocols, the Sundering Reach (starting region), Caradril (first major city), three Ring 1 adjacent regions, the full continent of Orrun (5 built + 13 placeholder far regions), seven major factions (operational with clocks and quest chains), the NPC codex (50 majors + secondaries + minors + far-continent rosters), the quest library, the mystery/clue/secret web, dungeons and adventure sites, the encounter/bestiary library, the treasure/reward/artifact library, and the level 5–20 arc (Tiers 2–4, endgame, region/faction escalation, off-route and ignore-arc guides). Stage 17 (Live Campaign Operation) is next — begin via `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`.

---

## Core Principle

**Load only what you need.** Loading everything at once wastes context. Use this guide to load the minimum necessary files for the current scene, then expand if needed.

---

## Scenario Load Map

The fastest way to use this guide: find your scenario, load the listed files. "Always-on" runtime state (CURRENT_STATE, CURRENT_LOCATION, PLAYER_CHARACTER) is assumed loaded in any active session and is not relisted per scenario.

### Starting a new campaign
1. `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md` — the entry procedure
2. `03_canon/CANON.md`
3. `03_canon/PLAYER_SAFE_CANON.md`
4. `03_canon/DM_ONLY_CANON.md`
5. `12_campaign_arc/MAIN_ARC_OVERVIEW.md`
6. `12_campaign_arc/ACT_1_LEVELS_1_4.md` — the open-world Act 1 spine
7. `02_runtime_state/PLAYER_CHARACTER.md`
8. `05_regions/SUNDERING_REACH.md` + `06_settlements/HOLLOWMERE.md` — starting region/settlement
9. `09_quests/HOOKS_TABLE.md` (Hook 1 = default opener)

### Resuming a campaign mid-session
Load in this order:
1. `02_runtime_state/CURRENT_STATE.md`
2. `02_runtime_state/CURRENT_LOCATION.md`
3. `02_runtime_state/CURRENT_SCENE.md`
4. `02_runtime_state/PLAYER_CHARACTER.md`
5. `02_runtime_state/ACTIVE_QUESTS.md`
6. `02_runtime_state/OPEN_THREADS.md`
7. `02_runtime_state/NPC_MEMORY.md`
8. `02_runtime_state/FACTION_STATE.md`
9. `02_runtime_state/WORLD_CLOCKS.md`
10. `02_runtime_state/KNOWN_CLUES.md`
11. `16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md` + `02_runtime_state/NEXT_SESSION_START.md`

Then load the world files for the current location, active quests, and NPCs present.

### Opening scene / first session
- `16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`
- `12_campaign_arc/ACT_1_LEVELS_1_4.md` + `08_npcs/ACT_1_NPC_GUIDE.md`
- `06_settlements/HOLLOWMERE.md`
- `09_quests/HOOKS_TABLE.md` + `09_quests/RUMORS_TABLE.md`
- `13_encounters_and_bestiary/ACT_1_THREATS.md`
- **Reveal cap: R1 only.** Never surface Remembrance-as-substance, Reke's treachery, the harvest, or the Hollow Court.

### Entering a settlement (any)
- The settlement file (`06_settlements/...`)
- The parent region file if not loaded
- `08_npcs/NPC_INDEX.md` → the relevant NPC roster files for NPCs present
- `02_runtime_state/FACTION_STATE.md` + the relevant faction file(s) for factions active here
- Active quests / hooks relevant to this settlement (`09_quests/QUEST_INDEX.md` → specific files)
- `01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md` if intrigue is at stake

### Entering a region (core Ring 1)
- The region file: `05_regions/ASHGARDEN_VALE.md` / `05_regions/TOLLWOOD.md` / `05_regions/PALE_COAST.md` (or `05_regions/SUNDERING_REACH.md`)
- The region's wilderness sites file (`05_regions/wilderness/..._SITES.md`)
- `04_world_atlas/TRAVEL_ROUTES_RING1.md` for the journey in
- The region's encounter table (`13_encounters_and_bestiary/[REGION]_ENCOUNTERS.md`)
- Region hooks/rumors (`09_quests/hooks_and_rumors/[REGION]_HOOKS.md` / `_RUMORS.md`)
- `15_campaign_arcs/REGIONAL_ARC_PACKS_LEVEL_5_TO_20.md` if the player is L5+ here

### Entering a far-continent region
- `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` (what lies beyond; placement; secrecy)
- `08_npcs/by_region/[REGION]_NPCS.md` — the far-region roster
- `13_encounters_and_bestiary/[REGION]_ENCOUNTERS.md` — the far-region encounter table
- `15_campaign_arcs/REGION_TO_REGION_TRANSITION_GUIDE.md` + `15_campaign_arcs/PLAYER_GOES_ANYWHERE_GUIDE.md`
- `15_campaign_arcs/CONTINENTAL_PRESSURE_TIMELINE.md` for what's happening far away
- **Endgame stays vertical under Hollowmere — never relocate the keystone/Concord Deep/Hollow Court to a distant land.**

### Cartography and map rendering (generating / placing maps)
- **Master geometry:** `04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md` (coastline, rivers, ranges, terrain polygons, region boundaries, routes; the 0–100 render grid).
- **Feature registry:** `04_world_atlas/MAP_FEATURE_REGISTRY.md` (every map-visible feature with coords, visibility flags, confidence) — filter `player_safe_visibility = yes` for player maps; add the DM-only rows for DM maps.
- **Route/water/terrain geometry:** `04_world_atlas/ROADS_RIVERS_AND_ROUTES_AUTHORITY.md` · `WATER_AND_SHORELINE_AUTHORITY.md` · `MOUNTAINS_PASSES_AND_TERRAIN_AUTHORITY.md`.
- **Label authority + image prompts:** `04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` + `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` (player-safe label rules; copy into image prompts).
- **A region map:** `04_world_atlas/region_map_packets/REGION_[NAME].md` (local grid, terrain/water/routes/settlements/dungeons, player-safe vs DM-only layers).
- **A city map:** `06_settlements/city_map_packets/[CITY]_CITY_MAP.md` (Caradril / Glassmere / Calderport / Ashfast — districts, bridges, road exits, landmarks).
- **A settlement map:** `06_settlements/settlement_map_packets/SETTLEMENT_[NAME]_MAP.md`.
- **Placing an adventure site:** `10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` (D01–D36 coords + surface markers + player/DM visibility).
- **DM-only / NEVER on player maps:** the Concord Deep, the Under-Shrine / Drowned Keystone, the Hollow Court seat, node-network links, and D23. The endgame is **vertical beneath Hollowmere**, never a distant land. Far ruins are surface/echo only, drawn unexplained.

### Entering a dungeon or adventure site
- `10_dungeons_and_ruins/DUNGEON_INDEX.md` and/or `10_dungeons_and_ruins/RUIN_INDEX.md` to locate the file
- The specific dungeon/ruin file
- `13_encounters_and_bestiary/DUNGEON_ENCOUNTER_SUPPORT.md` + the regional encounter table
- `13_encounters_and_bestiary/BESTIARY_INDEX.md` → adversary stat profiles for occupants
- `14_treasure_and_artifacts/DUNGEON_REWARD_INDEX.md` for the site's treasure
- `11_mysteries_and_secrets/CLUE_INDEX.md` (DM-only) for clues placed here
- `13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md` if scaling is needed

### Handling a faction action or faction clock
- `07_factions/FACTION_INDEX.md` — master table
- `07_factions/FACTION_TURN_RULES.md` — **load between sessions / at any time-skip** to make factions act off-screen
- `07_factions/FACTION_RELATIONSHIP_MAP.md` — load when an action ripples across factions
- `02_runtime_state/FACTION_STATE.md` + `02_runtime_state/WORLD_CLOCKS.md` — current positions and clocks
- The specific faction file in `07_factions/major_factions/`
- `15_campaign_arcs/FACTION_ESCALATION_PATHS.md` for L5+ faction arcs
- `13_encounters_and_bestiary/FACTION_ENCOUNTERS.md` if confrontation turns to combat

### Resolving a quest
- `09_quests/QUEST_INDEX.md` — locate the quest
- The specific quest file (`09_quests/.../Q_*.md`) or `09_quests/MAJOR_CAMPAIGN_QUESTS.md` / `09_quests/DEVELOPED_QUESTS_INDEX.md`
- `09_quests/HOOKS_JOBS_RUMORS_INDEX.md` for follow-up hooks
- `14_treasure_and_artifacts/QUEST_REWARD_INDEX.md` for the reward
- `01_runner_protocol/FAILURE_AND_CONSEQUENCES.md` on failure/partial success
- Update `02_runtime_state/ACTIVE_QUESTS.md`, `OPEN_THREADS.md`, `CONSEQUENCES.md` per the quest's State Updates section

### Delivering a clue or revelation
- `11_mysteries_and_secrets/CLUE_INDEX.md` — the clue's text, location, method (DM-only)
- `11_mysteries_and_secrets/REVELATION_MAP.md` + `11_mysteries_and_secrets/REVEAL_TIMING.md` — what may be revealed at this stage
- `11_mysteries_and_secrets/DISCOVERY_PATHS.md` — the multiple clue paths to each conclusion
- `11_mysteries_and_secrets/SECRET_PROTECTION_MATRIX.md` — what must stay hidden and why
- `11_mysteries_and_secrets/SECRET_INDEX.md` — the full secret ledger (DM-only)
- `02_runtime_state/KNOWN_CLUES.md` / `HIDDEN_CLUES.md` — what the player actually knows
- `01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md` + `SECRET_REVEAL_PROTOCOL.md`

### Using encounters / bestiary
- `13_encounters_and_bestiary/ENCOUNTER_INDEX.md` — master encounter lookup
- `13_encounters_and_bestiary/BESTIARY_INDEX.md` — adversary/creature stat profiles
- `13_encounters_and_bestiary/REGIONAL_ENCOUNTER_TABLES.md` + the specific region table
- `13_encounters_and_bestiary/TRAVEL_ENCOUNTERS.md` for road/wilderness
- `13_encounters_and_bestiary/DUNGEON_ENCOUNTER_SUPPORT.md` inside sites
- `13_encounters_and_bestiary/SOLO_ENCOUNTER_SCALING.md` — always check solo danger and scaling
- `01_runner_protocol/COMBAT_PROTOCOL.md`

### Giving treasure / rewards / artifacts
- `14_treasure_and_artifacts/TREASURE_INDEX.md` — master treasure lookup
- `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` — tier-by-tier reward feel + forwarding index
- `14_treasure_and_artifacts/SOLO_REWARD_BALANCE.md` — solo balance guardrails
- `14_treasure_and_artifacts/MAGIC_ITEM_INDEX.md` / `REGIONAL_TREASURE_TABLES.md` / `QUEST_REWARD_INDEX.md` / `DUNGEON_REWARD_INDEX.md`
- `14_treasure_and_artifacts/ARTIFACT_INDEX.md` — major relics/artifacts (gating is defined here; DM-only artifacts are M6–M9 gated)

### Reaching level 5 (Tier 2 entry)
- `15_campaign_arcs/LEVEL_5_TO_20_OVERVIEW.md`
- `15_campaign_arcs/TIER_2_LEVELS_5_10.md` + `15_campaign_arcs/TIER_2_PLAYABLE_PATHS_LEVELS_5_10.md`
- `15_campaign_arcs/ACT_2_LEVELS_5_8.md`
- `15_campaign_arcs/LEVELING_AND_MILESTONE_GUIDE.md`
- `15_campaign_arcs/REGIONAL_ARC_PACKS_LEVEL_5_TO_20.md` + `15_campaign_arcs/FACTION_ESCALATION_PATHS.md`
- `11_mysteries_and_secrets/REVEAL_TIMING.md` — reveal cap rises to R2 at L5+

### Reaching level 11 (Tier 3 entry)
- `15_campaign_arcs/TIER_3_LEVELS_11_16.md` + `15_campaign_arcs/TIER_3_PLAYABLE_PATHS_LEVELS_11_16.md`
- `15_campaign_arcs/ACT_3_LEVELS_9_12.md` + `15_campaign_arcs/ACT_4_LEVELS_13_16.md`
- `15_campaign_arcs/VILLAIN_AND_APEX_THREAT_ESCALATION.md` (+ `VILLAIN_ESCALATION.md`)
- `15_campaign_arcs/MAIN_ARC_REVELATION_SEQUENCE.md`
- `13_encounters_and_bestiary/BOSS_AND_APEX_THREATS.md`

### Reaching level 17 (Tier 4 / endgame entry)
- `15_campaign_arcs/TIER_4_LEVELS_17_20.md` + `15_campaign_arcs/TIER_4_PLAYABLE_PATHS_LEVELS_17_20.md`
- `15_campaign_arcs/ACT_5_LEVELS_17_20.md`
- `15_campaign_arcs/ENDGAME_STRUCTURE.md` + `15_campaign_arcs/ENDGAME_STATES.md`
- `15_campaign_arcs/FINAL_REVELATION_AND_ENDING_PATHS.md`
- `15_campaign_arcs/ENDGAME_REGION_PLAYBOOK.md`
- `14_treasure_and_artifacts/ARTIFACT_INDEX.md` — endgame artifact gating (Harvest Engine Shard, Quiet Country Vessel)

### Handling off-route travel
- `15_campaign_arcs/PLAYER_GOES_ANYWHERE_GUIDE.md`
- `15_campaign_arcs/REGION_TO_REGION_TRANSITION_GUIDE.md`
- `04_world_atlas/TRAVEL_ROUTES_RING1.md` (Ring 1) or `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` (far)
- `01_runner_protocol/TRAVEL_PROTOCOL.md`
- `13_encounters_and_bestiary/TRAVEL_ENCOUNTERS.md`
- `15_campaign_arcs/OPEN_WORLD_CONTINUITY_GUIDE.md`

### Handling the player ignoring the main arc
- `15_campaign_arcs/PLAYER_IGNORES_MAIN_ARC_GUIDE.md`
- `15_campaign_arcs/CAMPAIGN_ESCALATION_TIMELINE.md` + `15_campaign_arcs/CONTINENTAL_PRESSURE_TIMELINE.md`
- `15_campaign_arcs/FAILURE_STATES_AND_WORLD_CONSEQUENCES.md`
- `07_factions/FACTION_TURN_RULES.md` — factions advance their clocks regardless
- `02_runtime_state/WORLD_CLOCKS.md`

### Handling endgame content
- `15_campaign_arcs/ENDGAME_STRUCTURE.md` + `ENDGAME_STATES.md` + `ENDGAME_REGION_PLAYBOOK.md`
- `15_campaign_arcs/FINAL_REVELATION_AND_ENDING_PATHS.md`
- `15_campaign_arcs/VILLAIN_AND_APEX_THREAT_ESCALATION.md`
- `03_canon/DM_ONLY_CANON.md` — the full hidden truth (only now fully surfaced through play)
- `13_encounters_and_bestiary/BOSS_AND_APEX_THREATS.md`
- `10_dungeons_and_ruins/THE_UNDER_SHRINE_APPROACH.md` + `THE_BASIN_KEYSTONE_APPROACH.md`

---

## Pre-Content-Generation Checks

Before improvising or creating any major new content during play (NPCs, factions, regions, quests, mysteries, monsters, artifacts), check these first:

| File | What To Check |
|---|---|
| `00_control/CANON_AUTHORITY.md` | Which file wins if there's a contradiction |
| `00_control/GENERATION_GUARDRAILS.md` | Drift prevention — does this fit the project? |
| `00_control/NAMING_REGISTRY.md` | Is this name already taken or forbidden? |
| `00_control/RULESET_ASSUMPTIONS.md` | Are mechanics consistent with D&D 5e / 2024? |
| `00_control/DND_MECHANICS_REQUIREMENTS.md` | Does this meet mechanical completeness requirements? |
| `03_canon/CANON.md` | Does this contradict established canon? |

The AI DM should improvise only connective tissue (descriptions, dialogue, minor incidental NPCs, weather, local color, logical consequences). Major content already exists — find it before inventing.

---

## File Priority Levels

| Priority | Meaning | Examples |
|---|---|---|
| Always load | Required for any session | CURRENT_STATE, PLAYER_CHARACTER, CURRENT_LOCATION |
| Load on demand | Load when relevant | NPC files, quest files, dungeon files, region files |
| Load for secrets | DM-only; never surface to player | DM_ONLY_CANON, HIDDEN_CLUES, SECRET_INDEX, mystery files |
| Reference only | Load to check standards, not during play | Standards files, AUDIT_STANDARDS |

---

## Secrecy Enforcement

**Never load DM-only files and then summarize their contents to the player.**

- `secrecy: dm-only` files are for AI DM reasoning only.
- `secrecy: player-safe` files can be paraphrased, quoted, or described to the player.
- `secrecy: dm-facing-player-safe-output` files describe what to *omit* from player output (e.g. map-render manifests) — they are NOT themselves safe to share directly.
- `secrecy: mixed` files require care — read the individual sections before using.

**Apex secrets that must never be surfaced until earned in play:** the Hollow Court's true identity (surviving Custodians), the harvest, the Under-Shrine / Drowned Keystone, the Concord Deep. The reveal schedule is in `11_mysteries_and_secrets/REVEAL_TIMING.md` and `SECRET_PROTECTION_MATRIX.md`.

---

## Region-Specific Load Notes

### Sundering Reach (starting region, L1–6)
Region: `05_regions/SUNDERING_REACH.md`. Settlements: Hollowmere (start), Kettle Bridge, Saltmargin, Candlewick, Greywater Holm, Harrowgast, Reedford, The Ashwalk Rest (solo-safety sanctuary). Wilderness: `05_regions/wilderness/` (Greyfens, Sunder Heights, Mirewend/roads, basin shore). Dungeons: Peat Chapel (L1–2 first delve), Sunken Tollhouse (L2–3), Whispering Cairn (Script gate), Ledger Vault (heist), Barrow of Nine Doors (parley-boss), Deep Adit (L4–6, thin-touch). Encounters: `13_encounters_and_bestiary/SUNDERING_REACH_ENCOUNTERS.md`.

### Caradril (first major city, ~L5–12 with L3–5 on-ramps)
Overview: `06_settlements/CARADRIL.md`. Districts: `06_settlements/caradril_districts/`. City quests: `09_quests/city_quests/`. Encounters: `CARADRIL_ENCOUNTERS.md`. **Never name the Hollow Court (M7) in Caradril; the Sealed Archive (M6/M9) is Act 3 / L9–12.**

### Ring 1 (Ashgarden Vale S / Tollwood E / Pale Coast W, L1–7)
Each has an *honest window* (Tilbrook / Coldhearth-Sennet / Cobble Strand-Bryd) confirming the failures spread outward from the Reach (M5). Gated apex sites (Old Mast, Skerry Shrine, deep Saint Veddow's/Drowned Lamp) give fragments and danger only. **Never name the Hollow Court or the harvest mechanism in Ring 1.** Reveal caps: R1 at Act-1 levels, R2 at L5+, never R3+ in Ring 1.

### Far continent (Orrun, 5 built + 13 placeholder regions, L6–17)
Load `04_world_atlas/FULL_WORLD_MAP_AUTHORITY.md` first. Per-region NPC rosters in `08_npcs/by_region/`, encounter tables in `13_encounters_and_bestiary/`, far adventure sites in `10_dungeons_and_ruins/`. No far NPC knows the apex truth. Endgame never relocates from Hollowmere.

---

## Related Files

- [`CONTENT_INDEX.md`](CONTENT_INDEX.md)
- [`TAG_INDEX.md`](TAG_INDEX.md)
- [`MANIFEST.md`](MANIFEST.md)
- [`01_runner_protocol/AI_DM_CORE_RULES.md`](../01_runner_protocol/AI_DM_CORE_RULES.md)
- [`16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`](../16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md)
- [`16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`](../16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md)
