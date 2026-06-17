# CARADRIL_CITY_MAP.md — City Map Packet

---
type: settlement
secrecy: mixed
status: static
region: Caradril
settlement: Caradril
level_range: 3-16
related: [../CARADRIL.md, ../../04_world_atlas/CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../../04_world_atlas/region_map_packets/REGION_CARADRIL.md, ../caradril_districts/THE_MAGISTERIUM.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md]
tags: [type:map, secrecy:mixed, function:cartography, city-map, map-packet, caradril]
---

> **Secrecy classification:** Mixed. The Sunken Wards deep entrance and any Concord-Deep faint touch are DM-only. The Sealed Archive is a visible building, but its contents are DM-only. Never hand directly to the player.

## City: Caradril — Local City Grid

- **Local grid:** 0–100 (X east, Y south). (0,0) = NW corner of the city frame, (100,100) = SE.
- **Full-continent position:** render-grid (34,35); campaign-grid (82,80). The whole city = full-grid point; this packet is the internal layout.
- **Population:** ~18,000–22,000. A true city with districts.

## River and Lake Geometry

- **The Verdance** runs roughly **west-to-east** through the city: enters at local (5,50), flows to local (80,50), then widens into the Stillwater.
- **The Stillwater** (harbor-lake) lies at the **east end**: local (80,40)→(95,40)→(95,65)→(80,65). The Counting-Quays front it.
- **North bank** = upper city (higher ground, local Y < 45). **South bank** = low city (riverside, local Y > 55).

## District Positions

| District | Bank | Local centroid | Rough bounds | Power bloc | File |
|---|---|---|---|---|---|
| The Magisterium | N (upper) | (35,25) | X 25–50, Y 15–35 | Tidewater Council / Charter Houses | THE_MAGISTERIUM.md |
| The Lantern Reach | N (E, near Stillwater) | (65,30) | X 55–78, Y 20–40 | Concord Remnant | THE_LANTERN_REACH.md |
| The Counting-Quays | N (waterfront, Verdance→Stillwater) | (72,45) | X 62–85, Y 40–52 | Cinder Ledger | THE_COUNTING_QUAYS.md |
| Highmourn | S (E hill) | (70,72) | X 60–82, Y 62–82 | Mourners' Circle / clergy | HIGHMOURN.md |
| The Crucible | S (W foundry) | (25,68) | X 15–38, Y 60–78 | craft guilds | THE_CRUCIBLE.md |
| The Ashmarket | S (riverfront) | (45,60) | X 35–55, Y 55–66 | Salt Syndicate (black market) | THE_ASHMARKET.md |
| The Sill | S (low waterfront undercity) | (40,72) | X 30–50, Y 66–80 | the Hush / the poor | THE_SILL.md |
| The Sunken Wards | below (partly flooded old undercity) | (45,85) | beneath the S bank | (delvers, cultists) | THE_SUNKEN_WARDS.md |

## Bridges / Ferries (N↔S banks)

| Crossing | Local | Notes |
|---|---|---|
| Upper Bridge (Magisterium ↔ Ashmarket/Crucible) | (40,50) | the main civic crossing |
| Quay Bridge (Counting-Quays ↔ Highmourn/Sill) | (68,50) | the trade crossing near the harbor |
| The Brass Ferry | (50,55) | river ferry serving the Sill (tavern landmark) |

## Main Road Exits

| Exit | Local edge | Leads to |
|---|---|---|
| North road | (35,5) N edge | the southern downs / Ashgarden Vale (South Road) |
| East docks road / Stillwater | (95,50) E edge | the Stillwater quays; sea-route arrivals; up-Verdance (Verdance Road, Ring 2) |
| South road | (45,95) S edge | the Verdance Reaches up-river (SE) |
| Western gate | (5,50) W edge | the Tollwood approach (East Road) and the western hinterland |

## Docks / Quays

- **The Counting-Quays** front the Verdance-to-Stillwater junction (local 72,45) — the Ledger's banking docks.
- **Stillwater quays** at the lake's W shore (local 80,45) — the grand water-arrival point.

## Named Landmark Positions

| Landmark | District | Local | Notes |
|---|---|---|---|
| Magisters' Hall (Tidewater Council seat) | Magisterium | (35,25) | civic heart |
| The Ledger Keep (Cinder Ledger HQ) | Counting-Quays | (72,45) | Vyre's seat |
| The Lamplighters' Hall (Remnant college) | Lantern Reach | (62,30) | public face |
| The Sealed Archive (Remnant true vault) | Lantern Reach | (68,28) | M6/M9 — building visible, contents DM-only |
| The Threshold Cathedral | Highmourn | (70,70) | Three Thresholds temple |
| The Quiet Houses (cemetery-temple) | Highmourn | (74,75) | death-rites |
| The Pale Star inn (player base) | Magisterium edge | (45,38) | recommended base |
| The Last Tally tavern | Counting-Quays | (70,48) | rumor node |
| The Brass Ferry tavern | the Sill | (50,55) | rumor node |
| Lampgate | Lantern Reach edge | (78,30) | district gate |
| The Sealgate (sealed stair to Sunken Wards) | the Sill / below | (45,80) | D16 entrance (visible sealed door) |

## Walls / Gates

- Caradril is a tiered river-city with district gates rather than a single continuous wall; the named gates are **Lampgate** (Lantern Reach) and the **Western gate** (the main landward gate). Tide-Watch posts guard the bridges and the Quays.

## Player-Safe Layer

All 8 districts and their boundaries; the Verdance and the Stillwater; the two bridges + the Brass Ferry; the four road exits; the docks; all named landmark buildings (including the Sealed Archive and the Sealgate as a visible sealed door); the Tide-Watch posts.

## DM-Only Layer (NEVER on the player map)

- The **Sunken Wards** as a mapped flooded Concord level beneath the S bank (the Remnant's secret map; Wessel Dree guards the way).
- The Sunken Wards' **deep entrance** below the Sealgate (D16 lower levels).
- The **Concord-Deep faint touch** to the Wards (a dormant cousin-node; never a network line).
- The **Sealed Archive's contents** (the harvest/Quietfall proof — the building is visible, the truth is not).

## Unresolved Map Gaps

- Exact district boundaries are approximate (the district files hold internal detail).
- The Sunken Wards' subsurface extent is DM-only and deliberately vague.

## Related Files

- [`../CARADRIL.md`](../CARADRIL.md) · [`../../04_world_atlas/region_map_packets/REGION_CARADRIL.md`](../../04_world_atlas/region_map_packets/REGION_CARADRIL.md) · [`../caradril_districts/`](../caradril_districts/) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
