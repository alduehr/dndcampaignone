# PROGRESS_LOG.md

## Purpose

Chronological record of all meaningful production passes. This is the project history.

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
