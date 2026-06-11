# WORLD_MAP_PROMPTS.md — Campaign-Area (Northwestern Orrun) Image Generation Prompts

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [WORLD_MAP_AUTHORITY.md, WORLD_MAP_COORDINATES.md, WORLD_MAP_LAYERS.md, MAP_DESCRIPTION.md, FULL_WORLD_MAP_PROMPTS.md]
tags: [type:map, secrecy:mixed, function:cartography, image-prompts, orrun, campaign-area]
---

> **SCOPE NOTE (read first):** These prompts render the **current campaign area only** — the **northwestern corner cluster** of Orrun (Sundering Reach + Ring 1 + Caradril), NOT the whole continent. Earlier text below calls Prompt 1 a "full-world map"; that label is **historical and now means "campaign-area world map."** For true **full-continent / full-world** maps of Orrun, use **`FULL_WORLD_MAP_PROMPTS.md`** (5 prompts), which embeds this campaign-area map as its NW inset (Prompt 5 there = Prompt 3 here).

## AI Use

Four ready-to-use prompts for generating **campaign-area (northwestern Orrun)** maps. **Prompt 1 (campaign-area player-safe) and Prompt 3 (regional close-in) are safe to render and show the player.** **Prompt 2 (DM-only) and the DM toggles in Prompt 4 must never be shown to the player** — they expose hidden geography. Coordinates referenced are the campaign-area 0–100 grid in `WORLD_MAP_COORDINATES.md` (north=top, west=left), which is a ~3× zoom on the NW corner of the full-continent grid. Adapt label spelling exactly as registered in `NAMING_REGISTRY.md`.

**Secrecy reminder before generating:** never include the Concord Deep, the Under-Shrine/Drowned Keystone, the node-network lines, the Hollow Court, or any DM-only annotation on a player-facing map.

---

## Prompt 1 — Campaign-Area Player-Safe World Map (Northwestern Orrun) (SAFE TO SHOW)

> **Scope:** the campaign-area cluster only (NW Orrun). For the whole continent, use `FULL_WORLD_MAP_PROMPTS.md` Prompt 1.

> **Style/medium:** Hand-drawn fantasy cartography on aged parchment; ink linework with soft watercolor washes; subtle compass rose, decorative border, and a small legend. Cold, muted palette — peat-browns, fog-greys, sea-greys, pale orchard-greens, with the central basin rendered as dark water.
> **Orientation:** North at top, west at left. Compass rose top-right.
> **Scale reference:** Include a scale bar reading "approx. 12 days' travel corner to corner" and a small note "point-to-point overland on the old roads."
> **Area:** The northwestern quarter of the continent of Orrun (world of Vael) — a cold, wet shelf of land between mountains and sea.
> **Show and label:**
> - Center: the **Sundering Reach**, a fen-and-moor basin, with the town of **Hollowmere** on the rim of a wide dark flooded hollow (the **Hollowmere basin**, labeled "drowned Concord ruin").
> - North: the **Sunder Heights** (broken highlands), with the mining town **Harrowgast**; behind them, a far mountain wall labeled **the Highmark Spine**.
> - West: the **Pale Coast** (grey sea-cliffs, salt-pans), the port town **Wrackmouth**, the village **Cobble Strand**, a ruined cliff lighthouse labeled **the Drowned Lamp**, and offshore rocks labeled **the Skerries**; beyond, the open **Pale Sea**.
> - East: the **Tollwood** (deep old-growth forest) with the road-town **Hartfell**, the village **Coldhearth**, the hamlet **Tollstone Cross**, and a dark unlabeled forest heart marked "deep wood — shunned."
> - South: the **Ashgarden Vale** (orchards, hedged fields), the town **Orchardmere** on **Orchardmere lake**, the pilgrimage town **Saint Veddow's Rest**, and the village **Tilbrook**; the **Ammet** river winding through.
> - Southeast: the city-state **Caradril** on the **Verdance** river where it widens into the **Stillwater** harbor-lake; an edge-arrow "to inland Orrun."
> - Rivers: **Mirewend** (through the Reach), **Ammet** (Vale), **Verdance** (to Caradril and the sea).
> - Roads: the **South Road**, **East Road**, and **Pale Road** as old stone causeways radiating from the Reach; a dotted sea-route from Wrackmouth down-coast and up the Verdance to Caradril.
> - Reach gateway towns **Kettle Bridge** (east), **Saltmargin** (west), **Candlewick** (south); the central **Ashwalk Rest** waystation; the **Greyfens** marsh (SW of Hollowmere).
> **Do NOT show or label:** anything beneath the basin; any tunnels, node-links, or "network" lines; the Hollow Court; any hidden dungeon depths; the Verdance Reaches' interior detail (an edge-arrow only).
> **Color/shading conventions:** water dark, fens grey-brown, forest deep green, farmland soft green, highlands grey, danger-spots (Skerries, deep wood, Drowned Lamp) get a faint ominous wash but no explanation.
> **Dimensions:** landscape, ~4:3 or 3:2 aspect ratio.

## Prompt 2 — Campaign-Area DM-Only World Map (Northwestern Orrun) (NEVER SHOW THE PLAYER)

> **Scope:** the campaign-area cluster only (NW Orrun). For the DM-only whole continent, use `FULL_WORLD_MAP_PROMPTS.md` Prompt 2.

> **Style/medium:** Same parchment base as Prompt 1, but overlaid with a darker "occult survey" layer — fine red/charcoal annotation lines, dashed subterranean links, and a second legend marked "DM EYES ONLY."
> **Orientation:** North at top, west at left.
> **Scale reference:** Same as Prompt 1.
> **Area:** Same NW quarter of Orrun.
> **Show everything in Prompt 1, PLUS (DM-only overlay):**
> - The **Hollowmere basin** marked as the **keystone** of a buried network.
> - Dashed subterranean **network lines** linking the basin to: the **Deep Adit** (under Harrowgast), the **Sunken Tollhouse** (under Kettle Bridge), **Saint Veddow's Tomb** (under the Vale pilgrimage hill), the **Drowned Lamp** and **Skerry Shrine** (Coast), the **Sunken Wards** (beneath Caradril), and an oblique dashed line to the **Tollwood deep / Old Mast** marked "pre-Concord — built AROUND, not linked."
> - A depth-callout beneath the basin labeled **the Concord Deep** and, deepest, **the Under-Shrine / Drowned Keystone (endgame)**.
> - Faction influence shading (Cinder Ledger trade-web; Concord Remnant seat at Caradril; Mourners' strength in Vale/Coast; Gravecaller cells at the Greyfens, Hanging Oaks, and wrecker coves; Reachward Compact's thin grip).
> - Level-tier danger bands (green near Hollowmere/Vale → black at the keystone).
> **Color/shading conventions:** network links dashed red; pre-Concord sites marked with a distinct older glyph; warming nodes flagged with a small flame-mark.
> **Secrecy:** this map embodies the campaign's core secret. Store as DM-only; never display, summarize, or hand to the player.
> **Dimensions:** landscape, ~4:3.

## Prompt 3 — Parchment Regional Reference Map: The Reach + Ring 1 (SAFE TO SHOW)

> **Style/medium:** Hand-drawn, close-in parchment map with a heavier hand-lettered, "local ranger's sketch" feel; more detail, fewer flourishes; ink with light wash.
> **Orientation:** North at top, west at left. Small compass.
> **Scale reference:** "0.5–8 days' travel between sites on foot" scale note.
> **Area:** Cropped to the early-game play-area — the **Sundering Reach** at center and its three Ring 1 neighbors (Ashgarden Vale S, Tollwood E, Pale Coast W), with Caradril shown only as a labeled edge-arrow at the SE corner ("~10–12 days to Caradril").
> **Show and label (more granular than Prompt 1):**
> - All 8 Reach settlements (Hollowmere, Kettle Bridge, Saltmargin, Candlewick, Greywater Holm, Harrowgast, Reedford, the Ashwalk Rest).
> - Ring 1 hubs and villages (Orchardmere, Saint Veddow's Rest, Tilbrook; Hartfell, Coldhearth, Tollstone Cross; Wrackmouth, Cobble Strand).
> - The Greyfens, the Sunder Heights, the Hollowmere basin, the Mirewend and Ammet rivers, the Pale Sea, the Drowned Lamp, the Skerries (as a hazard label), the Old Mast deep wood (as a shunned-area label).
> - The South/East/Pale Roads as the safe threads; the Coast sea-route arrow.
> **Do NOT show or label:** subterranean anything, node-links, the keystone truth, dungeon depths.
> **Color/shading conventions:** same cold palette; mark each settlement with a simple icon (house = village, walled = town); mark old Concord ruins with a small broken-arch/shrine-stone icon.
> **Dimensions:** landscape or square, ~1:1 to 4:3. This is the map most useful for actual early play.

## Prompt 4 — Clean Functional AI / Reference Map (DM prep; base is safe, toggles are DM-only)

> **Style/medium:** Minimal, high-density **functional diagram** — flat colors, clean sans labels, thin connector lines, a node-and-edge feel rather than fantasy art. Think "annotated planning map," not parchment.
> **Orientation:** North at top, west at left.
> **Scale reference:** Grid overlay 0–100 on both axes (matches `WORLD_MAP_COORDINATES.md`); travel-day labels on each route edge.
> **Area:** The full mapped NW quarter.
> **Show (base, safe):** every region, settlement, river, road, sea, and major landmark as labeled nodes at their grid coordinates; route edges with day-counts and risk levels; a clean legend.
> **DM toggles (DM-only — keep on a separate layer/version, never in the player copy):** node-network links, Concord Deep + Under-Shrine depth-callout, faction influence overlay, mystery (M1–M9) site markers, level-tier danger coloring.
> **Color/shading conventions:** regions by flat tint; danger by border color (green→black); factions by hatch pattern; mystery sites by numbered pins. Maximize legibility and information density over beauty.
> **Secrecy:** generate the **base** version for shared reference; generate the **toggle** version DM-only and never display it to the player.
> **Dimensions:** square or 4:3; high resolution for label density.

---

## Generation Notes & Order

- **Scope reminder:** these four prompts render the **campaign-area cluster (NW Orrun)** only. For a **whole-continent** map, use `FULL_WORLD_MAP_PROMPTS.md`.
- **A campaign-area player-safe map can be generated now** from **Prompt 1** — all five cluster regions, all local bodies of water, mountains, forests, rivers, roads, and known settlements have authoritative positions (`WORLD_MAP_COORDINATES.md`) and registered names (`NAMING_REGISTRY.md`).
- **Recommended first map to generate: Prompt 3** (the Reach + Ring 1 regional reference) — it is the highest-value, lowest-risk map for actual early play, contains only high/medium-confidence positions, and exposes no secrets. Generate **Prompt 1** next for the broad player-facing world view.
- **Generate Prompt 2 and the Prompt 4 DM-toggle version for DM prep only.** Store them outside any player-shared space.
- **Low-confidence placeholders** (Verdance Reaches, Highmark passes) should be drawn faint/edge-only until expansion passes pin them down.

## Related Files

- [`WORLD_MAP_AUTHORITY.md`](WORLD_MAP_AUTHORITY.md) · [`WORLD_MAP_COORDINATES.md`](WORLD_MAP_COORDINATES.md) · [`WORLD_MAP_LAYERS.md`](WORLD_MAP_LAYERS.md) · [`MAP_DESCRIPTION.md`](MAP_DESCRIPTION.md)
