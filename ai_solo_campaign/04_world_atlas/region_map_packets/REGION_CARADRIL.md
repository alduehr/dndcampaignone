# REGION_CARADRIL.md — Regional Map Packet (city-state and hinterland)

---
type: region
secrecy: mixed
status: static
region: Caradril
level_range: 3-16
related: [../CARTOGRAPHY_AUTHORITY_FULL_CONTINENT.md, ../MAP_FEATURE_REGISTRY.md, ../../06_settlements/CARADRIL.md, ../../06_settlements/city_map_packets/CARADRIL_CITY_MAP.md, ../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md]
tags: [type:map, secrecy:mixed, function:cartography, map-packet, region-map, caradril]
---

> **Secrecy classification:** Mixed. The Sunken Wards deep / Concord-Deep faint touch is DM-only. Never hand directly to the player.

## Region: Caradril (city-state + hinterland) (MF-005)

- **Local grid:** 0–100 (X east, Y south). (0,0) = NW of the region frame.
- **Full-continent bounds:** render-grid **X 31–38, Y 32–38** (NW cluster SE corner). Local (50,50) ≈ full (34,35) Caradril.
- **Campaign-grid anchor:** Caradril = campaign (82,80).
- **City detail:** the city's internal districts/bridges/landmarks are in `../../06_settlements/city_map_packets/CARADRIL_CITY_MAP.md`.

## Neighboring Regions

| Direction | Region |
|---|---|
| NW | Ashgarden Vale (southern-downs approach) |
| N | Tollwood (eastern approach) |
| W (water) | Verdance mouth / Pale Coast (sea-route) |
| SE | the Verdance Reaches (up-river, Ring 2) |

## Terrain Zones

| Zone | Type | Local | Notes |
|---|---|---|---|
| City (tiered banks) | urban | (50,50) | N-bank upper city, S-bank low city |
| Northern hinterland | farmland | (50,25) | the Vale/downs approach |
| Eastern hinterland | thinning forest-farmland | (75,40) | the Tollwood approach |
| The Stillwater | harbor-lake | (65,50) | E of the city |

## Water Features

| Feature | Type | Local | Campaign-grid | Flow |
|---|---|---|---|---|
| The Verdance | river | through (50,50) | (82,80) | runs W→E through the city; feeds the Stillwater |
| The Stillwater | harbor-lake | (65,50) | (80,78) | the city's port-lake (E end) |

## Roads / Routes

| Route | Local waypoints | Notes |
|---|---|---|
| Verdance Road (→ inland Orrun) | (50,50) Caradril→(90,80) SE up-river | to the Verdance Reaches / Glassmere (Ring 2) |
| South Road (← Vale) | (20,15) downs→(50,50) Caradril | from Orchardmere across the southern downs |
| East Road (← Tollwood) | (80,25) forest-edge→(50,50) Caradril | from Hartfell |
| Pale Coast Sea-Route (← Coast) | (60,80) Verdance-up→(65,50) Stillwater | the grand water-arrival |

## Bridges / Fords / Ferries

| Feature | Local | Notes |
|---|---|---|
| Caradril river-bridges (×2) + ferry | (50,50) | N/S bank crossings (see city packet) |
| Stillwater quays | (62,50) | the harbor frontage |

## Settlements

| Settlement | Type | Local | Campaign-grid | File |
|---|---|---|---|---|
| Caradril | city (major) | (50,50) | (82,80) | CARADRIL.md (+ city packet) |

> The hinterland has no built villages; it is approach-country (downs N/NW, forest-farmland N/E).

## Dungeons / Adventure Sites

| Site | Local | Campaign-grid | Surface marker | Player-map |
|---|---|---|---|---|
| D16 Sunken Wards Deep | (50,55) below city | (82,80) | the Sealgate (sealed stair) | urban (gate visible) |
| D17 Ashmarket Undercroft | (45,52) | (82,80) | Ashmarket cellars (interior) | urban |

## Ruins / Landmarks

City landmarks (Ledger Keep, Threshold Cathedral, Lamplighters' Hall, Sealed Archive, Magisters' Hall, the Sealgate) are positioned in the **city packet**.

## Local Labels (player map)

Caradril; the Verdance; the Stillwater; the Verdance Road (to inland Orrun); the southern downs (approach); the East Road approach.

## Player-Safe Layer

The city, the Verdance, the Stillwater, the three approaches + the up-river road, and an edge-arrow "to the Verdance Reaches & inland Orrun."

## DM-Only Layer (NEVER on the player map)

- The **Sunken Wards** are a dormant minor Concord relic-level (a cousin-node the Court's network faintly touches; M2/M7 faint).
- The **Sealed Archive** holds the clearest written proof of the harvest/deliberate Quietfall (M6/M9) — a building on the city map, but its contents are DM-only.
- Reke corresponds with someone in the Magisterium (lead, not a map feature).

## Unresolved Map Gaps

- The hinterland's exact extent toward the Verdance Reaches is a soft Ring-2 boundary (faint).

## Related Files

- [`../../06_settlements/CARADRIL.md`](../../06_settlements/CARADRIL.md) · [`../../06_settlements/city_map_packets/CARADRIL_CITY_MAP.md`](../../06_settlements/city_map_packets/CARADRIL_CITY_MAP.md) · [`../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md`](../../10_dungeons_and_ruins/ADVENTURE_SITE_CARTOGRAPHY_INDEX.md)
