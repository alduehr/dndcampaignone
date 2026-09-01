# Widdershin Cave — Map Specifications

Non-canon, standalone — see [`../README.md`](../README.md) and
[`WIDDERSHIN_CAVE.md`](WIDDERSHIN_CAVE.md) for the full adventure this map
supports.

Three things are specified here: (1) a schematic dungeon layout usable
directly at the table or dropped into a VTT, (2) battle-map notes for the
tactical rooms, and (3) an image-generation prompt for a poster-style overview
map, written in the same copy-paste-ready format this repo's own cartography
files use for the main campaign.

**The geometry here has not changed since the map was first drawn** — same six
zones, same linear 1→2→3→4→5→6 string, same cliff-route shortcut into Zone 3,
same 1-square tunnel, same dry spine, same throne-and-altar shelf. Later fixes
to the adventure's physics, balance, and Zone 4 participation were all made in
text so that any map already generated from §3 stays accurate.

---

## 1. Schematic Layout

Cross-section logic: **the cave floor rises as it runs inland.** The sea-arch
(Zone 1) is the low point and the only part of the cave the tide actually
closes. Zones 2–5 sit **above the high-water line**, which is why Zone 3 and
Zone 4 are bone dry after thirty years while Zone 2 keeps standing pools —
water trapped in the hollows by the spring tides, exactly the way real tide
pools work. Zone 5 is the high point; a short flight of steps leads back
**down** from its far door into Zone 6, which is open to the ocean on one wall
and always tidal. That stair is the whole reason the vault stayed dry.

*(This elevation logic is invisible on a top-down map — it exists so the
adventure's physics hold up, not to change any drawn geometry.)*

North is nominal — orient however suits your table; the cave doesn't need to
match any real-world compass. Foe counts and treasure below are the base
module's **four-characters-at-level-1** baseline; see
[`PARTY_AND_LEVEL_SCALING.md`](PARTY_AND_LEVEL_SCALING.md) for other tables.

| Zone | Name | Approx. size | Connects to | Elevation / water | Light | Key contents |
|---|---|---|---|---|---|---|
| 1 | Tidewrack Landing | 30 ft × 40 ft, irregular | Zone 2 (main path); cliff-route entrance also lands here | Cave's low point; tidal — impassable except at dead-low tide via the sea-arch | Dim | Wreckage dressing, belt-buckle clue, seaward weathering (wind hint) |
| — | Cliff Route (alternate entrance) | N/A — a route, not a room | Clifftop path → Zone 3 directly | Bypasses tidal timing entirely | — | DC 13 Athletics or trivial with rope; the rope stays as an exit |
| 2 | The Tide Pools | 50 ft × 35 ft, uneven floor | Zone 1 ↔ Zone 3 | Above high water; ankle-to-chest-deep trapped pools, one dry stone spine crossing | Dim (algae) | 5 reef crabs, strongbox (22 gp + Scrimshaw Fragment #1) |
| 3 | The Wreck Gallery | 60 ft × 45 ft, high ceiling | Zone 2 ↔ Zone 4; cliff route enters here | Above high water; dry, sandy floor | Dim (fungus) | The *Widdershin* wreck, Tam (ghost), Scrimshaw Fragment #2, smashed skeleton + boarding maul (vulnerability hint); **half the Zone 4 fight spills out here** |
| 4 | The Smuggler's Cache | 25 ft × 25 ft room + 20-ft single-file tunnel approach | Zone 3 ↔ Zone 5 | Above high water; dry | Dark | 4 drowned skeletons, strongbox (35 gp), silver flask, 2 potions of healing, Tam's knucklebone, tide-chart disc, salvageable salt barrels (40–60 gp), **the empty idol-shaped travelling-case** (motive clue) |
| 5 | The Rune-Dial Vault | 30 ft diameter, round | Zone 4 ↔ Zone 6 (only after puzzle solved) | Cave's high point; dry because it is above the tide, not because of the seal | Dark | 3-dial tide puzzle (counterclockwise-ratcheted) on the far door; steps down to Zone 6 beyond |
| 6 | The Widdershin Deep | 70 ft × 60 ft, cavern open to the sea on one wall | Zone 5 only (dead end otherwise) | Sea level; tidal, open water on one side, raised dry stone shelf (Locke's throne + altar) | Dim | Boss fight: Captain Locke, **carrying the Fathom Eye on his belt**; the tide-altar on the shelf stands **empty**; sea-chest treasure (300 gp, cutlass, 2 Widdershin Coins) |

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
- A grappling crab drags its catch toward the nearest chest-deep pool, so
  it's worth knowing which pools those are before initiative starts.

### Zone 4 — The Smuggler's Cache (1×4 square tunnel + 5×5 square room)
- The approach tunnel is **exactly 1 square wide for its full 4-square
  length**, at every party size and level. This is the choke point and it
  should read as one on the map. **Do not widen it** — the participation
  problem is solved by deployment, not geometry, so the drawn map never needs
  to change.
- The room itself opens up to 5×5 once through the tunnel, with 3–4
  crate/barrel clusters as light cover (+2 AC, half cover rules) and one
  fallen crate pinning the tide-chart disc (flavor, not mechanical cover).
- **Skeleton deployment (the important part):** one holds the tunnel mouth,
  **two push out past it into Zone 3** within a round or two and fight in the
  open gallery, and any remaining skeletons shoot shortbows down the tunnel
  from inside the room. That turns the chokepoint into a tactic the party can
  *choose* rather than a queue that benches half the table, and it uses Zone 3
  — already mapped, large, and the best-looking room in the cave — as the real
  battlefield. At level 3+ the Bosun's Bones elite is the one in the tunnel.

### Zone 3 — The Wreck Gallery (12×9 squares)
Not originally a battle map, but half the Zone 4 fight now happens here, so
prep it lightly:
- The *Widdershin*'s hull runs along one long wall — treat it as full cover
  from behind, difficult terrain to climb over, and a 5-ft elevation for
  anyone who gets up on the canted deck.
- Open sand across the middle. This is where the two pushed-out skeletons
  should end up, in reach of everybody.
- Tam sits on the broken rail and does not move, take up space, or block
  anything.

### Zone 6 — The Widdershin Deep (14×12 squares)
- Roughly two-thirds open water (difficult terrain even before Tide Call;
  swimming rules apply), one-third raised dry stone shelf along the back
  wall at a height of about 3 ft (minor elevation — treat climbing on/off
  as free with a hand free, or DC 8 Athletics if rushed).
- Locke's throne and the tide-altar both sit on the raised shelf, roughly
  15 ft apart. **The altar is empty** — Locke carries the Fathom Eye on his
  belt, held there by a black thread of water running off the shelf into the
  deep.
- **The altar is a defended objective, so mark its square.** The idol can't be
  taken off Locke until he's below half HP, and returning it means a character
  standing on that square holding it for **three consecutive rounds** while he
  attacks them. The 15 ft between throne and altar is the most important
  distance on the map, and the shelf-to-water edge is the second — Tide Call
  and the Tier B lair action both push toward the arch, i.e. *away from the
  altar.* That's not a coincidence; play it that way.
- The sea-arch opening is centered on the far wall — waves/tide visual motif
  here, it's the room's "outside" reference point, and it's the direction
  everything gets pushed.
- **Tide Call** affects the **entire open-water two-thirds**: DC 13 Strength
  save or knocked prone **and pushed 10 ft toward the sea-arch.** Mark the
  affected area clearly on a grid so the scope is unambiguous in the moment.
  Note it does *not* add difficult terrain — the open water already is.
- **At party size 5–6,** Locke also has a lair action on initiative 20
  dragging one creature in the open water 10 ft toward the arch (DC 13 Str).
  Between that and Tide Call, standing in the water is a real positional
  decision, which is the point of drawing the shelf.
- Locke hovers and is unaffected by his own surges.

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
