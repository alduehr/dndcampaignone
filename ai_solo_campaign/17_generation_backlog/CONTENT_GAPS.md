# CONTENT_GAPS.md

## Purpose

Track missing or underdeveloped content by category. Use this for category-level gaps. Use `TODO.md` for actionable tasks. Use `CONSISTENCY_AUDIT.md` for defects or contradictions.

## Current Status

**Stages 0–7 complete; Full-World Cartographic Expansion pass done.** Stage 7 (Regional Expansion Ring 1) added 3 regions (Ashgarden Vale, Tollwood, Pale Coast), 8 settlements, 3 wilderness files, 9 dungeons, 3 encounter tables, 6 hooks/rumors files, 20 developed quests, ~60 NPCs, and travel routes. The **Full-World Cartographic Expansion pass** then expanded the map from the NW campaign quarter to the **whole continent of Orrun** — 4 new full-continent atlas files, 13 placeholder regions, all continental geographic features, 3 overseas landmasses, 8 map layers, 5 image prompts (cartography only; the new regions are NOT deep-built). The world now opens outward in multiple directions from the Sundering Reach, with the rest of the continent named and positioned as a placeholder horizon.

**Stages 0, 1, 2, 3, 4, and 5 complete.** The campaign foundation + AI runtime exist, the starting region is deep-built, the **first major city (Caradril) is deep-built**, and the **Level 1–4 Act 1 play kit (Stage 5) now exists** (open-world arc spine, 6 faction-alignment quests, 5 recurring early-threat profiles, an existing-clue Act 1 access overlay with R1 cap, 9 failure-redirect states, milestone/XP triggers, and an Act 1 NPC casting guide). The campaign now has a frontier sandbox, a mid-game city hub, and a runnable early-game arc.

**Stage 6 (First Full Audit) complete 2026-06-10** — foundation verified sound; 0 Critical, 1 High (fixed inline), 4 Medium, 5 Low. See `../18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`. The gaps below reflect what remains for **Stage 7+ depth and scale** (faction quest chains, the keystone + Caradril dungeon builds, treasure-by-level, the bestiary, Acts 2–5, adjacent regions). Targets are drawn from `DEVELOPMENT_STAGES.md`, `PROJECT_RULES.md` content-scale targets, and `WORLDBUILDING_STANDARDS.md` density guidelines.

---

## Regions

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~Starting region exists as a frame only~~ — **deep-built in Stage 3** (8 settlements, 4 wilderness zones, 6 dungeons, encounter/rumor tables, 12 developed quests) | — (no gap) | — | — | done in Stage 3 |
| ~~No adjacent (Ring 1) regions~~ — **deep-built in Stage 7**: Ashgarden Vale (3 settlements, 3 dungeons, 8 quests), Tollwood (3 settlements, 3 dungeons, 7 quests), Pale Coast (2 settlements, 3 dungeons, 5 quests), travel routes | — (no gap) | — | — | done in Stage 7 |
| ~~Distant named regions are world-overview stubs only~~ — **Full-World Cartographic Expansion** named/positioned the whole continent: 13 placeholder regions with political form + 1-line identity, all continental water/terrain features, 3 overseas Vael landmasses | Low (cartography done; deep builds pending) | Long-term travel and high-tier play | Deep-build individual regions as the arc reaches them; placeholders in `FULL_WORLD_MAP_AUTHORITY.md`/`REGION_INDEX.md` | 15+ |
| Ring 2 + 13 continental placeholder regions are map-authoritative only (Verdance Reaches, deep Sunder Heights, Highmark passes; Glassmere League, Marrowdowns, Sallowmarch Protectorate, Hollow Gulf Ports, Wender Steppe, Karran Marches, Emberfell Theocracy, Saltmere Reaches, Concord Heartlands, Hethewald Free Holds, Sunmark) | Medium | Midgame/late/continental play past Caradril | Deep-build when play warrants; positions + political form + 1-line identities exist | future (Ring 2+ / continental) |
| Overseas Vael landmasses (Surren, Iron Skards, Sundered Isles) are 1-line placeholders | Low | Possible far-future overseas play | Develop only if the campaign ever leaves Orrun (not arc-required) | far-future |
| Map images not yet generated | Low | Player-facing & DM visual reference | Prompts ready (campaign-area + full-continent); generate `FULL_WORLD_MAP_PROMPTS.md` Prompt 5 then Prompt 1 then Prompt 3 first | interstitial |
| Low-confidence map coordinates (~22 campaign-area + ~86 full-continent) | Low | Map self-consistency | Upgrade to medium/high as the placeholder regions are built | ongoing |

---

## Settlements

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~No additional regional towns/villages~~ — **7 added in Stage 3 (8 total)**: Kettle Bridge, Saltmargin, Candlewick, Greywater Holm, Harrowgast, Reedford, The Ashwalk Rest | — (no gap) | — | — | done in Stage 3 |
| ~~No major city~~ — **Caradril deep-built in Stage 4** (city overview + 8 districts, government, services, criminal networks, city NPCs/quests/clocks) | — (no gap) | — | — | done in Stage 4 |
| Caradril's Sunken Wards + Sealed Archive lack full room-by-room dungeon files (specced as district/quest content only) | Low | Deep delve play in the city | Full dungeon build (mirrors keystone deferral) | 12 |

---

## Factions

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| Seven major factions exist with public face, hidden agenda, leader, members, resources, and a clock each | — (no gap) | — | — | done in Stage 1 |
| Faction quest chains are not yet fully built out (intro → trust → complication → decision point) | Medium | Repeatable faction play and consequences | Build per-faction quest chains | 8, 10 |
| ~~Secondary/minor faction members lack full entries~~ — **all five registered placeholders + ~16 more secondary faction agents created in Stage 3** | — (no gap for the registered set) | — | — | done in Stage 3 |
| No minor/local factions | Low | Texture in settlements and wilderness | Add minor factions during regional builds | 7+ |

---

## NPCs

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| 20 major NPCs exist with secrets and motivations | — (no gap) | — | — | done in Stage 1 |
| Major NPC count below long-term target (50–100) | Medium | Reduce major improvisation across the campaign | Expand major NPC roster | 9 |
| Secondary NPCs: **~21 (Stage 3) + ~15 (Stage 4 city) + 29 (Stage 7 Ring 1) = ~65 secondary NPCs** (toward 200–500 target) | Medium | Continue toward target | Keep generating with each region/city pass | 3✓, 4✓, 7✓, 9 |
| Minor named NPCs: **~35 (Stage 3) + ~25 (Stage 4 city) + 33 (Stage 7 Ring 1) = ~93 minor NPCs** (toward 500+ target) | Medium | Continue toward target | Generate minor NPC tables per area | 3✓, 4✓, 7✓, 9 |
| Ring 1 NPC density below per-region target (30–60 per region; actual ~20 per region across 3 Ring 1 regions) | Medium | Reduce improvisation in Ring 1 settlements and sites | Expand Ring 1 secondary + minor NPCs — prioritize Pale Coast and Tollwood | 9 |
| `NPC_RELATIONSHIP_WEB.md`, `NPC_SECRET_LEDGER.md`, `NPC_VOICE_GUIDE.md` not created | Low | Managing a large NPC population | Create when NPC roster grows | 9 |

---

## Quests

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| 10 session hooks + 20 rumors exist (Act 1) | — (no gap) | — | — | done in Stage 1 |
| Developed quest files: **12 (Stage 3) + 11 (Stage 4) + 6 (Stage 5 Act 1) = ~29** (toward 75–150 target); region/city/Act-1 coverage good | Medium | Continue toward target; add faction quest chains | Build per-faction quest chains | 8, 10 |
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
| Keystone dungeon referenced but not built | High | The campaign's central adventure site | Full dungeon build with solo-safety valves and scaling | 12 |
| ~~No regional dungeons/ruins~~ — **6 built in Stage 3** (Peat Chapel, Sunken Tollhouse, Whispering Cairn, Ledger Vault, Barrow of Nine Doors, Deep Adit), full mechanics | — (no gap) | — | — | done in Stage 3 (target 5–8 met) |
| First major Act 1 dungeon: **Act 1 routes its dungeon beats through the 6 Stage 3 Concord sites** (sufficient for play); an optional dedicated Act 1 climax dungeon could sharpen the L3→4 beat | Low (was High) | Level 1–4 arc climax site | Optional purpose-built Act 1 dungeon | 5 (optional) / 12 |

---

## Encounters and Bestiary

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~No regional encounter tables~~ — **4 solo-tuned zone tables built in Stage 3** (Roads/River, Greyfens, Heights, Basin), stat-referenced | — (no gap for the starting region) | — | Build city/other-region tables later | done in Stage 3 |
| Adversary stat profiles: zone tables (Stage 3) + city tables (Stage 4) + **5 recurring Act 1 threat profiles (Stage 5 `ACT_1_THREATS.md`)** exist; no standalone full bestiary yet | Medium (was High) | Solo-safe, mechanically usable threats across all tiers | Build the full bestiary (mid/high tiers especially) | 13 |
| Recurring-villain stat profiles: Act 1 early rivals statted (Ashby, Ren, Dunn via `ACT_1_THREATS.md` + NPC entries); no mid/high-tier villain profiles yet | Medium | Mechanically usable named antagonists at all tiers | Build villain profiles | 13, 15 |
| No noncombat obstacle library (though Act 1 quests/threats each provide noncombat outs) | Medium | Solo-friendly non-fight challenges | Build noncombat obstacles | 13 |

---

## Treasure and Artifacts

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No treasure-by-level guidance or magic-item list | Medium | Level-appropriate solo rewards | Build treasure/rewards files | 14 |
| Remembrance relics referenced in lore but not statted as items | Medium | Mystery-linked rewards | Build artifact files | 14 |

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
| No standalone act files for Acts 2–5 (levels 5–20) | High | Detailed mid/late-campaign play | Build act files | 15 |
| No standalone villain-escalation / endgame-states files | Medium | Escalating antagonist pressure and ending logic | Build escalation/endgame files | 15 |

---

## Audits

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| ~~No formal AI-readiness audit yet~~ — **Stage 6 first full audit complete (2026-06-10)**; foundation verified sound (0 Critical, 1 High fixed, 4 Medium, 5 Low); scaling to Stage 7 approved | — (no gap) | — | — | done in Stage 6 |
| No pre-play readiness audit | Medium | Confirm campaign is ready for live play | Run before Stage 17 | 16 |

---

## Related Files

- [`../00_control/TODO.md`](../00_control/TODO.md)
- [`../00_control/CONSISTENCY_AUDIT.md`](../00_control/CONSISTENCY_AUDIT.md)
- [`../00_control/DEVELOPMENT_STAGES.md`](../00_control/DEVELOPMENT_STAGES.md)
- [`EXPANSION_PLAN.md`](EXPANSION_PLAN.md)
