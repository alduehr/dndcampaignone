# REGION_SALTMERE_REACHES.md — Regional Map Packet

---
type: region
secrecy: mixed
status: static
region: Saltmere Reaches
level_range: 11-15
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../MAP_FEATURE_REGISTRY.md, ../../08_npcs/by_region/SALTMERE_REACHES_NPCS.md, ../../09_quests/by_region/SALTMERE_REACHES_QUESTS.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md, ../../10_dungeons_and_ruins/THE_SALTMERE_DEEP_TOWNS.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, saltmere-reaches]
---

> **Secrecy classification:** Mixed. The Drowned Towns are pre-Concord ruins — their walking dead corroborate the "older, wider fall" theme but are NEVER the keystone, the machine, the Concord Deep, or the Hollow Court (NW only, vertical beneath Hollowmere). The Saltmere's "going-down" is a pre-Concord catastrophe-echo, never the harvest mechanism. Salt-Mother Tess's old-songs fragments are M2/M5-oblique folk-memory only. Never hand this file directly to the player; render only the Player-Safe Layer.

## Region: Saltmere Reaches (MF-009)

- **Local grid:** 0–100, where **(0,0) = NW corner of the region frame, X = east, Y = south** (Y=0 top). (100,100) = SE.
- **Full-continent bounds this local grid maps to:** render-grid **X 55–66, Y 66–76** (centroid full (60.5,71)); from `CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md §10`.
- **Local↔full transform:** `local_X = (full_X - 55) / 11 * 100`; `local_Y = (full_Y - 66) / 10 * 100`. (Inverse: `full_X = 55 + local_X/100*11`; `full_Y = 66 + local_Y/100*10`.)
- **One-sentence identity:** A dying inland salt sea ringed by salt-clan holds and the bone-white Bonepan Flats — where the receding water uncovers whole drowned towns, proving that catastrophe and troubled dead are older than the Concord.

## Neighboring Regions

| Direction | Region |
|---|---|
| N | Concord Heartlands / the Ruin'd Crown (across the Ghostmark foothills) |
| NW | Marrowdowns (chalk-downs; shared Ghostmark-edge) |
| NE | open country toward the Emberfells (no named region at this boundary) |
| E | Emberfell Theocracy (across the Bonepan Flats) |
| SW | Sallowmarch Protectorate (the delta coast) |
| SE | Hollow Gulf Ports |

## Terrain Zones (local polygons)

| Zone | Type | Local centroid | Full-grid | Description |
|---|---|---|---|---|
| The Saltmere basin shore | salt-clan hold-country | (35,40) | (58.9,70) | The Saltmere's shrinking shore; hold-towns, salt-pans, brine-flats. |
| The Bonepan Flats | salt badland | (72,62) | (62.9,72.2) | White bone-dry salt expanse E and S of the sea; lethal without water. |
| The Ghostmark foothills | low mountain fringe (N) | (30,18) | (58.3,67.8) | The Ghostmark Range's foot; crumbling Concord-era waystation ruins; S passes to the Heartlands. |
| The receding shore zone | active retreat-zone | (45,50) | (59.9,71) | Where the lake-edge has fallen back; exposed flats, emerging ruins, wrong-coming dead. |
| The deep Saltmere | surviving inland brine-water | (25,35) | (57.8,69.5) | The still-living salt sea; fishing and barge-routes; rough brine-squalls. |

## Water Features

| Feature | Type | Local | Full-grid | Flow |
|---|---|---|---|---|
| The Saltmere | inland salt sea (receding) | (25,35) | (57.8,69.5) | Static/shrinking; NW shore retreating fastest; exposes ruins |
| Salt-harvest pans | salt-flat extraction shores | along W shore | — | Worked by the clans; the region's primary economy |
| Ghostmark drainage | seasonal melt-streams (N) | (25,18) | (57.8,67.8) | Feed the sea in winter; dwindling |

> The Saltmere has no river inlet strong enough to replace what it loses — the "going-down" is a slow, generational catastrophe the clans have accepted as the world's truth.

## Roads / Routes (local polylines)

| Route | Local waypoints | Full-grid | Travel time | Notes |
|---|---|---|---|---|
| Saltmere Shore Road | (18,20) Brackhold → (45,50) Drowned Towns → (73,70) Saltcairn | (57,68)→(60,71)→(63,73) | 3–5 days end-to-end | Follows the retreating shoreline; watch the clan-barges |
| Ghostmark Pass (N, to Heartlands) | (30,18) pass-foot → N edge | (58.3,67.8)→(58,60) Heartlands S | weeks through passes | Poorly maintained; rockfall; dead stir at the old waystation |
| Bonepan Track (SE, to Gulf) | (73,70) Saltcairn → SE edge | (63,73)→(65,80) toward Calderport | 4–6 days (water required) | Only the prepared attempt the Bonepan; dry-season only |
| Clan-barge routes | Brackhold ↔ Drowned Towns ↔ open lake | lake-wide | hours–days | The salt-clans' internal sea-lanes; barge pilot required |

## Bridges / Fords / Ferries / Locks

| Feature | Type | Local | Full-grid | Notes |
|---|---|---|---|---|
| Brackhold harbor-mole | stone quay (hold) | (18,20) | (57,68) | The matriarch's harbor; barge-moorings and salt-docks |
| Saltcairn quay | smaller hold-quay | (73,70) | (63,73) | Ghostmark-edge hold; caravan terminus for the Bonepan Track |
| Drowned Town ford | emerging shoreline ford | (45,50) | (60,71) | Exposed as the lake retreats — not always passable; dead make it worse |

## Settlements

| Settlement | Type | Local | Full-grid | Anchor source / file |
|---|---|---|---|---|
| Brackhold | largest surviving salt-clan hold (hub) | (18,20) | (57,68) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (sr.brackhold); NPC/quest hub |
| Saltcairn | Ghostmark-edge clan-town | (73,70) | (63,73) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (sr.saltcairn) |
| The Drowned Towns | pre-Concord ruin-cluster (D24 — NOT a live settlement) | (45,50) | (60,71) | `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (sr.drowned_towns); D24 anchor |

> The Drowned Towns are a **pre-Concord ruin-cluster** uncovered by the receding Saltmere — a dungeon anchor (D24), not a hold-town.

## Dungeons / Adventure Sites

| Site | Local | Full-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D24 The Saltmere Deep Towns | (45,50) | (60,71) | exposed ruin-buildings at the lake-edge (intact walls, drowned streets) | visible (label "the Drowned Towns") |

## Ruins / Wilderness Landmarks

| Landmark | Local | Full-grid | Notes |
|---|---|---|---|
| The Drowned Towns (D24) | (45,50) | (60,71) | pre-Concord ruins uncovered by the receding Saltmere; walking dead (Q_SALT_001); M2/M5-oblique |
| The Bone-Gate waystation | (30,18) | (58.3,67.8) | crumbling Ghostmark-pass Concord-era ruin; passage-ghost legends |
| The Salt-Pile | (65,45) | (62.2,70.5) | vast ancient brine-evaporation mound on the Bonepan edge; pre-Concord, possibly pre-anything |

## Level Range And Solo Danger

- **Recommended level:** 11–15.
- **Expected solo danger:** Moderate on the shore-road and in the hold-towns; high at the Drowned Towns and on the Bonepan; extreme in the deep Drowned Town ruins or if the walking-dead crisis spreads.
- **Lethal-at-low-level zones (telegraphed):** the **Bonepan Flats** (exposure without water; Constitution DC 15 per day, worsening) and the **Drowned Towns at depth** (CR 11–14 undead, water hazards). Telegraphed by the clan-saying ("the bones take the careless") and the town's reputation for "walking things."
- **Telegraphing:** the shore-road is safe by clan custom; the Drowned Town threat is the inciting event of Q_SALT_001; Matriarch Bryd explicitly rates the dangers for any outsider who asks; the Bonepan's bleached bones of past failures are visible before committing.

## Encounter And Hazard Mechanics

- **Encounter themes (stat references):** salt-clan warriors (**Berserker / Veteran-like**, AC 13–15, ~52–65 HP; mounted or barge-poleboats); Drowned Town undead (**Ghoul / Wight / Revenant-like**, CR 5–11 surface, scale at D24 depth); Ghostmark waystation spirits (**Wraith / Specter-like**, CR 5–8). Use `13_encounters_and_bestiary/` plains and undead encounter lines scaled to L11+.
- **Environmental hazards:** Bonepan dehydration (Constitution DC 15 per day without water; 2d6 damage on fail); Saltmere brine-squall (Vehicles(water) / Athletics DC 16; swamped barge possible); Thin-touch from unshielded relic contact at deep D24 ruins; Ghostmark landslide (Dexterity DC 14, 3d6 bludgeoning).
- **Social DCs (typical):** Persuasion DC 17 (Matriarch Bryd Saltmere); Persuasion DC 16 (Delver Oss — ruin access); Insight DC 16 (Salt-Mother Tess Brackhold's grief-rite knowledge); Persuasion DC 16 (Marek Bonepan, Saltcairn). Per-quest DCs in `SALTMERE_REACHES_QUESTS.md`.
- **Scaling:** L11 — shore-road on-ramp and the first uncovered-town mystery (Q_SALT_001). L15 — the deep town's full walking dead (D24), a confederation-crisis, and Salt-Mother Tess's old-songs at full depth.

## Local Labels (player map)

The Saltmere Reaches (region label, ONE); the Saltmere (water, label on water); Brackhold; Saltcairn; the Drowned Towns (ruin marker at the lake-edge); the Ghostmark foothills (terrain label, N edge); the Bonepan Flats (terrain label, E/SE); the Saltmere Shore Road; Ghostmark Pass (route, N); South Track (route, SE; label "water required").

## Player-Safe Layer

- Visible: the shrinking lake, the two hold-towns, the Drowned Towns ruin-cluster at the lake-edge, the shore-road, the Bonepan Flats. The region reads as a place of slow ancient disaster — the sea going away, tough clan-survivors enduring it — with one active crisis (dead walking from the exposed ruins).
- Nothing here points to the Hollow Court or the keystone.

## DM-Only Layer (NEVER on the player map)

- The Drowned Towns (D24) are **pre-Concord ruins** — their walking dead and the salt-clan grief-lore together corroborate that catastrophe and troubled dead are *older than the Concord*, which is why the Concord built the harvest. NEVER the keystone, NEVER the machine.
- Salt-Mother Tess Brackhold's old-songs are **M2/M5-oblique** — folk-memory of "what the sea took and never sent back right" — never named as Quiet Country drain or Concord harvest.
- No apex geometry here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- The lake's precise current shoreline vs. historical extent is intentionally fluid.
- The Ghostmark Range's individual passes are noted but not individually mapped.
- The true extent of the Drowned Towns complex is covered in D24 (`THE_SALTMERE_DEEP_TOWNS.md`).

## Related Files

- NPCs: [`../../08_npcs/by_region/SALTMERE_REACHES_NPCS.md`](../../08_npcs/by_region/SALTMERE_REACHES_NPCS.md)
- Quests: [`../../09_quests/by_region/SALTMERE_REACHES_QUESTS.md`](../../09_quests/by_region/SALTMERE_REACHES_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_SALTMERE_DEEP_TOWNS.md`](../../10_dungeons_and_ruins/THE_SALTMERE_DEEP_TOWNS.md)
- Authority: [`../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md`](../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md) · [`../FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../FULL_CONTINENT_SETTLEMENT_ANCHORS.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
