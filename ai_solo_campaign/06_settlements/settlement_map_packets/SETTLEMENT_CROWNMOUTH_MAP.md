# SETTLEMENT_CROWNMOUTH_MAP.md — Settlement Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Concord Heartlands
settlement: Crownmouth
level_range: 13-17
related: [../../04_world_atlas/region_map_packets/REGION_CONCORD_HEARTLANDS.md, ../../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md, ../../09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md]
tags: [type:map, secrecy:mixed, function:cartography, settlement-map, map-packet, crownmouth, concord-heartlands]
---

> **Secrecy classification:** Mixed. **CRITICAL:** Crownmouth sits at the edge of the Concord's *surface* fallen capital — NOT the keystone, NOT the Concord Deep, NOT the Hollow Court's seat. The ruin beyond the walls is presented as "the old empire's heart, smashed" — unexplained, never a machine or network. Never hand directly to the player; render only the Player-Safe Layer.

## Settlement: Crownmouth (Concord Heartlands — fortified scavenger-town)

- **Local grid:** 0–100 (X east, Y south); (0,0) = NW corner. Town is compact; walls on W/N face the Crown Road; ruin-edge to the E/SE.
- **Full-continent position:** render-grid (60,54).
- **Population / scale:** ~600–900 permanent residents; the only functioning settlement at the ruin's edge; a large fortified scavenger-town by this frontier's standards.
- **Water/road relationship:** no river within walls; well-water only; the **Crown Road** W toward Glassmere is the main supply-line; the ruin-edge gate E is where the scavengers go in.

## Layout / Notable Areas

| Area | Local | Notes |
|---|---|---|
| The Crown Road Gate | (20,35) | fortified main gate; road to Glassmere W; War-Captain's inspection point |
| The War-Captain's Hall | (45,30) | Lyssa Crownmouth's command seat; practical law; the real governance center |
| The Pilgrim-Quarter | (70,40) | camp-inn and rough lodging for relic-seekers; the largest building in town |
| The Salvage Market | (55,60) | relic sales, provisions, rope, tools; Remnant-affiliated buyers present |
| The Healer's Row | (35,70) | Remnant-affiliated medic; mundane + 2nd-level divine healing |
| The Ruin-Edge Gate | (80,55) | toward D21; War-Captain controls access; only guides go through officially |

## Entrances / Exits

| Exit | Local edge | Leads to |
|---|---|---|
| Crown Road (W) | (0,35) | Glassmere (weeks away via the Greatspine passes) |
| Greatspine Pass track (N) | (45,0) | N pass; altitude; dangerous; weeks |
| Ruin-Edge Gate (E/SE) | (95,55) | D21 / the Ruin'd Crown (immediately beyond the gate) |
| Pilgrim Road (S) | (60,100) | Pilgrim Camps (63,58; another anchor); Saltmere S |

## Services

| Service | Where | Details |
|---|---|---|
| Rest | Pilgrim-Quarter (70,40) | rough camp-inn; 2sp/night; safe within walls; shared sleeping |
| Resupply | Salvage Market (55,60) | rations, rope, tools, torches, salvage gear; limited healing potions |
| Healing | Healer's Row (35,70) | mundane + Cure Wounds/Lesser Restoration; Wisdom DC 14 to locate when not obvious |
| Information | War-Captain's Hall or Salvage Market | Lyssa (Persuasion DC 17); Market rumors (Persuasion DC 13) |
| Faction contact | War-Captain's Hall | Remnant contact via Hollin Vane (Persuasion DC 17; arrives periodically) |

## Law and Threat DCs

- **Gate entry:** state purpose; Persuasion DC 14 (routine business) or DC 16 (claiming Remnant affiliation without credentials).
- **Carrying unregistered salvage:** Persuasion DC 16 to explain without confiscation.
- **Moving toward Ruin-Edge Gate without a guide:** stopped by guards; Persuasion DC 15 to proceed alone (Lyssa recommends against it).
- **Violent act within walls:** immediate response — 15 town-guards (**Guard / Veteran-like**, AC 15, ~16–45 HP); Survival DC 17 to escape the walled perimeter.
- **Bribery (gate officials):** DC 14 to attempt discreetly; failure attracts Lyssa's attention.

## Key NPC Links

| NPC | Role | Location | Notes |
|---|---|---|---|
| War-Captain Lyssa Crownmouth | settlement leader; independent | War-Captain's Hall (45,30) | Persuasion DC 17; the real authority |
| Crown-Reclaimer Magister Hollin Vane | Remnant expedition-lord; apex-adjacent | periodically at Salvage Market | Persuasion DC 17; never confirms Hollow Court or keystone; a dupe |
| Father Casian Ord | Pilgrim Camps heretic-priest | Pilgrim-Quarter (70,40) | Insight DC 16 to sense he knows more than he says |
| "Old Crown" Mab | deep-ruin guide | Salvage Market or Ruin-Edge Gate | Persuasion DC 15 for guided access; DC 17 for deep interior |

## Quest Hooks

- **Q_CH_001 — The Last Safe Town:** Crownmouth is the inciting-incident hub; defense, politics, and the first push toward the ruin. On-ramp for the Heartlands arc (L13).
- **Q_CH_002 — The Record-Vault Expedition:** Hollin Vane recruits at the Salvage Market for a push to the deep vaults in D21 (L15; surface-proof of the Concord's history only).
- **"Old Crown" Mab's run:** hire Mab for a guided D21 salvage run; she names exactly how far she will go and why she stops there (L13+; see `THE_OLD_CONCORD_HEARTLANDS_RUIN.md`).

## Encounter / Treasure References

- Encounter: rival expedition factions (Remnant, Ledger, Emberfell agents; **Veteran-like**, AC 16, ~65 HP); Crown undead at ruin-edge (**Wight / Wraith-like**, CR 8–12); see `13_encounters_and_bestiary/` undead + rival-faction lines at L13+.
- Treasure: `14_treasure_and_artifacts/REWARDS_BY_LEVEL.md` Tier 3 (L11–16) salvage; Remnant document-certificates as currency; Vane's expedition-pay in gold.

## Player-Safe Layer

The fortified scavenger-town; the Crown Road arrival; the Pilgrim-Quarter as social hub; the Salvage Market; the Healer's Row; the Ruin-Edge Gate as the threshold toward D21 (the broken ruin, presented as "the old empire's heart, smashed"). Nothing here confirms the Concord's machine, the harvest, or the Hollow Court.

## DM-Only Layer (NEVER on the player map)

- The deep record-vaults in D21 are M6-adjacent lore — a surface-proof of the harvest as historical event; they confirm what the Concord DID, never where the machine IS.
- Hollin Vane is a dupe; he believes his records are the full truth. They are not; the keystone's location is vertical beneath Hollowmere (NW only), not in the Heartlands.
- No Hollow Court presence in Crownmouth; the Court never staffed the surface capital after the Quietfall.

## Unresolved Map Gaps

- Internal building layout is compact-town level; full district depth is not required for an eagle-test landing.
- The Ruin-Edge Gate's immediate exterior (the first 100m into the ruin) is covered in D21 (`THE_OLD_CONCORD_HEARTLANDS_RUIN.md`).

## Related Files

- Region: [`../../04_world_atlas/region_map_packets/REGION_CONCORD_HEARTLANDS.md`](../../04_world_atlas/region_map_packets/REGION_CONCORD_HEARTLANDS.md)
- NPCs: [`../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md`](../../08_npcs/by_region/CONCORD_HEARTLANDS_NPCS.md)
- Quests: [`../../09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md`](../../09_quests/by_region/CONCORD_HEARTLANDS_QUESTS.md)
- D-site: [`../../10_dungeons_and_ruins/THE_OLD_CONCORD_HEARTLANDS_RUIN.md`](../../10_dungeons_and_ruins/THE_OLD_CONCORD_HEARTLANDS_RUIN.md)
