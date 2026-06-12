# FULL_WORLD_MAP_PROMPTS.md — Full-World Image Generation Prompts

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: []
level_range: 1-20
related: [FULL_WORLD_MAP_AUTHORITY.md, FULL_WORLD_MAP_COORDINATES.md, FULL_WORLD_MAP_LAYERS.md, WORLD_MAP_PROMPTS.md]
tags: [type:map, secrecy:mixed, function:cartography, image-prompts, orrun, full-continent]
---

## AI Use

Five ready-to-use prompts for generating **full-continent / full-world** maps of Orrun (world of Vael). **Prompts 1, 3, and 5 are safe to render and show the player.** **Prompt 2 (DM-only) and the DM toggles in Prompt 4 must never be shown to the player** — they expose hidden geography. Coordinates referenced are the full-continent 0–100 grid in `FULL_WORLD_MAP_COORDINATES.md` (north=top, west=left). Adapt label spelling exactly as registered in `NAMING_REGISTRY.md`.

**Secrecy reminder before generating:** never include the Concord Deep, the Under-Shrine/Drowned Keystone, the node-network lines, the Hollow Court, warming-node marks, or any "the far ruins ARE the machine" implication on a player-facing map. The endgame is **vertical, beneath the NW campaign cluster** — never draw it as a distant land.

For the **campaign-area-only** maps (the most-used play maps), use `WORLD_MAP_PROMPTS.md` (the Reach + Ring 1 + Caradril zoom). This file is for the **whole continent**.

---

## Prompt 1 — Player-Safe Full-World / Full-Continent Map (SAFE TO SHOW)

> **Style/medium:** Hand-drawn fantasy cartography on aged parchment; ink linework with soft watercolor washes; compass rose, decorative border, and a legend. Palette graded along a cold-to-warm axis: cold greys, peat-browns, and sea-greys in the northwest; greens through the settled center; warm ochres, ash-greys, and obsidian-blacks in the volcanic southeast; warm blues in the southern sea.
> **Orientation:** North at top, west at left. Compass rose top-right.
> **Scale reference:** Scale bar reading "approx. 2–3 months' travel corner to corner." The NW campaign frontier (Sundering Reach, Ring 1 regions, Pale Coast, Tollwood, Ashgarden Vale, Caradril) is shown directly on the main continent map, with somewhat higher local detail, NOT as an inset, box, overlay, or separate mini-map.
> **Area:** The entire continent of **Orrun** (world of **Vael**) — a large continent that tilts from a cold, broken, ruin-strewn **northwest frontier** to a warm, rich, settled **south and southeast**.
> **Show and label:**
> - **NW corner (the campaign frontier, drawn directly on the main map at somewhat higher local detail — NOT as an inset or box):** the **Sundering Reach** with **Hollowmere** on its dark flooded basin; the **Sunder Heights** (N) below the **Highmark Spine** mountain wall; the **Pale Coast** and **Pale Sea** (W) with **Wrackmouth**; the **Tollwood** (E) with **Hartfell**; the **Ashgarden Vale** (S) with **Orchardmere**; and the city-state **Caradril** at the cluster's SE edge, on the **Verdance** river and **Stillwater**.
> - **North:** the **Sunder Ocean** along the top; the **Highmark Spine** running NW; the cold **Wender Steppe** (open grassland) beyond the Spine; the jagged **Karran Teeth** range and the **Karran Marches** (NE outlaw frontier).
> - **Center:** the great **Greatspine / Sundering Wall** cordillera splitting the continent NW–SE; the **Verdance Reaches** and the river-city **Glassmere League** on the **Glasswater** river; the **Hethewood** forest and **Hethewald Free Holds** (E) along the **Hethe** river.
> - **South-central:** the **Marrowdowns** (chalk downs); the dying inland **Saltmere** sea ringed by the **Ghostmark Range** and the **Bonepan Flats**; the **Saltmere Reaches**.
> - **Southeast:** the **Emberfells** (volcanic highlands, ash-plains, vents) and the **Emberfell Theocracy / the Ashfast**; the **Cindern Waste** badland; the **Glass Coast** of black sea-stacks; the warm **Calm Reach** sea.
> - **South:** the **Sunmark** (warm forest & sacred groves); the **Mardenflow** river and the **Sallow Marches** delta; the **Sallowmarch Protectorate**; the **Hollow Gulf** and its **Hollow Gulf Ports**.
> - **A distant labeled ruin-country** in the central-SE: "**the fallen Concord heart — ruins, contested**" (the Concord Heartlands), drawn as broken towers, NOT explained.
> - **Long-distance routes** as threads: the Verdance Road, the Glasswater Run, the Greatspine Crown Road (marked "contested"), the Salt Road, the Hethe Tollway, the Pale Coast Sea-Route, and dotted South Sea Lanes with edge-arrows "to overseas lands."
> **Render authority:** Use `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md` as the label authority. Do not generate labels from any other table if they would duplicate a manifest feature. Every feature with `duplicate_rule: render exactly once` must appear no more than once. Route-anchor labels, region-context labels, and alias labels must not be rendered as separate locations unless they have their own canonical manifest entry.
> **Do NOT show or label:** anything subterranean; node-links or network lines; the Concord Deep; the Under-Shrine/keystone; the Hollow Court; any implication that the far ruins are a "machine"; the interiors of placeholder regions (label + tinted area only, drawn faint).
> **Color/shading conventions:** campaign NW = crisp detail; far regions = softer, "less-surveyed" linework; rumored ruins (Cindern, Drowned Steps, Saltmere towns, Concord heart) get a faint ominous wash but no explanation.
> **Dimensions:** landscape, ~3:2 or 16:10 aspect ratio; high resolution for continental label density.
>
> **Before generating:** verify labels against Section 4 (canonical feature table) and Section 7 (duplicate-prone audit) of `PLAYER_SAFE_FULL_CONTINENT_RENDER_MANIFEST.md`. **After generating:** run the Section 8 audit checklist.

## Prompt 2 — DM-Only Full-World / Full-Continent Map (NEVER SHOW THE PLAYER)

> **Style/medium:** Same parchment base as Prompt 1, overlaid with a darker "occult survey" layer — fine red/charcoal annotation, dashed subterranean links, a second legend marked "DM EYES ONLY."
> **Orientation / scale / area:** Same as Prompt 1 (full continent).
> **Show everything in Prompt 1, PLUS (DM-only overlay):**
> - In the **NW campaign cluster only**, the **harvest node-network**: dashed lines from the **Hollowmere basin keystone** to the **Deep Adit** (Harrowgast), **Sunken Tollhouse** (Kettle Bridge), **Saint Veddow's Tomb** (Vale), **Drowned Lamp / Skerry Shrine** (Coast), **Sunken Wards** (Caradril), and an oblique line to the **Tollwood Old Mast** marked "pre-Concord — built AROUND, not linked."
> - A **depth-callout beneath the NW basin** labeled "**the Concord Deep**" and, deepest, "**the Under-Shrine / Drowned Keystone (ENDGAME — vertical, beneath Hollowmere)**." CRITICAL: keep this callout in the NW corner; do NOT spread network lines across the continent.
> - The far **Concord Heartlands** annotated "Concord's fallen SURFACE capital — ruin, NOT the keystone"; the **Cindern Waste / Drowned Steps / Saltmere drowned towns** annotated "pre-Concord echo / surface ruin — corroborates theme, NOT a node."
> - Faction continental reach (Cinder Ledger trade-web NW→central→S; Concord Remnant reaching toward the Heartlands; Mourners' folk-network in the settled south; Wardens NW-only; Gravecaller cells NW + rumored far echoes).
> - Level-tier danger bands (green NW core → black at the NW keystone; orange interior; red far frontiers; striped "beyond campaign" overseas).
> - Off-map notes: "Surren (S, overseas), Iron Skards (N, overseas), Sundered Isles (far W) — placeholder, non-campaign"; "other surviving Custodians: undefined, off-map."
> **Color/shading conventions:** network links dashed red (NW only); pre-Concord/echo sites a distinct older glyph; warming NW nodes flagged with a small flame-mark.
> **Secrecy:** embodies the campaign's core secret. DM-only; never display, summarize, or hand to the player.
> **Dimensions:** landscape, ~3:2.

## Prompt 3 — Parchment-Style Full-World Map (in-world artifact; SAFE TO SHOW)

> **Style/medium:** Heavily aged, hand-drawn **in-world parchment artifact** — as if a Caradril cartographer or a Concord-era survey copy: foxed and water-stained edges, faded ink, a hand-lettered title cartouche ("Orrun, as the Old Roads Knew It"), sea-monster doodles in the oceans, and **deliberately vague/blank far quarters** ("here the maps grow uncertain"). Looks like a prop the player could be handed at a table.
> **Orientation:** North at top, west at left. Ornate compass rose.
> **Scale reference:** An old-fashioned dividers-and-leagues scale; a note "by the old reckoning, a season's road end to end."
> **Area:** All of **Orrun**, but rendered as a **period artifact** — the NW frontier and the settled south/center reasonably detailed; the far north (Wender Steppe, Iron Skards), the deep volcanic SE, and the overseas edges drawn faint, partial, or marked "unsurveyed / by report only."
> **Show and label (player-safe only):** the same player-safe regions, seas, ranges, rivers, forests, and routes as Prompt 1, but with an **antique, incomplete feel** — some far regions labeled only by rumor-name; the Concord Heartlands shown as a romantic ruin-vignette ("the Old Crown, fallen").
> **Do NOT show or label:** anything subterranean; node-links; the keystone; the Hollow Court; warming marks; any "machine" implication. The artifact should look like genuine in-world knowledge, which does NOT include the secret.
> **Color/shading conventions:** sepia/aged parchment; muted inks; the cold-to-warm palette muted under the aging; decorative not clinical.
> **Dimensions:** landscape or near-square, ~4:3; suitable for sharing with the player as a found map.

## Prompt 4 — Clean Functional AI / Reference Map (DM prep; base safe, toggles DM-only)

> **Style/medium:** Minimal, high-density **functional diagram** — flat region tints, clean sans labels, thin connector lines; a node-and-edge "planning map," not fantasy art.
> **Orientation:** North at top, west at left.
> **Scale reference:** Grid overlay 0–100 on both axes (matches `FULL_WORLD_MAP_COORDINATES.md`); a boxed NW-corner sub-grid note "campaign cluster = X 8–40, Y 8–42 (see campaign-area grid for ~3× zoom)."
> **Area:** The full continent.
> **Show (base, safe):** every region (campaign + placeholder), sea, range, river, forest, badland, steppe, and major route as labeled nodes/areas at their grid coordinates; route edges with rough leg-times and risk; a clean legend; placeholder regions clearly tagged "(placeholder — not yet built)."
> **DM toggles (DM-only — separate layer/version, never in the player copy):** the NW node-network links and Concord Deep / Under-Shrine depth-callout; faction continental-reach overlay; mystery (M1–M9) site markers (clustered NW + faint far-corroboration pins); level-tier danger coloring; off-map landmass notes.
> **Color/shading conventions:** regions by flat tint (cold-to-warm by axis); danger by border color (green→black); factions by hatch; mystery sites by numbered pins. Maximize legibility and information density.
> **Secrecy:** generate the **base** version for shared reference; generate the **toggle** version DM-only and never display it to the player.
> **Dimensions:** square or 4:3; high resolution for label density.

## Prompt 5 — Current Campaign Area Inset Map (SAFE TO SHOW)

> **Style/medium:** Hand-drawn, close-in parchment map with a "local ranger's sketch" feel — more detail, fewer flourishes; ink with light wash. (This is the day-to-day play map; identical in spirit to Prompt 3 in `WORLD_MAP_PROMPTS.md`.)
> **Orientation:** North at top, west at left. Small compass.
> **Scale reference:** "0.5–8 days' travel between sites on foot."
> **Area:** Zoomed in to the **NW campaign cluster** — the **Sundering Reach** at center with all 8 settlements (Hollowmere, Kettle Bridge, Saltmargin, Candlewick, Greywater Holm, Harrowgast, Reedford, the Ashwalk Rest); **Ashgarden Vale** (S: Orchardmere, Saint Veddow's Rest, Tilbrook); **Tollwood** (E: Hartfell, Coldhearth, Tollstone Cross); **Pale Coast** (W: Wrackmouth, Cobble Strand); and **Caradril** at the SE corner (labeled, "~10–12 days").
> **Show and label:** the Greyfens, Sunder Heights, Hollowmere basin, the Mirewend and Ammet rivers, the Pale Sea, the Drowned Lamp and Skerries (hazard labels), the Old Mast deep wood (shunned-area label); the South/East/Pale Roads and the Coast sea-route arrow; old Concord ruins with a small broken-arch icon.
> **Do NOT show or label:** subterranean anything, node-links, the keystone truth, dungeon depths.
> **Color/shading conventions:** cold palette (greys, peat-browns, fog-whites); house-icon = village, walled-icon = town.
> **Dimensions:** landscape or square, ~1:1 to 4:3. The highest-value map for actual early play.

---

## Generation Notes & Order

- **A true full-continent player-safe map of Orrun can now be generated** from **Prompt 1** — all regions (campaign + placeholder), all seas, ranges, rivers, forests, and long-distance routes have authoritative grid positions (`FULL_WORLD_MAP_COORDINATES.md`) and registered names (`NAMING_REGISTRY.md`). Far regions are placeholders and should be drawn faint until built.
- **Recommended first map to generate: Prompt 5** (the current campaign area inset) — it is the highest-value, lowest-risk, most-played map, contains only high/medium-confidence positions, and exposes no secrets. Then **Prompt 1** for the broad player-facing continent, and **Prompt 3** as the in-world parchment artifact to hand the player.
- **Generate Prompt 2 and the Prompt 4 DM-toggle version for DM prep only.** Store them outside any player-shared space.
- **Low-confidence placeholders** (everything beyond the NW cluster + the Verdance Reaches) should be drawn faint/low-detail until expansion passes pin them down.

## Related Files

- [`FULL_WORLD_MAP_AUTHORITY.md`](FULL_WORLD_MAP_AUTHORITY.md) · [`FULL_WORLD_MAP_COORDINATES.md`](FULL_WORLD_MAP_COORDINATES.md) · [`FULL_WORLD_MAP_LAYERS.md`](FULL_WORLD_MAP_LAYERS.md)
- [`WORLD_MAP_PROMPTS.md`](WORLD_MAP_PROMPTS.md) (campaign-area prompts)
