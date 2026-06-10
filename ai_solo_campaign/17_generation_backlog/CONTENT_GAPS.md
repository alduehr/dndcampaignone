# CONTENT_GAPS.md

## Purpose

Track missing or underdeveloped content by category. Use this for category-level gaps. Use `TODO.md` for actionable tasks. Use `CONSISTENCY_AUDIT.md` for defects or contradictions.

## Current Status

**Stages 0, 1, and 2 complete.** The campaign foundation exists: a starting region and settlement, seven major factions, twenty major NPCs, the full mystery/secret/revelation infrastructure, the level 1–20 arc shape, opening scenes, hooks, rumors, ten world clocks, the full AI runtime layer (protocols, prompts, templates), and seeded runtime state. The campaign is runnable for opening sessions.

The gaps below reflect what remains for **Stage 3+ depth and scale**, not foundational absence. Targets are drawn from `DEVELOPMENT_STAGES.md`, `PROJECT_RULES.md` content-scale targets, and `WORLDBUILDING_STANDARDS.md` density guidelines.

---

## Regions

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| Starting region exists as a frame only; lacks deep build (settlement spread, wilderness sites, encounter/rumor tables, regional quest chains) | High | 10–20 sessions of open-world play in the starting region | Deep-build the starting region | 3 |
| No adjacent (Ring 1) regions | Medium | World opens outward in multiple directions | Generate adjacent regions | 7 |
| Distant named regions are world-overview stubs only | Low | Long-term travel and high-tier play | Expand later as arc reaches them | 7, 15 |

---

## Settlements

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| Starting settlement (hub) is fully built; no additional regional towns/villages | High | Player needs multiple destinations within the starting region | Add 5–10 settlements (towns + villages) to the region | 3 |
| No major city | High | Mid-campaign political/social hub | Build first major city with districts | 4 |

---

## Factions

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| Seven major factions exist with public face, hidden agenda, leader, members, resources, and a clock each | — (no gap) | — | — | done in Stage 1 |
| Faction quest chains are not yet fully built out (intro → trust → complication → decision point) | Medium | Repeatable faction play and consequences | Build per-faction quest chains | 8, 10 |
| Secondary/minor faction members referenced in faction files lack full entries | Medium | AI DM avoids inventing recurring faction agents | Create secondary NPC entries | 3, 9 |
| No minor/local factions | Low | Texture in settlements and wilderness | Add minor factions during regional builds | 7+ |

---

## NPCs

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| 20 major NPCs exist with secrets and motivations | — (no gap) | — | — | done in Stage 1 |
| Major NPC count below long-term target (50–100) | Medium | Reduce major improvisation across the campaign | Expand major NPC roster | 9 |
| No secondary NPCs (target 200–500) | High | Settlements/factions feel populated; quest-givers, rivals, witnesses, contacts | Generate secondary NPCs alongside regional build | 3, 9 |
| No minor named NPCs (target 500+) | Medium | Local color across shops, temples, guards, villages | Generate minor NPC tables | 9 |
| `NPC_RELATIONSHIP_WEB.md`, `NPC_SECRET_LEDGER.md`, `NPC_VOICE_GUIDE.md` not created | Low | Managing a large NPC population | Create when NPC roster grows | 9 |

---

## Quests

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| 10 session hooks + 20 rumors exist (Act 1) | — (no gap) | — | — | done in Stage 1 |
| No developed multi-scene quest files (target 75–150) | High | Authored play beyond hooks; failure states and consequences | Build developed quests for region and factions | 5, 10 |
| No fully shaped main-arc Act 1 quest line (level 1–4) | High | Default narrative path through early levels | Build Act 1 quests | 5 |
| Hook/rumor library below long-term target (300–600) | Medium | Always-available authored opportunities | Expand hook/rumor library | 10 |
| Failure states not yet attached to developed quests (no developed quests exist yet) | Medium | Player choices have teeth | Add failure states as quests are built | 5, 10 |

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
| No regional dungeons/ruins (target 5–8 in starting region) | High | Adventure sites for early/mid play | Build regional dungeons | 3, 12 |
| No first major Act 1 dungeon | High | Level 1–4 arc climax site | Build first dungeon | 5 |

---

## Encounters and Bestiary

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No regional encounter tables | High | Travel/wilderness/downtime resolution without improvisation | Build encounter tables per region | 3, 13 |
| No custom monsters/adversary groups with stat profiles | High | Solo-safe, mechanically usable threats | Build bestiary with D&D-compatible stat profiles | 13 |
| No recurring-villain stat profiles | Medium | Mechanically usable named antagonists | Build villain profiles | 13, 15 |
| No noncombat obstacle library | Medium | Solo-friendly non-fight challenges | Build noncombat obstacles | 13 |

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
| No standalone act files for Acts 2–5 (levels 5–20) | High | Detailed mid/late-campaign play | Build act files | 15 |
| No standalone villain-escalation / endgame-states files | Medium | Escalating antagonist pressure and ending logic | Build escalation/endgame files | 15 |

---

## Audits

| Gap | Severity | Needed For | Suggested Fix | Related Stage |
|---|---|---|---|---|
| No formal AI-readiness audit yet | Medium | Confirm the foundation before scaling | Run first full audit | 6 |
| No pre-play readiness audit | Medium | Confirm campaign is ready for live play | Run before Stage 17 | 16 |

---

## Related Files

- [`../00_control/TODO.md`](../00_control/TODO.md)
- [`../00_control/CONSISTENCY_AUDIT.md`](../00_control/CONSISTENCY_AUDIT.md)
- [`../00_control/DEVELOPMENT_STAGES.md`](../00_control/DEVELOPMENT_STAGES.md)
- [`EXPANSION_PLAN.md`](EXPANSION_PLAN.md)
