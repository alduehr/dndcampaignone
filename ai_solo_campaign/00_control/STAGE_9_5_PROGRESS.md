# STAGE 9.5 — Full-Continent NPC Readiness — PROGRESS

## Status: COMPLETE (2026-06-12; honest-recount cleanup pass 2026-06-12)

Stage 9.5 extended the NPC codex from the campaign cluster (Reach / Caradril / Ring 1) to the **12 far-continent placeholder regions**, so the AI DM can run play anywhere on Orrun (Lvl 6–17) without improvising major social infrastructure. The placeholder regions remain placeholders — these are **light NPC-facing anchors** (a major roster, faction agents, services, witnesses, and color), NOT full gazetteers, quests (Stage 10), or dungeons (Stage 12).

A 2026-06-12 cleanup pass re-counted every region by hand and by script, corrected stale counts, lifted five regions (and Sallowmarch's distinct-authored count) from 11 → 12 secondaries, registered the light anchors and the six new secondaries in `NAMING_REGISTRY.md`, and reconciled all tracking files.

---

## Counting Method

- **Major** = profiled `### XX-Mn.` entries in each file's MAJOR section (verified by hand).
- **Secondary** = `- **[Faction]**`-prefixed bullet entries in each file's SECONDARY section (verified by script + hand). A handful are **cross-listed** references to an NPC authored in another region file (Hadwin Vael → Verdance; Mossa Drenn → Verdance; Crown-Customs Legate Vorr → shared Hollow Gulf/Sallowmarch); these are counted in the file where they appear (an AI DM loading that file sees them) but noted as cross-listed so the distinct-authored total is also tracked.
- **Minor** = data rows in each file's MINOR table (total pipe-rows minus the header + separator), verified by two independent awk passes that agree.

---

## Final NPC Counts (verified 2026-06-12)

| Region | File | Major | Secondary | Minor | Lvl |
|---|---|---|---|---|---|
| Verdance Reaches | `08_npcs/by_region/VERDANCE_REACHES_NPCS.md` | 4 | 18 | 35 | 8–12 |
| Concord Heartlands / Ruin'd Crown | `08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md` | 4 | 16 | 35 | 13–17 |
| Glassmere League | `08_npcs/by_region/GLASSMERE_LEAGUE_NPCS.md` | 5 | 19 | 47 | 9–13 |
| Hethewald Free Holds | `08_npcs/by_region/HETHEWALD_FREE_HOLDS_NPCS.md` | 3 | 15 | 35 | 7–12 |
| Hollow Gulf Ports | `08_npcs/by_region/HOLLOW_GULF_PORTS_NPCS.md` | 5 | 15 | 43 | 10–15 |
| Saltmere Reaches | `08_npcs/by_region/SALTMERE_REACHES_NPCS.md` | 3 | 12 | 34 | 11–15 |
| Emberfell Theocracy / Ashfast | `08_npcs/by_region/EMBERFELL_THEOCRACY_NPCS.md` | 4 | 12 | 36 | 12–16 |
| Sallowmarch Protectorate | `08_npcs/by_region/SALLOWMARCH_PROTECTORATE_NPCS.md` | 4 | 13 | 35 | 10–14 |
| Marrowdowns | `08_npcs/by_region/MARROWDOWNS_NPCS.md` | 3 | 12 | 35 | 6–10 |
| Wender Steppe | `08_npcs/by_region/WENDER_STEPPE_NPCS.md` | 3 | 12 | 31 | 8–13 |
| Karran Marches | `08_npcs/by_region/KARRAN_MARCHES_NPCS.md` | 3 | 12 | 33 | 9–14 |
| Sunmark | `08_npcs/by_region/SUNMARK_NPCS.md` | 3 | 12 | 33 | 8–13 |
| **STAGE 9.5 TOTAL** | — | **44** | **168** | **432** | — |

- Secondary 168 counts every secondary bullet as it appears per-file; **4 of these are cross-listed** references to NPCs authored in another region file, so the distinct-authored secondary total is **164**.
- **Every region meets the per-region minimum: 3+ major, 12+ secondary, 30+ minor.** ✓

**Cumulative codex totals (Stage 9 core + Stage 9.5 far):** **94 major · 368 secondary · 953 minor** (50 / 200 / 521 core + 44 / 168 / 432 far).

---

## The 44 Far-Continent Majors

- **Verdance:** Wessel Crane, Lord Ennis Marrow, Mossa Drenn, Hadwin Vael
- **Concord Heartlands:** Hollin Vane (apex-adjacent care), Lyssa Crownmouth, Father Casian Ord, "Old Crown" Mab
- **Glassmere:** Oren Glass, Sefwy Holt, "the Glass Ear", Mareth Senn, Wenna Lowwater
- **Hethewald:** Bram Hethe, Onn Greenward, "Greenfinger" Maddoc
- **Hollow Gulf:** Ive Calder, Roke Mallin, Doss Saltgate, Sera Mardenmouth, Hadiz of Surren
- **Saltmere:** Bryd Saltmere, Delver Oss, Tess Brackhold
- **Emberfell:** Vole Cindra, Sef Embren, Mira Cindra, Doss Ashfast
- **Sallowmarch:** Vorr Sallow, Doll Fenn, "Heron" Maddox, Sela Reed
- **Marrowdowns:** Aldous Penmark, Senna Crale, Doss Wether
- **Wender:** Tamur Wend-Khar, Wind-Singer Esha, Borr of the Black Horse
- **Karran:** "Iron" Brask, Mully Karr, Wenna Stone
- **Sunmark:** Sael Sunmark, Sun-Singer Doll, Doss Sunward

(Most are elevations of the `FAR_CONTINENT_NPCS.md` horizon-scaffold figures, now fully profiled; the rest are wholly new. Registered in `NAMING_REGISTRY.md` → "Stage 9.5 Far-Continent NPCs".)

---

## Cleanup-Pass Changes (2026-06-12)

### Six secondary NPCs added (5 regions 11→12; Sallowmarch to 12 distinct-authored)

| Name | Region | Anchor | Role |
|---|---|---|---|
| Salt-Caravan Master Marek Bonepan | Saltmere Reaches | the trade-track / Bonepan Flats | Salt-train master; land-route out; anti-Ledger lever |
| Horse-Reeve Edony Marrow | Marrowdowns | down-roads / Marrowmoot | Mounted shire-lawkeeper; road-law contact; M5 animal-omen |
| Kin-Mother Tamur-Sai | Wender Steppe | the Winter-Camp | Clan-matriarch; social glue of the confederacy (no kin to the Speaker) |
| Pass-Toll Warlord Hessa Teeth | Karran Marches | the pass toward the south | Lesser pass-warlord; gateway south; refugee-flow witness |
| Greenway-Warden Tamsin Greenway | Sunmark | the Green Roads | Grove-road captain; safe-passage; missing-pilgrim (M5-faint) witness |
| Rice-Moot Speaker Pell Sallows | Sallowmarch Protectorate | the Rice Sallows | Rice-villages' speaker; the delta's civic will/defiance lever |

All six carry: name, region, location/circuit, role, distinctive trait, current problem, useful knowledge, a link to a major NPC / faction / route / tension, a player-safe description, and a labeled **(DM)** note. None exposes the apex truth; all reinforce existing M-line corroborations obliquely.

### Light NPC-facing anchors registered

All Stage 9.5 anchor place-names (Marrowfen Stair, Lord's Wend, Cresswater, the Nine Locks, Crownmouth, the Pilgrim Camps, Glassmere city, the Floor, the Three Bridges, the Reliquary, Lowwater, Sennfort/Cairnwater, Hethemoot, Greenward, Tollreach, the Old Holds, Calderport, Saltgate, the Foreign Quarter, the Mardenmouth, Brackhold, the Drowned Towns, Saltcairn, Ashfast city, Cinderhold, the Ash Roads, Fenward, Reedmouth, the Rice Sallows, the Fever Channels, Marrowmoot, Penmark Hold, the Barrow-Fields, Wether, the Winter-Camp at Cold Springs, the Sky-Stones, the Spine-Foot trade-meet, Brask's Hold, Karran-Gate, the Deep Cuts, the Old Iron forts, the Great Grove at Sunhollow, the Grove-Camps, the Green Roads) are now logged in `NAMING_REGISTRY.md` → "Stage 9.5 — Light NPC-Facing Anchors", each marked **"light NPC-facing anchor — not a full settlement, not a major map feature."** They are retained in the region files (useful) and not promoted to full settlements.

### Count references reconciled

`STAGE_9_5_PROGRESS.md`, `STAGE_STATUS.md`, `CONTENT_INDEX.md`, and `NPC_INDEX.md` were all updated to the verified per-region and total counts (44 / 168 / 432; cumulative 94 / 368 / 953) and to accurate "no new major geography; light anchors added and registered" language.

---

## Files Created/Modified This Pass

- 6 region NPC files edited (one secondary each): `SALTMERE_REACHES`, `MARROWDOWNS`, `WENDER_STEPPE` (+inline count fix), `KARRAN_MARCHES`, `SUNMARK`, `SALLOWMARCH_PROTECTORATE`.
- `00_control/NAMING_REGISTRY.md` — new "Stage 9.5 — Light NPC-Facing Anchors" subsection + cleanup-pass secondary note.
- `00_control/STAGE_9_5_PROGRESS.md` (this file), `00_control/STAGE_STATUS.md`, `00_control/CONTENT_INDEX.md`, `08_npcs/NPC_INDEX.md` — counts reconciled.

(Infrastructure files — `NPC_RELATIONSHIP_WEB.md`, `NPC_SECRET_LEDGER.md`, `NPC_VOICE_GUIDE.md` — already carry Stage 9.5 sections covering all 44 majors; the six new *secondaries* do not require voice-guide entries per `NPC_STANDARDS.md`, and their links are captured inline in the region files.)

---

## Completion Verdict & Gate Checklist

- [x] All 12 far-continent region NPC files exist.
- [x] Every region meets minimums (3+ major / 12+ secondary / 30+ minor) — verified by hand and script.
- [x] 44 majors carry full profiles (player-safe + DM-only fields, mechanical Tier profiles, relationship links).
- [x] Relationship web, secret ledger, and voice guide cover all 44 majors (Stage 9.5 sections).
- [x] NPC_INDEX points to all 12 files.
- [x] NAMING_REGISTRY has all 44 major names + the light anchors + the 6 new secondaries.
- [x] CONTENT_INDEX has all 12 files.
- [x] No player-safe secret leaks; **apex-truth firewall held** — NO far-region NPC knows the harvest, the Hollow Court, the surviving Custodians, the deliberate Quietfall, or the Hollowmere keystone.
- [x] No new major geography or factions — only **light NPC-facing anchors** (registered) and 6 secondary NPCs.
- [x] Pre-Concord echoes (Saltmere drowned towns, Marrowdowns barrows, Karran Old Iron forts) and the Emberfell thematic mirror are kept **distinct** from the keystone; the Concord Heartlands are the *surface* fallen capital, never the Concord Deep / Under-Shrine.
- [x] All four count/status files agree on the final totals (44 / 168 / 432; cumulative 94 / 368 / 953).
- [x] No known audit blockers.

**Stage 9.5 is COMPLETE.** Every gate criterion is met: all 12 region files exist and meet the per-region minimum, the major roster is fully profiled and supported by the relationship/secret/voice infrastructure, naming and content indexes are reconciled, no apex secret leaks, and no new major geography or factions were created beyond registered light anchors.

## Remaining Gaps

- None blocking. The 12 far regions remain **placeholders** by design — they have NPC rosters but not yet quests (Stage 10), dungeons (Stage 12), or full gazetteer/region files. This is intentional and consistent with `FULL_WORLD_MAP_AUTHORITY.md`.

## Next Stage

**Stage 10 — Quest Library Expansion.**
