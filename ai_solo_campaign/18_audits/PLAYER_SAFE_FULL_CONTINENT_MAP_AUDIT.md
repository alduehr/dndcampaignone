# Audit Report: Player-Safe Full-Continent Map — Settlement Distribution

---
type: audit
secrecy: player-safe
status: static
region: Orrun
related: [../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md, ../04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md, ../04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md, ../04_world_atlas/FULL_WORLD_MAP_COORDINATES.md]
tags: [type:audit, secrecy:player-safe, cartography, full-continent, settlement-anchors, map-audit]
---

## Scope

Audit of the cartographic precision pass that added player-safe far-continent settlement/social anchors with coordinates and render rules. Files reviewed: `FULL_CONTINENT_SETTLEMENT_ANCHORS.md` (new), `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` (§8.5 added), `PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md` (§D.5 + audit checks added), against `FULL_WORLD_MAP_COORDINATES.md`, `FULL_WORLD_MAP_AUTHORITY.md`, `NAMING_REGISTRY.md`.

## Summary

The anchor layer is healthy. All 12 far-continent placeholder regions now have player-safe settlement/social anchors with full-continent coordinates spread within their region footprints. NW settlements are correctly clustered in the northwest and unchanged. No DM-only locations, no invented names, no duplicate-Caradril, no centroid-stacking. The map will now show settlements distributed across the whole continent rather than bunched in the NW.

## Audit Checks

| # | Check | Result | Notes |
|---|---|---|---|
| 1 | Are NW campaign settlements correctly clustered in the northwest? | PASS | All 17 NW anchors sit in X 8–40 / Y 8–42; coordinates mirrored unchanged from `FULL_WORLD_MAP_COORDINATES.md`. |
| 2 | Are far-continent settlement/social anchors present across the rest of the map? | PASS | 36 far-continent anchors across center, south, east, north, and southeast. Center (Glassmere ~55,50; Crownmouth ~60,54; Hethemoot ~71,39), south (Marrowmoot ~50,66; Fenward ~57,82; Calderport ~65,89; Brackhold ~57,68; Sunhollow ~44,80), north (Cold Springs ~45,16; Brask's Hold ~73,17), southeast (Ashfast ~80,62). |
| 3 | Does every far-continent region have at least one visible reference-map anchor? | PASS | All 12 regions have a hub with `render_on_reference_map = true`. |
| 4 | Are high-density regions visually denser than wilderness/steppe/ruin regions? | PASS | Settled regions (Glassmere 4, Verdance 4, Hollow Gulf 3, Hethewald 4, Marrowdowns 4, Sallowmarch 3) carry more anchors than wild/forbidden regions (Wender 3, Karran 4, Emberfell 3, Saltmere 3, Heartlands 2, Sunmark 3). Heartlands deliberately sparsest (forbidden ruin). Density gradient documented in the anchors file. |
| 5 | Are anchors placed within their region footprints, not all at centroids? | PASS | Each region's anchors are offset within its `approx_bounds` (e.g. Verdance hub 41,41 / 45,39 / 39,45 / 43,43 within X 38–48, Y 38–48). |
| 6 | Is Caradril rendered exactly once? | PASS | Single anchor `nw.caradril` (34,35); flagged "render exactly once." No region/route-anchor duplicate. |
| 7 | Is Stillwater shown as a harbor-lake at Caradril? | PASS | Handled by the parent manifest §4 (`water.stillwater` adjacent to Caradril, no duplicate label). The anchor layer adds no second Caradril/Stillwater marker. |
| 8 | Are any non-rendered local anchors incorrectly shown as cities? | PASS | 5 `non_rendered_local_anchor` rows (Lowwater, The Floor, The Three Bridges, The Foreign Quarter, The Fever Channels) all carry `render_on_reference_map = false` and `render_on_art_map = false`; documented as hub-internal districts / diffuse areas. |
| 9 | Are any light anchors mislabeled as major cities? | PASS | Only Glassmere, Calderport, Ashfast, and Caradril are `settlement_major`. All others are `settlement_secondary` / `travel_anchor` / `social_anchor` / `ruin_edge_anchor`. Seasonal camps and groves (Cold Springs, Sunhollow) explicitly tagged as camp/grove hubs, not cities. |
| 10 | Are any invented settlement names present? | PASS | Zero. Every name is registered in `NAMING_REGISTRY.md` (Stage 9.5 light anchors) and used in the NPC/quest files. No new proper nouns coined. |
| 11 | Are any DM-only locations shown? | PASS | None. No Concord Deep, Under-Shrine, Drowned Keystone, or Hollow Court. Ruin-edge anchors (Old Iron forts, Drowned Towns, Pilgrim Camps, Old Holds, Barrow-Fields) explicitly show only living camps, never the ruin truth or any network/depth annotation. |

## Critical Findings

None.

## High Findings

None.

## Medium Findings

None.

## Low Findings

| Issue | File(s) | Why It Matters | Recommended Fix |
|---|---|---|---|
| No machine-readable JSON manifest exists | `04_world_atlas/` | The pass anticipated a `player_safe_full_continent_render_manifest.json`, but none exists in the repo. Markdown is the only source. | Optional: if a JSON render pipeline is later added, mirror Tables 1–2 of the anchors file into it. Not required now. |

## Exposed Secrets

None. All anchor content is player-safe; DM-only locations are explicitly excluded and called out in the anchors file's Secrecy Rules.

## Distribution Verdict

The full-continent map can now render settlement markers across all of Orrun. The NW remains correctly dense; the settled center/south reads as second-densest; the wild steppe, volcanic highland, and forbidden ruin-country read as sparse. This resolves the original problem (settlements bunched in the northwest).

## Recommended Fix Order

1. None blocking. The generation packet (§D.5) and manifest (§8.5) are ready for new full-continent map renders.

## Related Files

- [`../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md`](../04_world_atlas/FULL_CONTINENT_SETTLEMENT_ANCHORS.md)
- [`../04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`](../04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md)
- [`../04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md`](../04_world_atlas/PLAYER_SAFE_FULL_CONTINENT_GENERATION_PACKET.md)
- [`../04_world_atlas/FULL_WORLD_MAP_COORDINATES.md`](../04_world_atlas/FULL_WORLD_MAP_COORDINATES.md)
