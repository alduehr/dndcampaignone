# Widdershin Cave — Map Specifications

Non-canon, standalone — see [`../README.md`](../README.md) and
[`WIDDERSHIN_CAVE.md`](WIDDERSHIN_CAVE.md) for the full adventure this map
supports.

Two things are specified here: (1) a schematic dungeon layout usable
directly at the table or dropped into a VTT, and (2) an image-generation
prompt for a poster-style overview map, written in the same copy-paste-ready
format this repo's own cartography files use for the main campaign.

---

## 1. Schematic Layout

Cross-section logic: the cave descends gently from the sea-arch entrance
(Zone 1, sea level) down and inward to the vault (Zone 5, slightly below
sea level, kept dry by the stone door's seal) and back up into the open
sea-cavern (Zone 6, sea level, tidal). North is nominal — orient however
suits your table; the cave doesn't need to match any real-world compass.

| Zone | Name | Approx. size | Connects to | Elevation / water | Key contents |
|---|---|---|---|---|---|
| 1 | Tidewrack Landing | 30 ft × 40 ft, irregular | Zone 2 (main path); cliff-route entrance also lands here | Sea level; tidal — impassable except at dead-low tide via the sea-arch | Wreckage dressing, belt-buckle clue |
| — | Cliff Route (alternate entrance) | N/A — a route, not a room | Clifftop path → Zone 3 directly | Bypasses tidal timing entirely | DC 13 Athletics or trivial with rope |
| 2 | The Tide Pools | 50 ft × 35 ft, uneven floor | Zone 1 ↔ Zone 3 | Sea level; ankle-to-chest-deep pools, one dry stone spine crossing | 2 reef crabs, strongbox (22 gp + Log Fragment #1) |
| 3 | The Wreck Gallery | 60 ft × 45 ft, high ceiling | Zone 2 ↔ Zone 4; cliff route enters here | Sea level; mostly dry, sandy floor | The *Widdershin* wreck, Tam (ghost), Log Fragment #2, bioluminescent fungus lighting |
| 4 | The Smuggler's Cache | 25 ft × 25 ft room + 20-ft single-file tunnel approach | Zone 3 ↔ Zone 5 | Sea level; dry | 3 drowned skeletons (choke-point fight in the tunnel), strongbox (35 gp), tide-chart disc |
| 5 | The Rune-Dial Vault | 30 ft diameter, round | Zone 4 ↔ Zone 6 (only after puzzle solved) | Slightly below sea level; kept dry by the sealed door | 3-dial tide puzzle on the far door |
| 6 | The Widdershin Deep | 70 ft × 60 ft, cavern open to the sea on one wall | Zone 5 only (dead end otherwise) | Sea level; tidal, open water on one side, raised dry stone shelf (Locke's throne + altar) | Boss fight: Captain Locke; sea-chest treasure (140 gp, cutlass, Widdershin Coin); Fathom Eye idol on the altar |

**Traversal note:** the cave is a mostly linear string of pearls
(1→2→3→4→5→6) with one shortcut (the cliff route skips 1 and 2, landing in
3). This is intentional — a one-shot benefits from a layout a table can
hold in their head without a grid reference, while the shortcut still gives
players a real choice to make during the "Getting In" beat.

---

## 2. Battle-Map Notes (the three tactical rooms)

Grid assumed at 5 ft/square, standard D&D VTT convention.

### Zone 2 — The Tide Pools (10×7 squares)
- Irregular pool shapes covering roughly 60% of the floor; mark pools as
  difficult terrain (ankle-deep) or hazardous/swim-required (chest-deep) —
  vary it, don't make every pool the same depth.
- One clear "dry spine" of stone running roughly diagonally corner-to-corner
  — the Stealth/Acrobatics bypass route mentioned in the adventure text.
  Make this visually obvious on the map (lighter stone color).
- Crab starting positions: in the two largest pools, out of the dry spine's
  path — they should have to close distance, not ambush from adjacent.

### Zone 4 — The Smuggler's Cache (5×4 squares tunnel + 5×5 square room)
- The approach tunnel is **exactly 1 square wide** for its full 4-square
  length — this is the choke point and it should read as one on the map,
  not just in the text. **Stays 1 square wide for any level-1 party,
  regardless of size** (the reduced skeleton counts at level 1 keep it
  snappy even with six characters waiting in line). **For level 2+ parties
  of size 4 or more,** per [`PARTY_AND_LEVEL_SCALING.md`](PARTY_AND_LEVEL_SCALING.md)'s
  tunnel-width rule, widen it to **2 squares** so the fight doesn't bench
  most of the table behind a single front-liner — draw both widths if
  you're prepping the map ahead of knowing your final table's level.
- The room itself opens up to 5×5 once through the tunnel, with 3–4
  crate/barrel clusters as light cover (+2 AC, half cover rules) and one
  fallen crate pinning the tide-chart disc (flavor, not mechanical cover).
- Skeleton starting positions: one just inside the tunnel mouth (first to
  engage), two staged in the room behind — the geometry should make "fight
  them one at a time in the tunnel" the obviously correct read.

### Zone 6 — The Widdershin Deep (14×12 squares)
- Roughly two-thirds open water (difficult terrain even before Tide Call;
  swimming rules apply), one-third raised dry stone shelf along the back
  wall at a height of about 3 ft (minor elevation — treat climbing on/off
  as free with a hand free, or DC 8 Athletics if rushed).
- Locke's throne and the tide-altar (holding the Fathom Eye) both sit on
  the raised shelf, roughly 15 ft apart from each other.
- The sea-arch opening is centered on the far wall — waves/tide visual
  motif here, and it's the room's "outside" reference point.
- When Tide Call triggers, treat the **entire open-water two-thirds** as
  affected — mark it clearly if playing on a physical or digital grid so
  the surge's scope is unambiguous to the player in the moment.

---

## 3. Overview Map — Image-Generation Prompt

Copy-paste ready for an AI image generator. Written in the same
parchment-cartography style this repo uses for its own settlement and
region map packets — no campaign-canon labels included, since this site
doesn't exist in that world's authored geography.

> **Style/medium:** Hand-drawn fantasy dungeon map on aged, slightly
> water-stained parchment; ink linework with a light blue-green watercolor
> wash for water features; a small decorative compass rose and a
> hand-lettered title banner reading "Widdershin Cave."
> **Perspective:** Top-down schematic cross-section, cave-survey style —
> like a hand-drawn spelunker's map, not a photorealistic render.
> **Orientation:** Sea-arch entrance at the bottom/south edge, cave
> extending north and slightly downward in elevation toward the vault, then
> opening back up into a large sea-cavern at the top/north edge.
> **Show and label, left to right/south to north:**
> - The sea-arch entrance (Zone 1) with wave-line hatching indicating the
>   tideline, and a small dotted alternate path along the cliff face to the
>   side labeled "cliff route."
> - A pool-dotted cavern (Zone 2) rendered with small blue-wash tide-pool
>   shapes and one clear unshaded "dry spine" path crossing it.
> - A wide chamber (Zone 3) with a small sketched shipwreck silhouette and
>   soft green speckling to suggest bioluminescent fungus.
> - A narrow single-width tunnel (Zone 4 approach) opening into a small
>   square room with crate/barrel icon clusters.
> - A round chamber (Zone 5) with a door glyph — three concentric ring
>   shapes with small tick-marks (representing the dial puzzle) inset into
>   the door.
> - A large open cavern (Zone 6) with a wide arch opening to open water on
>   its far edge, a small raised shelf with a chair icon (the throne) and a
>   small round altar icon beside it.
> **Color/shading conventions:** parchment tan/cream base, ink-black
> linework, blue-green wash for all water and tide features, a faint
> ominous grey-green wash creeping in only around Zone 6 to mark it as the
> climax space.
> **Do NOT include:** any text/labels beyond the six zone names and the
> title banner — no lore text, no read-aloud boxes, no references to any
> other Orrun location or faction. This map should read as fully
> self-contained.
> **Dimensions:** portrait or landscape, ~4:3 aspect ratio, single page.
