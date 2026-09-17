# SETTLEMENT_BRACKHOLD_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Saltmere Reaches
settlement: Brackhold
level_range: 11-15
related: [../../04_world_atlas/region_map_packets/REGION_SALTMERE_REACHES.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/SALTMERE_REACHES_NPCS.md, ../../09_quests/by_region/SALTMERE_REACHES_QUESTS.md]
tags: [type:map, secrecy:mixed, function:cartography, settlement-map, map-packet, brackhold, saltmere-reaches]
---

> **Secrecy classification:** Mixed. The Drowned Towns (D24) are pre-Concord ruins visible from Brackhold's shore — a surface/echo of an older catastrophe, NEVER the keystone. Salt-Mother Tess's grief-rites are folk-wisdom of the crisis, never named as the harvest. Never hand directly to the player.

## Settlement: Brackhold (Saltmere Reaches — largest surviving salt-clan hold)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. Hold faces W toward the Saltmere water; shore-road runs E along the retreating waterline.
- **Full-continent position:** render-grid (57,68).
- **Population / scale:** ~900–1,300 residents; the largest surviving hold; the salt-clan confederacy's political center.
- **Water/road relationship:** on the **Saltmere's NW shore-land**; the **Salt Road** runs N (to Marrowdowns) and E (shore-road to Saltcairn, 63,73); clan-barge routes depart from the harbor-mole.

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The Clan Hold Gate | (20,35) | fortified stone quay-gate; clan-toll collected here |
| The Matriarch's Hall | (45,25) | Bryd Saltmere's seat; clan confederacy politics |
| The Salt-Works | (70,40) | drying pans, scale-houses; the hold's economic heart |
| The Grief-Keeper's Hall | (40,65) | Salt-Mother Tess Brackhold; old-rites and healing |
| The Harbor-Mole | (65,75) | clan-barge moorings; departure for the Drowned Towns shore |
| The Delver-Quarter | (30,80) | salvage guides, relic-buyers; rough but not dangerous |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Salt Road (N) | (30,0) | Marrowdowns (days–weeks via chalk-downs) |
| Shore Road (E) | (100,40) | Saltcairn (63,73; days along the retreating shore) |
| Clan-barge route | (65,95) S/E via water | Drowned Towns shore (45,50; hours by barge) |
| Ghostmark track (NW) | (0,20) | Ghostmark foothills / pass (Concord Heartlands N; weeks, dangerous) |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Clan guesthouse by the Hold Gate (20,35) | 3sp/night for non-kin; safe within walls; clan protocol expected |
| Resupply | Salt-Works market (70,40) | salt, fish, leather, rope; Matriarch's permit for barge access |
| Healing | Grief-Keeper's Hall (40,65) | mundane healing + old-rite comfort; DC 14 to earn Tess's attention |
| Information | Matriarch's Hall or Delver-Quarter | Bryd (DC 17); Delver Oss (DC 16); shore-road travelers (DC 13) |
| Faction contact | Matriarch's Hall | confederacy politics (Bryd); Cinder Ledger salt-buyers present seasonally |

## Law and Threat DCs

- **Entering Brackhold (non-kin):** greeting at the gate; clan-customary toll (2gp or equivalent trade) OR Persuasion DC 15 to waive.
- **Entering without toll or greeting:** politely stopped; Persuasion DC 16 to explain.
- **Disturbing the Grief-Keeper's rites:** Matriarch intervenes (not violent unless escalated); Persuasion DC 15 to smooth over.
- **Violent act within walls:** immediate clan-warrior response — 20+ fighters (**Berserker-like**, AC 13, ~67 HP); the Matriarch leads personally.
- **Approaching the Drowned Towns without Oss:** allowed (public); warned (the dead walk there now); Oss offers to guide for a fee (Q_SALT_001).

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| Salt-Clan Matriarch Bryd Saltmere | confederacy head | Matriarch's Hall (45,25) | Persuasion DC 17; the political center |
| Salt-Mother Tess Brackhold | grief-keeper; old-songs node | Grief-Keeper's Hall (40,65) | Insight DC 16 to sense her knowledge of "what the water keeps" |
| Drowned-Town Delver Oss | ruin-scavenger guide | Delver-Quarter (30,80) | Persuasion DC 16; guides for D24 at cost (L11+) |
| Marek Bonepan | salt-caravan master | passing (Salt Road); Harbor-Mole | secondary; Persuasion DC 14; trade news |

## Quest Hooks

- **Q_SALT_001 — The Town the Lake Gave Back:** the inciting event (walking dead uncovered at D24); first heard in Brackhold when Oss brings a survivor back. On-ramp for the Saltmere arc (L11).
- **Q_SALT_003 — The Confederation Crisis:** if Matriarch Bryd calls council on what to do about the Drowned Towns threat, the player can attend and be asked to act as neutral arbiter (L12+).
- **Barge-run contract:** Oss hires an escort to the Drowned Town shore for a deep-salvage run; the walking dead have made it untenable alone (L11+; leads to D24).

## Encounter / Treasure References

- Encounter: clan-warriors (Berserker / Veteran-like, AC 13–15, ~52–67 HP); Drowned Town undead at the shore (Ghoul / Wight-like, CR 5–8 surface-side; escalate at D24 depth); see `13_encounters_and_bestiary/` plains and undead lines at L11+.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 3 (L11–16) salt-trade rewards; clan-favors as currency; salvage from D24 (Remembrance relics, old-craft objects — use relic rules).

## Player-Safe Layer

The hold's fortified gate; the Matriarch's hall; the salt-works; the grief-keeper's hall; the harbor-mole with its barge-lines; the Delver-Quarter with its guides. From the shore you can see the Saltmere's retreating waterline and, at a distance, the emerging rooftops of the Drowned Towns.

## DM-Only Layer (NEVER on the player map)

- The Drowned Towns (D24) are **pre-Concord ruins** — their walking dead and the salt-clan grief-lore together corroborate that catastrophe and troubled dead are older than the Concord. NEVER the keystone or the machine.
- Salt-Mother Tess Brackhold's old-songs are M2/M5-oblique: "what the sea took and never sent back right" — folk-memory of a pre-Concord fall, not the harvest.
- No apex geometry here. The endgame is vertical beneath Hollowmere (NW only).

## Unresolved Map Gaps

- The Saltmere shoreline recedes year by year; the harbor-mole's exact reach into the water is illustrative.
- The Drowned Towns' visible extent from the shore is purposely left impressionistic (D24 reveals detail).

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_SALTMERE_REACHES.md`](../../04_world_atlas/region_map_packets/REGION_SALTMERE_REACHES.md)
- NPCs: [`../../08_npcs/by_region/SALTMERE_REACHES_NPCS.md`](../../08_npcs/by_region/SALTMERE_REACHES_NPCS.md)
- Quests: [`../../09_quests/by_region/SALTMERE_REACHES_QUESTS.md`](../../09_quests/by_region/SALTMERE_REACHES_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_SALTMERE_DEEP_TOWNS.md`](../../10_dungeons_and_ruins/THE_SALTMERE_DEEP_TOWNS.md)
