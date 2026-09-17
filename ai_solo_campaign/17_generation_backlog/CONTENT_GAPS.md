# CONTENT_GAPS.md

## Purpose

Track missing or underdeveloped content by category. Use this for category-level gaps. Use `TODO.md` for actionable tasks. Use `CONSISTENCY_AUDIT.md` for defects or contradictions.

## Current Status

**Stages 0–16 complete (Stage 16 Pre-Play Readiness Audit: 2026-06-15; verdict READY FOR LIVE PLAY). Stage 17 (Live Campaign Operation) is next, awaiting the user to begin play.** Stage 16 confirmed the campaign is fully runnable 1–20 with no blockers (0 Critical/0 High/2 Medium fixed/4 Low). The **only remaining content gaps are non-blocking/optional**: (1) **far-region settlement deep-builds** — narrowed 2026-07-07: all 12 far regions now have canonical `05_regions/` region files (Phase 5 consolidation) and Caradril is inside its NPC target band; what stays light is the far **settlement** layer (`06_settlements/` files — the eagle-test map packets carry it; deepen per region when play approaches); (2) **map images** not yet generated (prompts/manifests ready). ~~(3) `/15_random_tables/` unpopulated~~ — **closed 2026-07-07** (5 table files + README built). ~~(4) RtHW bestiary integration pending~~ — **closed 2026-07-07** (book verified real and integrated Track-A; every bestiary source attribution re-verified against the published books; unverifiable placeholders removed; all Track-B originals anchored to official chassis). None blocks play. Stage 15B before it added a concrete play-layer over the Stage 15 frameworks (12 files + 6 stubs in `15_campaign_arcs/`); Stage 15 closed the Campaign Arc gaps (15 framework files).**

**(Historical:) Stages 0–11 complete (Stage 11 Mystery/Secret/Clue Expansion: 2026-06-13).** Stage 11 added a full mystery infrastructure: 10 mapped revelations (each with 3–8 independent clue sources), an expanded CLUE_INDEX (~100 clues), 6 regional clue trail files, a FACTION_KNOWLEDGE_MAP covering all 7 factions, an NPC_KNOWLEDGE_MAP (~60 entries), 9 false leads, 10 discovery paths, a SECRET_PROTECTION_MATRIX (DM-only), a MYSTERY_STATE_TRACKER_TEMPLATE, and a Stage 11 secrecy audit (0 Critical / 0 High). Stage 10 quest–clue cross-links added to MAJOR_CAMPAIGN_QUESTS.md.

Earlier stages: Stage 10 (Quest Library Expansion) added 28 major campaign quests, ~165 developed quests, 304 short-form hooks/rumors/jobs. Stage 9/9.5 built the NPC codex to 94 major / 368 secondary / 953 minor. Stages 7/8 built Ring 1 regions and made all 7 factions operational. Stages 0–6 established foundation, AI runtime, starting region, first major city (Caradril), and Level 1–4 arc.

**Stage 12 (Dungeons, Ruins, Adventure Sites) complete (2026-06-13):** master `DUNGEON_INDEX.md` (23 sites) + `PUZZLE_DUNGEONS.md`; the 15 existing dungeons cross-linked to the Stage 11 REV/clue layer; 8 new sites (incl. the keystone approach, the Caradril deep-dungeon, two far high-tier sites, and the DM-only endgame); `STAGE_12_ADVERSARIES.md`.

**Stage 13 (Encounter and Bestiary Expansion) complete (2026-06-14):** 28 newly generated Stage 13 files (35 total .md files in `13_encounters_and_bestiary/` including README, the 5 pre-existing Ring 0/1/Caradril encounter files, STAGE_12_ADVERSARIES.md, and ACT_1_THREATS.md) — master encounter index, bestiary index (17 creature categories), copyright-safe source reference, solo scaling rules, 15-biome matrix, 18 tiered bosses, original Remembrance horror/curse bestiary, faction/mystery/travel/dungeon encounter support, and a dedicated encounter file for all 20 regions of Orrun. All 5 level-bands (1–20) covered. Official monsters source-referenced (never stat-block-copied). No new factions/NPCs/regions/mysteries/gods/artifacts; apex truth DM-only/gated. **Stage 14 (Treasure, Artifacts, and Rewards) complete 2026-06-14 — see status block above.**

**Stage 12.5 (Continental Adventure-Site Coverage) complete (2026-06-14):** 13 new far-continent adventure sites (D24–D36) bringing the total to **36 sites**, so **every map-authoritative far-continent region now has ≥1 authored explorable site** (Glassmere and Emberfell have 2). The four previously-deferred optional sites (Saltmere/Hethewald/Marrowdowns/Karran) are built. 13 new far corroboration/echo clue IDs added to `CLUE_INDEX.md` (all surface/echo, never the keystone/Court). All dungeon indexes + tracking files updated. **No new mystery/faction/god/cosmology/artifact; no apex truth in any player-safe section.**

> **Update (Stage 16 correction pass, 2026-06-16):** The "treasure-by-level" and "Acts 2–5" gaps once referenced here are now **closed**. `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` exists (the by-level forwarding index over the full Stage 14 treasure library), and Acts 2–5 / Tiers 2–4 are built in `15_campaign_arcs/`. The pre-play readiness audit is complete (`18_audits/PRE_PLAY_READINESS_AUDIT.md`). **Only optional/non-blocking gaps remain for live play:** far-continent region/settlement deep-builds (arc packs + rosters + dungeons already exist), map-image generation, the deferred `/15_random_tables/`, and the pending RtHW bestiary integration. None blocks starting the campaign.

Targets are drawn from `DEVELOPMENT_STAGES.md`, `PROJECT_RULES.md` content-scale targets, and `WORLDBUILDING_STANDARDS.md` density guidelines.

---

## Regions

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~Starting region exists as a frame only~~ — **deep-built in Stage 3** (8 settlements, 4 wilderness zones, 6 dungeons, encounter/rumor tables, 12 developed quests) | — (no gap) | — | — | done in Stage 3 |
| ~~No adjacent (Ring 1) regions~~ — **deep-built in Stage 7**: Ashgarden Vale (3 settlements, 3 dungeons, 8 quests), Tollwood (3 settlements, 3 dungeons, 7 quests), Pale Coast (2 settlements, 3 dungeons, 5 quests), travel routes | — (no gap) | — | — | done in Stage 7 |
| ~~Distant named regions are world-overview stubs only~~ — **Full-World Cartographic Expansion** named/positioned the whole continent: 13 placeholder regions with political form + 1-line identity, all continental water/terrain features, 3 overseas Vael landmasses | Low (cartography done; deep builds pending) | Long-term travel and high-tier play | Deep-build individual regions as the arc reaches them; placeholders in `FULL_WORLD_MAP_AUTHORITY.md`/`REGION_INDEX.md` | 15+ |
| ~~12 far-continent regions map-authoritative only~~ — **narrowed 2026-07-07 (Phase 5):** all 12 have canonical `05_regions/` region files consolidating the authored layers. Remaining light: far **settlement** files (map packets carry them), deep Sunder Heights, optional Highmark Passes | Low (was Medium) | Play-driven deepening past the region-file layer | Deepen a specific region's settlements when play approaches it | future (play-driven) |
| Overseas Vael landmasses (Surren, Iron Skards, Sundered Isles) are 1-line placeholders | Low | Possible far-future overseas play | Develop only if the campaign ever leaves Orrun (not arc-required) | far-future |
| Map images not yet generated (authority files now complete) | Low | Player-facing & DM visual reference | **Cartography Authority Pass (2026-06-16) made the repo cartography-deterministic** — continent/region/city/settlement/route/water/terrain/dungeon geometry is now coordinate-anchored (`CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`, `MAP_FEATURE_REGISTRY.md`, region/city/settlement packets, `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`). Remaining gap is only the *rendering*: generate images from `FULL_WORLD_MAP_PROMPTS.md` Prompt 5 → 1 → 3, then per-region/city packets. | interstitial |
| Low-confidence map coordinates (far-continent) | Low | Map self-consistency | Now catalogued with explicit confidence in `MAP_FEATURE_REGISTRY.md` (HIGH/MEDIUM/LOW/DERIVED). Far-continent geometry is intentionally LOW/placeholder and improv-safe; upgrade as placeholder regions are deep-built. Non-blocking per `18_audits/CARTOGRAPHY_READINESS_AUDIT.md`. | ongoing |
| Far-continent internal/city geometry is light-anchor / placeholder | Low | Far-region maps | The 3 far cities (Glassmere/Calderport/Ashfast) have canonical-enough layouts to map but are not deep-built; far settlements are light anchors. Deep-build when play warrants. | future (Ring 2+ / continental) |

---

## Settlements

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~No additional regional towns/villages~~ — **7 added in Stage 3 (8 total)**: Kettle Bridge, Saltmargin, Candlewick, Greywater Holm, Harrowgast, Reedford, The Ashwalk Rest | — (no gap) | — | — | done in Stage 3 |
| ~~No major city~~ — **Caradril deep-built in Stage 4** (city overview + 8 districts, government, services, criminal networks, city NPCs/quests/clocks) | — (no gap) | — | — | done in Stage 4 |
| ~~Caradril's Sunken Wards lacks a full room-by-room dungeon file~~ — **built in Stage 12** (`THE_SUNKEN_WARDS_DEEP.md`). The Sealed Archive's *back-route* is built; a dedicated Archive room-by-room file is optional polish (see Dungeons section) | — (mostly resolved) | Deep city delve | done in Stage 12 (Archive file optional) | 12 |
| ~~Tollreach (Hethewald; Greenfinger Maddoc's outlaw camp) lacks a standalone settlement packet~~ — **RESOLVED 2026-06-18 (Cartography Determinism Cleanup):** Tollreach is formalized as a **route-waypoint danger marker** at (75,37) on the Hethe Tollway in `ROADS_RIVERS_AND_ROUTES_AUTHORITY.md` and `MAP_FEATURE_REGISTRY.md` (MF-612, reclassified to a danger marker). It is a dangerous outlaw camp, not a service settlement; the AI DM runs an encounter/parley, not an arrival scene; Hethemoot provides regional services. No packet needed. | — (resolved) | — | — | resolved 2026-06-18 |

---

## Factions

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| Seven major factions exist with public face, hidden agenda, leader, members, resources, and a clock each | — (no gap) | — | — | done in Stage 1 |
| ~~Faction quest chains are not yet fully built out (intro → trust → complication → decision point)~~ — **built in Stage 8: all 7 factions have 4-quest chains** in `09_quests/faction_quests/[FACTION]/` (28 quests + 7 chain indexes) | — (no gap) | — | — | done in Stage 8 |
| ~~Factions lack rank-and-file combat profiles / "Combat Capability" sections~~ — **added in Stage 8** to all 7 faction files | — (no gap) | — | — | done in Stage 8 |
| ~~No full pairwise faction relationship map / no between-session faction-turn rules~~ — **`FACTION_RELATIONSHIP_MAP.md` + `FACTION_TURN_RULES.md` created in Stage 8** | — (no gap) | — | — | done in Stage 8 |
| ~~Secondary/minor faction members lack full entries~~ — **all five registered placeholders + ~16 more secondary faction agents created in Stage 3** | — (no gap for the registered set) | — | — | done in Stage 3 |
| No minor/local factions | Low | Texture in settlements and wilderness | Add minor factions during regional builds | 7+ |

---

## NPCs

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| 20 major NPCs exist with secrets and motivations | — (no gap) | — | — | done in Stage 1 |
| ~~Major NPC count below long-term target (50–100)~~ — **resolved in Stage 9/9.5: 94 major NPCs** (50 core + 44 far-continent) — meets the 50–100 target | — (no gap) | — | — | done in Stage 9/9.5 |
| ~~Secondary NPCs below target~~ — **resolved in Stage 9/9.5: 368 secondary NPCs** (within the 200–500 target) | — (no gap) | — | — | done in Stage 9/9.5 |
| ~~Minor named NPCs below target~~ — **resolved in Stage 9/9.5: 953 minor NPCs** (exceeds the 500+ target) | — (no gap) | — | — | done in Stage 9/9.5 |
| ~~Ring 1 NPC density below per-region target~~ — **resolved in Stage 9/9.5** Ring 1 rosters expanded as part of the 368 secondary / 953 minor codex build | — (no gap) | — | — | done in Stage 9/9.5 |
| ~~`NPC_RELATIONSHIP_WEB.md`, `NPC_SECRET_LEDGER.md`, `NPC_VOICE_GUIDE.md` not created~~ — **created in Stage 9** | — (no gap) | — | — | done in Stage 9 |

---

## Quests

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| 10 session hooks + 20 rumors exist (Act 1) | — (no gap) | — | — | done in Stage 1 |
| Developed quest files: **12 (Stage 3) + 11 (Stage 4) + 6 (Stage 5 Act 1) + 24 (Stage 7 Ring 1) + 28 (Stage 8 faction chains) = ~81** (within 75–150 target); region/city/Act-1/faction coverage good | Low | Continue toward upper target with regional/personal quests | Stage 10 quest-library expansion | 10 |
| ~~No fully shaped main-arc Act 1 quest line (level 1–4)~~ — **Act 1 play kit built in Stage 5** (arc spine, 6 faction quests, threats, clue trails, failure states, milestones, NPC guide) | — (no gap) | — | — | done in Stage 5 |
| Hook/rumor library: **39 hooks + 50 rumors** after Stage 3 (toward 300–600 target) | Medium | Continue toward target with each region/city | Expand hook/rumor library | 10 |
| ~~Failure states not yet attached to developed quests~~ — **every Stage 3/4/5 quest now has a Failure State + State Updates; Stage 5 added a dedicated `ACT_1_FAILURE_STATES.md` redirect playbook** | — (no gap for Act 1) | — | — | done through Stage 5 |

---

## Mysteries and Clues

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| Mystery web (M0–M10), revelation map (R1–R8), and 20-secret index exist with 3+ clue paths each | — (no gap) | — | — | done in Stage 1 |
| `CLUE_INDEX.md` and `HIDDEN_CLUES.md` populated from the mystery web (this pass) | — (no gap) | — | — | done in this pass |
| Individual per-clue files not created (clues currently tracked in index rows only) | Low | Finer-grained retrieval if needed later | Create individual clue files if play demands | 11 |
| `FALSE_LEADS.md`, `PROPHECIES_AND_OMENS.md`, `MYSTERY_CHAINS.md`, `REVEAL_TIMING.md` not created | Low | Deeper mystery infrastructure | Create during mystery expansion | 11 |

---

## Dungeons and Ruins

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~Keystone dungeon referenced but not built~~ — **built in Stage 12**: `THE_BASIN_KEYSTONE_APPROACH` (upper works, L5-9; apex gated) + `THE_UNDER_SHRINE_APPROACH` (DM-only endgame, L16-20) | — (no gap) | — | — | done in Stage 12 |
| ~~No master dungeon index~~ — **built in Stage 12**: `DUNGEON_INDEX.md` (23 sites) + `PUZZLE_DUNGEONS.md` | — (no gap) | — | — | done in Stage 12 |
| ~~No regional dungeons/ruins~~ — **6 built in Stage 3** (Peat Chapel, Sunken Tollhouse, Whispering Cairn, Ledger Vault, Barrow of Nine Doors, Deep Adit) + 9 Ring-1 (Stage 7) + 5 new in Stage 12 (Sunken Wards Deep, Ashmarket Undercroft, Concord Relay-Vault, Greyfens Deep, + the keystone approach) | — (no gap) | — | — | done in Stages 3/7/12 (target met) |
| First major Act 1 dungeon: **Act 1 routes its dungeon beats through the 6 Stage 3 Concord sites** (sufficient for play); an optional dedicated Act 1 climax dungeon could sharpen the L3→4 beat | Low (was High) | Level 1–4 arc climax site | Optional purpose-built Act 1 dungeon | 5 (optional) / 12 |
| ~~Optional far-continent dungeons named but not built (Saltmere Deep Towns, Hethewald Old Holds, Marrowdowns Barrow Complex, Karran Old Iron Forts)~~ — **all 4 built in Stage 12.5** (D24–D27), plus **9 more far sites** so every map-authoritative far region has ≥1 authored site (Glassmere ×2, Sallowmarch, Hollow Gulf, Wender Steppe, Sunmark, Verdance Reaches Ring-2, Highmark Passes, Emberfell 2nd) | — (no gap) | — | — | done in Stage 12.5 |
| Sealed Archive (Caradril) lacks a dedicated room-by-room file (the *back-route into it* is built via `THE_SUNKEN_WARDS_DEEP`; the Archive itself is specced as Lantern Reach district/quest content) | Low | Deep Act-3 city delve polish | Optional dedicated Archive dungeon file | 12 (optional) / 15 |
| ~~Pre-existing D-site numbering discrepancy in far packets~~ — **RESOLVED 2026-06-18 (Cartography Determinism Cleanup):** all region-packet D-site IDs corrected to match the authoritative `ADVENTURE_SITE_CARTOGRAPHY_INDEX.md` — REGION_MARROWDOWNS D30→**D26** (Barrow Complex); REGION_SALLOWMARCH D33→**D30** (Drowned Steps); REGION_HOLLOW_GULF_PORTS Drowned-Steps D33→**D30**; REGION_WENDER_STEPPE table D25→**D32** (Sky-Stones). Settlement packets (Marrowmoot/Fenward/Reedmouth) already used correct IDs. All region/settlement/index D-site IDs now consistent. | — (resolved) | — | — | resolved 2026-06-18 |

---

## Encounters and Bestiary

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~No regional encounter tables~~ — **4 solo-tuned zone tables built in Stage 3** (Roads/River, Greyfens, Heights, Basin), stat-referenced | — (no gap for the starting region) | — | Build city/other-region tables later | done in Stage 3 |
| ~~No standalone full bestiary~~ — **built in Stage 13** (`BESTIARY_INDEX.md`, 17 creature categories; `HORROR_AND_CURSE_THREATS.md` original undead/curses; `STAGE_12_ADVERSARIES.md` dungeon originals; source-referenced officials) | — (no gap) | — | — | done in Stage 13 |
| ~~No mid/high-tier villain/boss profiles~~ — **built in Stage 13** (`BOSS_AND_APEX_THREATS.md`, 18 bosses B1–B18 across all tiers; recurring-villain escape/return logic; Custodian apex DM-only/gated) | — (no gap) | — | — | done in Stage 13 |
| ~~No all-region encounter coverage~~ — **built in Stage 13** (all 20 regions have encounter files; `TRAVEL_ENCOUNTERS.md` covers all 5 level-bands; `BIOME_ENCOUNTER_MATRIX.md`, `FACTION_ENCOUNTERS.md`, `MYSTERY_ENCOUNTERS.md`, `DUNGEON_ENCOUNTER_SUPPORT.md`) | — (no gap) | — | — | done in Stage 13 |
| Noncombat obstacle coverage: each region file's "Noncombat Encounters" + `TRAVEL_ENCOUNTERS` variants + `SOLO_ENCOUNTER_SCALING` cover non-fight challenges; no single dedicated NONCOMBAT_OBSTACLES library file (folded into the region/travel files instead) | Low | Solo-friendly non-fight challenges | Optional: consolidate a standalone obstacle library if desired | 13 (folded) / optional |

---

## Treasure and Artifacts

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~No treasure-by-level guidance or magic-item list~~ — **done Stage 14 (2026-06-14):** `SOLO_REWARD_BALANCE.md` + `REGIONAL_TREASURE_TABLES.md` (20 regions × 5 bands) + `MAGIC_ITEM_INDEX.md` (38 items) | — (no gap) | — | — | done in Stage 14 |
| ~~Remembrance relics referenced in lore but not statted as items~~ — **done Stage 14:** `ARTIFACT_INDEX.md` (12 named relics, mystery-gated), `CURSED_ITEMS.md` (10), `SENTIENT_ITEMS.md` (6) — all tie to M1–M9 without spoiling the apex | — (no gap) | — | — | done in Stage 14 |
| ~~Endgame-artifact mechanics intentionally light (Quiet Country Vessel, Harvest Engine Shard, Last Voice)~~ — **done Stage 15:** endgame artifact gating + playbooks built (`ENDGAME_STRUCTURE.md`, `TIER_4_PLAYABLE_PATHS_LEVELS_17_20.md`); `ARTIFACT_INDEX.md` defines M6–M9 gates; `REWARDS_BY_LEVEL.md` forwards by tier | — (no gap) | — | — | done in Stage 15 |
| RtHW (verified real, integrated in the bestiary 2026-07-07) horror-**item** references not yet added | Low | Optional extra cursed/relic Track-A refs (the 2026-07-07 pass covered *creatures* only; the book's 2 magic items were not evaluated) | Add 1–2 item references if a future pass verifies them in print | future |

---

## AI Runtime

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| All 17 runner protocols, START/RESUME prompts, session-pack templates exist and are complete | — (no gap) | — | — | done in Stage 2 |
| 8 runtime state files seeded; clue state files populated this pass; play-only state files at empty baseline by design | — (no gap) | — | — | done in Stage 2 / this pass |
| `PLAYER_CHARACTER.md` is a scaffold awaiting character creation | Low (by design) | Filled at session 1 | Populate at character creation | 17 |
| No random tables (travel/weather/event/wilderness) | Low | Reduce improvisation during travel/downtime | Populate `/15_random_tables/` | 3+ |

---

## Campaign Arc

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| Main arc overview and level 1–20 progression exist (shape + Act 1 concrete) | — (no gap) | — | — | done in Stage 1 |
| ~~Act 1 (levels 1–4) not fully shaped~~ — **Act 1 play kit built in Stage 5** (`ACT_1_LEVELS_1_4.md` + milestones + failure states + threats + clue trails + NPC guide + 6 faction quests) | — (no gap) | — | — | done in Stage 5 |
| ~~No standalone act files for Acts 2–5 (levels 5–20)~~ — **done Stage 15 (2026-06-15):** built `15_campaign_arcs/TIER_2_LEVELS_5_10.md` (Act 2 + lower Act 3), `TIER_3_LEVELS_11_16.md` (Act 3 upper + Act 4), `TIER_4_LEVELS_17_20.md` (Act 5) + `LEVEL_5_TO_20_OVERVIEW.md` (tier↔act crosswalk) | — (no gap) | — | — | done in Stage 15 |
| ~~No standalone villain-escalation / endgame-states files~~ — **done Stage 15:** `VILLAIN_AND_APEX_THREAT_ESCALATION.md` (escalation by revelation; Veyl as choice-boss) + `ENDGAME_STRUCTURE.md` (9 approaches × 5 outcomes) + `FAILURE_STATES_AND_WORLD_CONSEQUENCES.md` + `CAMPAIGN_ESCALATION_TIMELINE.md` | — (no gap) | — | — | done in Stage 15 |
| ~~Stage 15 frameworks were reference-only ("see file X"), not concrete per-region/tier playable content~~ — **done Stage 15B (2026-06-15):** `REGIONAL_ARC_PACKS_LEVEL_5_TO_20` (19 packs + Cindern Waste), `TIER_3/4_PLAYABLE_PATHS` (6 + 9), `REGION_TO_REGION_TRANSITION_GUIDE`, `CONTINENTAL_PRESSURE_TIMELINE`, `PLAYER_IGNORES_MAIN_ARC_GUIDE`, `PLAYER_GOES_ANYWHERE_GUIDE`, `ENDGAME_REGION_PLAYBOOK`, `FINAL_REVELATION_AND_ENDING_PATHS` | — (no gap) | — | — | done in Stage 15B |
| Far-continent regions have runnable **arc packs** (Stage 15B) + NPC rosters (Stage 9.5) + dungeons (Stage 12.5), but **no full `05_regions/`/`06_settlements/` deep-builds** | Low | Deepening far-continent play beyond arc-pack depth | Optional future stage: deep-build far-region region/settlement files | post-16 (optional) |

---

## Audits

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~No formal AI-readiness audit yet~~ — **Stage 6 first full audit complete (2026-06-10)**; foundation verified sound (0 Critical, 1 High fixed, 4 Medium, 5 Low); scaling to Stage 7 approved | — (no gap) | — | — | done in Stage 6 |
| ~~No pre-play readiness audit~~ — **done Stage 16:** master verdict `18_audits/PRE_PLAY_READINESS_AUDIT.md` + 6 detailed Stage 16 reports; correction pass (2026-06-16) fixed the issues the prior pass overclaimed. Verdict: READY FOR LIVE PLAY | — (no gap) | — | — | done in Stage 16 |

---

## Related Files

- [`../00_control/TODO.md`](../00_control/TODO.md)
- [`../00_control/CONSISTENCY_AUDIT.md`](../00_control/CONSISTENCY_AUDIT.md)
- [`../00_control/DEVELOPMENT_STAGES.md`](../00_control/DEVELOPMENT_STAGES.md)
- [`EXPANSION_PLAN.md`](EXPANSION_PLAN.md)
