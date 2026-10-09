# Highwater — Map Specifications

Non-canon, standalone — see [`../README.md`](../README.md) and
[`HIGHWATER.md`](HIGHWATER.md) for the adventure this map supports.

This file is written so that **an image model, a drawing script, or a person
with graph paper can rebuild the dam from text alone.** Everything is given as
exact rectangles in feet and squares, with every door, stair, hazard, and
water state listed. Nothing here depends on the adventure text to be drawn
correctly.

It contains: (0) drawing conventions, (1) the side-on cross-section, (2–4)
three plan maps — Crest, Gallery, Sluice — as tables and machine-readable
YAML, (5) a master connection list, (6) the water-state overlays for each
Gauge Mark, (7) battle-map notes for the tactical rooms, (8) copy-paste image
prompts, and (9) a validation checklist.

---

## 0. Conventions (read first)

| Item | Value |
|---|---|
| Scale | **1 square = 5 ft.** A 300-ft-wide level is **60 squares** wide. |
| Canvas per level | **300 ft × 130 ft = 60 × 26 squares.** Same canvas for all three levels so they stack. |
| Origin | **Top-left (NW) corner = (x 0, y 0).** `x` increases **east (right)**; `y` increases **south (down)**. |
| Orientation | **North (top of the page) = upstream = the reservoir ("the Mere").** **South (bottom) = downstream = the valley and Lowmill.** The long axis of the dam runs **west–east**. |
| Coordinates | All `x,y` in feet from the origin. A rectangle `x a–b, y c–d` covers feet a→b east and c→d south. |
| Walls | Thick solid black. Dam masonry is **solid fill** (hatched grey) between rooms; rooms are the white or tinted voids. |
| Doors | Gap in a wall, short bar across it; **iron door** = filled bar; **arch** = open gap; **secret/barred** = dashed. |
| Stairs | Chevron lines, arrow pointing **down**. Spiral stairs = concentric arc with arrow. |
| Water | Blue wash; depth shown by shade (light = ankle/knee, mid = waist/chest, dark = swim/submerged). |
| Elevation | Crest = **0 ft**. Gallery = **−40 ft**. Sluice Level = **−90 ft**. |

**Naming:** Room IDs match the adventure: **C**rest (C1–C3), **G**allery
(G1–G11), **S**luice (S1–S10).

**Dimensions of the dam as a whole:** 300 ft along its length including both
abutments (west abutment x 0–40; dam body x 40–260; east abutment x 260–300).
Crest to base ≈ 90 ft. Thickness (north–south) = 40 ft at the crest, 65 ft at
the Gallery, 90 ft at the Sluice Level (the downstream face steps outward like
a gravity dam).

---

## 1. Cross-Section (side view, looking west)

A single elevation drawing to show how the levels stack. Optional but
strongly recommended for the table.

- Horizontal axis = **y** (north–south), 0 → 120 ft; vertical axis = elevation.
- **Upstream face** is **vertical** at y = 0, from the crest (0 ft) to the
  floor of the Mere at −90 ft. Mere water (blue) lies to the **left** of this
  face, with its surface a hand's breadth **below the crest lip** (≈ −1 ft).
- **Downstream face** steps out in three stages: crest slab ends at y = 40;
  at −40 ft the face is at y = 65; at −90 ft it is at y = 90. Draw it as a
  **stepped slope** (like a staircase of large blocks) falling to the valley
  floor at the right.
- **Crest slab** (top): 40 ft deep, ≈ 15 ft thick, with a small parapet bump at
  each edge.
- **Gallery Level** (−40 ft): a horizontal corridor band with the **Central
  Shaft** rising to the crest from it.
- **Sluice Level** (−90 ft): a wide chamber band along the base; **three
  gate slots** (iron slabs) rise from it toward the Mere; **tailrace tunnel**
  exits to the valley at the bottom right.
- **Central Shaft**, two parts: a narrow **hatch-well** (10 ft wide, centered
  at y 30) rising 40 ft from the Gallery ring's ceiling through the crest slab
  to the Crest hatch; and the **great well** (y ≈ 10–50, 26 ft void) from the
  Gallery ring 50 ft down to the sump pit at the Sluice Level. (The great well
  is wider than the crest slab is deep, which is why it stops at the
  Gallery.)
- **East Face Ledge** is a thin stone ledge on the downstream face 30 ft
  below the crest (elev −30), x 215–265.
- Add three **Mark lines** on the Mere side showing the failure level:
  **Danger Line** (just under the crest lip), **Crest Lip** (0 ft), and
  **Overtopping** (+1 ft above the Spill Notch floor).
- Label: "Mere (reservoir)", "Crest", "Gallery", "Sluice Level", "Valley",
  "Lowmill (off-map, 2 mi)".

---

## 2. LEVEL 1 — CREST (Elevation 0 ft)

### 2.1 Rooms and features

| ID | Name | Rect (ft) | Size (sq) | Notes |
|---|---|---|---|---|
| — | Dam top slab | x 40–260, y 0–40 | 44 × 8 | Whole crest. North edge = upstream (Mere), south edge = downstream drop. |
| C1 | **Crest Walk** | x 40–260, y 3–37 | 44 × 7 | Paved. **Parapets** (3 ft high) along y 0–3 (north) and y 37–40 (south), full length. Slick. |
| — | **Spill Notch** | x 170–190, y 0–40 | 4 × 8 | Crest dips 4 ft here. An **iron-grate footbridge** crosses it at y 10–30. **Stoplog slots** (vertical grooves) in both cheeks of the notch at y 2–4. Water overtops here at Marks 5–6. |
| — | **Central Shaft hatch** | circle, center (130, 30), r 5 → x 125–135, y 25–35 | 2 × 2 | Round iron hatch over the **hatch-well**: a 10-ft chimney with an iron ladder, 40 ft down to the Gallery ring. |
| C3 | **Keeper's House** | x 4–38, y 2–38 | 7 × 7 | West abutment. Stone building. |
| C3a | Kitchen-hall | x 4–38, y 2–24 | 7 × 4 | Cold hearth on west wall (x 4–10, y 8–14). **Cellar hatch** (5 × 5 ft) at x 10–15, y 14–19. |
| C3b | Chamber / office | x 4–38, y 24–38 | 7 × 3 | Desk against south wall; **Keeper's Log** on desk (x 14–20, y 34–38). Wall cabinet (x 28–36, y 34–38). |
| C3c | **Keeper's Cellar** *(below, elev −10)* | x 8–30, y 6–20 | 4 × 3 | Dashed outline. Stone, damp, a cot. Hatch above. Stair leaves from east wall at (30, 13). |
| C2 | **Winch House** | x 265–295, y 5–35 | 6 × 6 | East abutment. Three iron **winch drums** along north wall (x 270–290, y 6–10), each wound with chain running out through a wall-slot toward the Spill Notch's stoplogs. **Roof ladder** at NE corner (x 290–294, y 6–10). Crowbar and 100 ft of rope on the south wall. |
| C2a | **Signal beacon** *(on roof)* | x 280–292, y 8–16 (roof plan) | — | Lamp-cage + reflector + oil barrel + bell-cord. Draw as a small inset or note. |
| — | **East Stair turret** | x 262–270, y 36–44 | 2 × 2 | Tight spiral stair, **down** to G7 (it runs the full 40 ft inside the turret). Bulges slightly from the downstream face. Exterior iron door on its south side at elevation −30 (266, 44) onto the East Face Ledge. |
| — | **East Face Ledge** *(downstream, elev −30)* | x 215–265, y 40–45 | 10 × 1 | 5-ft stone ledge on the face, 30 ft below the crest. Reaches the turret door. Dashed. |
| — | Access road | x 0–4, y 15–25 | — | Arrives from the west at the Keeper's House front door. |

### 2.2 Doors and openings (Crest)

| From → To | Location (ft) | Type | State |
|---|---|---|---|
| Road → C3a (front door) | (4, 15–19), west wall | wooden | closed, unlocked |
| C3a → C1 (Crest door) | (38, 18–22), east wall | wooden | closed, unlocked |
| C3b → yard (back door) | (20, 38), south wall of the chamber | wooden | **barred outside** |
| C3a → C3c (cellar hatch) | (10–15, 14–19) | trapdoor | **barred** with an iron bar |
| C3a ↔ C3b | (22–26, 24) | arch | open |
| C1 → C2 (Winch House door) | (265, 18–22), west wall | wooden | stuck |
| C2 → East Stair | (268, 33–35), SW corner | arch/stair | open |
| C2 → roof | (290–294, 6–10) | ladder | open |
| C1 → Central Shaft | (125–135, 25–35) | iron hatch | closed (latched) |

### 2.3 Machine-readable (YAML)

```yaml
level: crest
elevation_ft: 0
canvas_ft: {w: 300, h: 130}
rects:
  dam_top:        {x: [40,260], y: [0,40]}
  crest_walk:     {x: [40,260], y: [3,37]}
  north_parapet:  {x: [40,260], y: [0,3]}
  south_parapet:  {x: [40,260], y: [37,40]}
  spill_notch:    {x: [170,190], y: [0,40], note: "crest dips 4 ft; iron-grate footbridge y 10-30"}
  keepers_house:  {x: [4,38], y: [2,38]}
  kitchen_hall:   {x: [4,38], y: [2,24]}
  chamber:        {x: [4,38], y: [24,38]}
  winch_house:    {x: [265,295], y: [5,35]}
  east_stair:     {x: [262,270], y: [36,44], kind: spiral, down_to: G7}
circles:
  central_shaft_hatch: {center: [130,30], r: 5}
below:
  keepers_cellar: {x: [8,30], y: [6,20], elevation_ft: -10, dashed: true}
external:
  east_face_ledge: {x: [215,265], y: [40,45], elevation_ft: -30, dashed: true}
doors:
  - {from: road, to: kitchen_hall, at: [4,17], axis: x}
  - {from: kitchen_hall, to: crest_walk, at: [38,20], axis: x}
  - {from: chamber, to: yard, at: [20,38], axis: y, state: barred}
  - {from: kitchen_hall, to: cellar, at: [12.5,16.5], kind: trapdoor, state: barred}
  - {from: crest_walk, to: winch_house, at: [265,20], axis: x, state: stuck}
  - {from: winch_house, to: east_stair, at: [268,34]}
features:
  - {name: cold_hearth, at: [4,8,10,14]}
  - {name: keepers_log_desk, at: [14,34,20,38]}
  - {name: winch_drums, at: [270,6,290,10]}
  - {name: roof_ladder, at: [290,6,294,10]}
```

---

## 3. LEVEL 2 — THE GALLERY (Elevation −40 ft)

A damp inspection level. **A single straight corridor** runs west to east, with
rooms off both sides and **four ways to bypass it**. At Mark 2 a stretch of the
corridor collapses and the level splits into two halves.

### 3.1 Rooms and features

| ID | Name | Rect (ft) | Size (sq) | Notes |
|---|---|---|---|---|
| — | Gallery body (mass) | x 40–260, y 0–65 | — | Solid masonry containing all voids below. West/east abutments extend x 0–40 and 260–300, y 0–50. |
| G1 | **West Stair Landing** | x 38–52, y 22–40 | 3 × 4 | Receives the cellar stair from the Keeper's House. Shelf with lamps on west wall. |
| G11 | **Inspection Corridor** | x 52–238, y 25–35 | 37 × 2 | 10 ft wide, 8 ft ceiling. Straight except where it meets the Shaft ring. |
| G8 | **Central Shaft** (ring) | center (130, 30); void r 13; ledge r 13–18 (5 ft); wall r 18–20 | 7 × 7 incl. wall | The **great well** drops 50 ft from here to the Sluice sump; a **spiral iron stair** hugs its wall. The **hatch-well** (r 5, iron ladder) opens in the ceiling over the center, reached by a short iron **catwalk** from the north side of the ledge. The corridor meets the ring at its **west point (110, 30)** and **east point (150, 30)**. Walking around the ring = half-circle of 5-ft ledge, ≈ 55 ft. |
| G2 | **The Cistern** | x 55–95, y 5–23 | 8 × 4 | Black water filling most of the room (x 58–92, y 8–20). **Stone walkway** 5 ft wide around the edge. Floor **drain grate** at (60, 18). |
| G3 | **Pump Room** | x 55–95, y 37–55 | 8 × 4 | Three **bucket-chain pumps** (x 72–90, y 40–50) driven by a small **water-wheel** on the east wall (x 88–94, y 38–44); overhead pipes. **Deep sump** (x 60–72, y 42–52). Tool rack with shovels and a pry-bar (x 56–60, y 38–44). |
| G9 | **Seepage Crawl** | from (95, 10) → (100, 7) → east along y 6–9 to x 150 → (150, 8) | 11 × 0.6 | 3-ft-wide, 3-ft-high maintenance crawl. Medium creatures squeeze. Connects G2 to G5 NW corner. |
| G5 | **Control Gallery** | x 150–180, y 5–23 | 6 × 4 | **Three levers** on the north wall (x 156, 162, 168 at y 6–8). **Flood Chart** painted on the north wall east of the levers (x 171–179, y 5–6). Splintered **Master Gear** on the floor (x 160–170, y 12–18). **Drive-shaft stub** (where the gear mounts) projecting from the arch to G4 at (174–180, 12–17). **Bell** on the south wall (152, 22), rung from the Valve Hall. |
| G4 | **Gear Hall** | x 180–220, y 5–23 | 8 × 4 | **Gate Train**: three large gears on a long axis along y 12–16 (x 185–215). **Chain-hoist trolley** on an overhead rail (y 8, x 185–215). **Catwalk** along the north wall (y 6–9, raised 8 ft). **Spoil Chute hatch** at (x 212–217, y 7–12). Lamp-oil crate cluster at (x 195–205, y 17–22). |
| G6 | **Forge Gallery** | x 190–235, y 37–55 | 9 × 4 | Cold **furnace** (x 195–205, y 38–44), **anvil** (x 212–216, y 42–46), **tipped slag crucible** (x 225–233, y 48–54), **steel Parts Cage** along the south wall (x 205–230, y 51–55). |
| G7 | **Culvert Junction** | x 235–262, y 18–50 | 5 × 6 | **Culvert channel** x 245–255, y 18–50 (10 ft wide, 4 ft deep, running **north to south**). **Plank bridge** across at y 28–32. **Ladder shaft** (iron ladder down 40 ft to the Gate 3 shelf) in NE corner at (256–260, 18–22). **Door to the East Stair** in the east wall at (262, 38–42), opening into the turret (x 262–270, y 36–44). |
| G10 | **Service Corridor** | from Pump east wall (95, 50–54) → east to (97, 52) → south to y 60 → east along y 58–62 to x 187 → north to (187, 50) → Forge west door (190, 48–52) | 5-ft wide | Dark, pipe-cluttered, 5 ft wide. Passes **under** the Shaft ring. |
| — | **Drain Pipe** | from Cistern grate (60, 18) to Pump sump (60, 42) | — | Flooded 3-ft iron pipe ≈ 24 ft long. Swim only. |

### 3.2 Doors and openings (Gallery)

| From → To | Location (ft) | Type | State |
|---|---|---|---|
| G1 ↔ G11 | (52, 28–32) | arch | open |
| G11 ↔ G2 | (72–78, 23–25) | wooden | open |
| G11 ↔ G3 | (72–78, 35–37) | wooden | open |
| G11 ↔ G8 (west) | (110, 28–32) | arch | open |
| G11 ↔ G8 (east) | (150, 28–32) | arch | open |
| G11 ↔ G5 | (162–168, 23–25) | iron | open |
| G11 ↔ G4 | (197–203, 23–25) | iron | open |
| G5 ↔ G4 | (180, 12–17) | arch (5 ft) | open; drive-shaft stub passes through |
| G11 ↔ G6 | (209–215, 35–37) | iron | open |
| G6 ↔ G10 | (190, 48–52) | wooden | open |
| G6 ↔ G7 | (235, 43–47) | wooden | open |
| G11 ↔ G7 | (235, 28–32) | arch | open (plank bridge beyond) |
| G3 ↔ G10 | (95, 50–54) | arch | open |
| G2 ↔ G9 | (95, 8–12) | low arch | open (crawl) |
| G9 ↔ G5 | (150, 7–9) | low arch | open (crawl) |
| G8 ↔ Crest | (130, 30) | hatch | above |
| G8 ↔ Sluice | (130, 30) | stair/sump | below |
| G4 → S1 | (212–217, 7–12) | hatch → chute | one-way slide |
| G7 → S4 | (256–260, 18–22) | ladder | down |
| G7 → East Stair turret | (262, 38–42) | wooden door → spiral stair | up to Winch House |
| G1 → C3c | (38, 31) | stair | up |

### 3.3 Collapse zone (Mark 2)

At Mark 2 the corridor **x 85–108, y 25–35** collapses (rubble, dust, a
fallen lintel). Show it as a hatched block labeled "collapse (Mark 2)".
West half = G1, G2, G3 and the corridor to x 85. East half = everything else.
The west and east halves stay connected via **G9 (crawl)**, **G10 (service
corridor)**, and the **Central Shaft**.

### 3.4 Machine-readable (YAML)

```yaml
level: gallery
elevation_ft: -40
canvas_ft: {w: 300, h: 130}
masonry: {x: [40,260], y: [0,65]}
rects:
  G1_west_stair_landing: {x: [38,52], y: [22,40]}
  G11_corridor:          {x: [52,238], y: [25,35]}
  G2_cistern:            {x: [55,95], y: [5,23]}
  G3_pump_room:          {x: [55,95], y: [37,55]}
  G5_control_gallery:    {x: [150,180], y: [5,23]}
  G4_gear_hall:          {x: [180,220], y: [5,23]}
  G6_forge:              {x: [190,235], y: [37,55]}
  G7_culvert_junction:   {x: [235,262], y: [18,50]}
circles:
  G8_shaft: {center: [130,30], void_r: 13, ledge_r: [13,18], wall_r: [18,20]}
corridors:
  G9_crawl: {width_ft: 3, path: [[95,10],[100,7],[150,7],[150,8]]}
  G10_service: {width_ft: 5, path: [[95,52],[97,52],[97,60],[187,60],[187,50],[190,50]]}
channels:
  culvert: {x: [245,255], y: [18,50], depth_ft: 4, flow: south}
pipes:
  drain_pipe: {from: [60,18], to: [60,42], flooded: true}
features:
  plank_bridge: {x: [245,255], y: [28,32]}
  levers: [[156,6],[162,6],[168,6]]
  master_gear_splinters: {x: [160,170], y: [12,18]}
  flood_chart: {x: [171,179], y: [5,6], wall: north}
  drive_shaft_stub: {x: [174,180], y: [12,17]}
  bell: {at: [152,22]}
  hatch_well: {center: [130,30], r: 5, rises_ft: 40, ladder: true, catwalk_from: [130,12]}
  gate_train_gears: {x: [185,215], y: [12,16]}
  chain_hoist_rail: {x: [185,215], y: [8,8]}
  catwalk: {x: [180,220], y: [6,9], elevation_ft: 8}
  spoil_chute_hatch: {x: [212,217], y: [7,12]}
  oil_crates: {x: [195,205], y: [17,22]}
  furnace: {x: [195,205], y: [38,44]}
  anvil: {x: [212,216], y: [42,46]}
  slag_crucible: {x: [225,233], y: [48,54]}
  parts_cage: {x: [205,230], y: [51,55]}
  ladder_down: {at: [258,20]}
  east_stair_door: {at: [262,40], to: "turret x 262-270, y 36-44, spiral up to Winch House"}
  pump_wheel: {x: [88,94], y: [38,44]}
  tool_rack_shovels: {x: [56,60], y: [38,44]}
collapse_mark2: {x: [85,108], y: [25,35]}
```

---

## 4. LEVEL 3 — THE SLUICE LEVEL (Elevation −90 ft)

The belly of the dam. **Three gate chambers** open off a central **Valve
Hall**; below them, a **tailrace** carries flow to the valley; east of them,
behind a sealed door, is a **smugglers' cache** and the intake of the **Old
Overflow Channel**.

### 4.1 Rooms and features

| ID | Name | Rect (ft) | Size (sq) | Notes |
|---|---|---|---|---|
| S1 | **Valve Hall** | x 100–200, y 15–55 | 20 × 8 | Vaulted. **Pressure Board** on north wall (x 150–190, y 15–17): three plate-size brass gauges labeled I, II, III. **Sump pit** (circular, center (130, 30), r 13 → x 117–143, y 17–43) is the foot of the Central Shaft, black water; **stair foot** at its south-east rim (140, 40). **Silt heap** where the Spoil Chute lands at (190–198, 18–24). **Bell-pull** to the Control Gallery beside the Pressure Board (192, 16). |
| S2 | **Gate 1 Chamber** ("Little") | x 55–100, y 15–55 | 9 × 8 | **Gate slab** in a slot at the north wall (x 70–85, y 15–18). **Hoist rack and hand-crank** on a platform 8 ft up at (90–96, 15–20). Discharge **grille** in the south wall (x 60–95, y 55). Door E to S1. |
| S9 | **Gate 1 Outfall** | x 55–100, y 55–90 | 9 × 7 | Clear stone channel with **its own open south mouth** (x 60–95, y 90) onto the dam toe. The **Tailrace West Branch** meets its east wall (x 100, y 75–85) through an **iron grate**, so Gate 1's water stays out of the Tailrace. |
| S3 | **Gate 2 Chamber** ("Great") | x 200–240, y 15–55 | 8 × 8 | **Gate slab** in a wide slot at the north wall (x 210–230, y 15–18): 20 ft wide. **Flush leaf** (small sluice) at the slab's foot (x 216–224, y 18–20), held by a visible iron **shear pin**. **Hand-crank** on a platform 8 ft up at (232–238, 15–20). South wall = heavy fixed iron **grille** (x 205–235, y 55) onto S8 — water passes, people don't. **Stair** up 10 ft to the Alcove along the east wall (x 232–240, y 30–40). Door W to S1 (200, 33–37); door E to S5 at the stair head (240, 33–37). |
| S8 | **Gate 2 Outfall** (the jam) | x 200–235, y 55–90 | 7 × 7 | **Mud slump** piled to the ceiling against the **east wall** and across the **south mouth**: the mud's edge runs diagonally from (235, 64) on the east wall to (200, 86) on the west wall; everything south-east of that line is mud. North-west of it is open channel with a low mud bank. Pale roots, a fence-post, a hayrick corner in the mud. **South mouth** (x 200–235, y 90) **plugged** by the mud. **Diversion Mouth** (8-ft arched opening, iron shutter) in the east wall (x 235, y 72–80), **buried** under the mud. Opening on the west wall at (x 200, y 75–85) = **Tailrace East Branch**, just clear of the mud. |
| S5 | **Alcove** | x 240–255, y 25–45 | 3 × 4 | Stone antechamber, floor **10 ft above** the Sluice floor (level with the Gate 3 shelf). Cold draft; sweating wall. **Old Overflow Door** in the south wall at (x 244–250, y 45): thick iron, barred from the other side. |
| S6 | **Overflow Passage** | x 244–250, y 45–55 | 1 × 2 | 5 ft wide, 10 ft long, a **ramp** dropping 10 ft to the Cache floor at its north wall (x 244–250, y 55). |
| S4 | **Gate 3 Chamber** ("Still") | x 255–290, y 15–55 | 7 × 8 | **Raised gallery shelf** (10 ft up, 10 ft wide) along the west wall (x 255–265) and north wall (y 15–25). **Ladder from G7** lands on the shelf's NW corner at (258, 18). **Gate slab** at north wall (x 268–280, y 15–18). **Hand-crank** on the north shelf at (282–288, 15–22). Discharge **floor grille** along the south wall (x 262–282, y 48–55) dropping into a **stone race** that runs under the Cache floor and exits at the dam toe (off-map, SE). Iron rungs up to the shelf in the SW corner (256, 52). Door W to S5 at (255, 33–37) — shelf level. |
| S7 | **Smugglers' Cache** | x 235–290, y 55–90 | 11 × 7 | Long vault, cold. **Bale clusters** (cover): (245–255, 60–68), (250–262, 80–88), (240–246, 70–78). **Barrel of lamp oil** at (265, 62). **Rope-and-plank gantry** (15 ft up) at the east end: x 270–288, y 66–84, **ladder** at (268, 75). **Great Wheel** (6 ft diameter) on the gantry at (282, 75). **Weir-Gate** (huge iron door) across the **Overflow Channel** mouth in the east wall (x 290, y 70–80), with a man-sized **wicket door** in its lower corner (x 290, y 78–80). **Diversion Mouth shutter** on the west wall (x 235, y 72–80). **Cable run** under the floor along y 76 from (238, 76) to (282, 75). Door N at (244–250, 55) from S6. |
| — | **Overflow Channel** | from (290, 70–80) east to the canvas edge (x 300), then SE (off-map) | — | A 10-ft-wide, 12-ft-high tunnel that runs about a quarter mile to the abandoned **Old Quarry** basin. Draw a few feet and an arrow labeled "to Old Quarry (¼ mi)". |
| S10 | **Tailrace Tunnel** | x 145–155, y 55–90, then daylight x 140–160, y 90–120 | 2 × 7 | The Valve Hall's drain and the inspection route to both outfalls. 10 ft wide, 8 ft ceiling, runs **south** from S1's south wall (x 145–155, y 55). **West Branch** x 100–145, y 75–85 → S9. **East Branch** x 155–200, y 75–85 → S8. Daylight mouth at the bottom (y 120), open to the beck. |

### 4.2 Doors and openings (Sluice)

| From → To | Location (ft) | Type | State |
|---|---|---|---|
| S1 ↔ S2 | (100, 30–36) | arch | open |
| S1 ↔ S3 | (200, 33–37) | iron | open |
| S1 ↔ S10 | (145–155, 55) | arch | open |
| S3 ↔ S5 | (240, 33–37) | iron, at the head of a 10-ft stair | open |
| S5 ↔ S4 | (255, 33–37) | iron (shelf level) | open |
| S5 ↔ S6 | (244–250, 45) | **Old Overflow Door** | **barred from inside** |
| S6 ↔ S7 | (244–250, 55) | arch at foot of ramp | open |
| S3 ↔ S8 | (205–235, 55) | fixed iron grille | impassable to people; water passes |
| S2 ↔ S9 | (60–95, 55) | iron grille | open (gate discharge) |
| S4 → race | (262–282, 48–55) | floor grille into stone race under S7 | discharge only; no passage |
| S8 ↔ S7 | (235, 72–80) | Diversion Mouth, shuttered | closed; buried by mud |
| S7 → Channel | (290, 70–80) | Weir-Gate | closed |
| S10 ↔ S9 | (100, 75–85) | iron grate | locked (the Keeper's Key fits; DC 13 thieves' tools); water passes slowly |
| S10 ↔ S8 | (200, 75–85) | arch | open |
| S1 ← G4 | (190–198, 18–24) | chute landing | one-way |
| S4 ← G7 | (258, 18) | ladder landing | one-way up/down by ladder |
| S1 ← G8 | (140, 40) | spiral stair foot | open |

### 4.3 Machine-readable (YAML)

```yaml
level: sluice
elevation_ft: -90
canvas_ft: {w: 300, h: 130}
masonry: {x: [40,290], y: [0,90]}
rects:
  S1_valve_hall:     {x: [100,200], y: [15,55]}
  S2_gate1_chamber:  {x: [55,100], y: [15,55]}
  S9_gate1_outfall:  {x: [55,100], y: [55,90]}
  S3_gate2_chamber:  {x: [200,240], y: [15,55]}
  S8_gate2_outfall:  {x: [200,235], y: [55,90]}
  S5_alcove:         {x: [240,255], y: [25,45], floor_ft: 10}
  S6_overflow_pass:  {x: [244,250], y: [45,55], ramp_down_ft: 10}
  S4_gate3_chamber:  {x: [255,290], y: [15,55]}
  S7_cache:          {x: [235,290], y: [55,90]}
  S10_tailrace:      {x: [145,155], y: [55,90]}
  tailrace_west:     {x: [100,145], y: [75,85]}
  tailrace_east:     {x: [155,200], y: [75,85]}
  tailrace_mouth:    {x: [140,160], y: [90,120]}
  S9_south_mouth:    {x: [60,95], y: [90,90], open: true}
  S8_south_mouth:    {x: [200,235], y: [90,90], plugged_by_mud: true}
circles:
  sump: {center: [130,30], r: 13}
features:
  pressure_board:    {x: [150,190], y: [15,17]}
  silt_heap:         {x: [190,198], y: [18,24]}
  gate1_slab:        {x: [70,85], y: [15,18]}
  gate1_crank:       {x: [90,96], y: [15,20], elevation_ft: 8}
  gate2_slab:        {x: [210,230], y: [15,18]}
  gate2_crank:       {x: [232,238], y: [15,20], elevation_ft: 8}
  gate2_flush_leaf:  {x: [216,224], y: [18,20], shear_pin: true}
  gate2_alcove_stair: {x: [232,240], y: [30,40], rises_ft: 10}
  bell_pull:         {at: [192,16]}
  gate3_slab:        {x: [268,280], y: [15,18]}
  gate3_crank:       {x: [282,288], y: [15,22], on_shelf: true}
  gate3_floor_grille: {x: [262,282], y: [48,55], to: "stone race under S7"}
  gate3_rungs:       {at: [256,52]}
  gate3_shelf:       [{x: [255,265], y: [15,55]}, {x: [255,290], y: [15,25]}]   # +10 ft
  gate3_ladder_landing: {at: [258,18]}
  mud_jam:           {polygon: [[235,64],[235,90],[200,90],[200,86]], note: "everything SE of the line (235,64)-(200,86) is mud to the ceiling"}
  diversion_mouth:   {x: [235,235], y: [72,80], buried_by_mud: true}
  old_overflow_door: {x: [244,250], y: [45,45], barred_inside: true}
  bale_clusters:     [{x: [245,255], y: [60,68]}, {x: [250,262], y: [80,88]}, {x: [240,246], y: [70,78]}]
  lamp_oil_barrel:   {at: [265,62]}
  gantry:            {x: [270,288], y: [66,84], elevation_ft: 15, ladder: [268,75]}
  great_wheel:       {center: [282,75], diameter_ft: 6}
  weir_gate:         {x: [290,290], y: [70,80], wicket: {y: [78,80]}}
  diversion_shutter: {x: [235,235], y: [72,80]}
  cable_run:         {path: [[238,76],[282,75]], under_floor: true}
  overflow_channel:  {from: [290,75], to: [300,75], then: "southeast, off-map, to Old Quarry (1/4 mile)"}
doors:
  - {S1-S2: [100,33]}
  - {S1-S3: [200,35]}
  - {S1-S10: [150,55]}
  - {S3-S5: [240,35]}
  - {S5-S4: [255,35], level: shelf}
  - {S5-S6: [247,45], kind: "Old Overflow Door", state: barred_inside}
  - {S6-S7: [247,55]}
  - {S10-S9: [100,80], kind: iron_grate, state: locked}
  - {S10-S8: [200,80]}
```

---

## 5. Master Connection List (all vertical and cross-level links)

| Link | From | To | Type | Notes |
|---|---|---|---|---|
| Keeper's stair | C3c cellar (30, 13) | G1 (38, 31) | stair, 50 ft run | Descends −10 → −40 ft. |
| Central Shaft | Crest hatch (130, 30) | G8 ring → S1 sump | spiral iron stair | −0 → −40 → −90. Fastest, most dangerous. |
| East Stair | Winch House (268, 34) | G7 east door (262, 40) | tight spiral stair in the turret | 0 → −40; exterior door at −30 onto the East Face Ledge. |
| Culvert Ladder | G7 (258, 20) | S4 shelf (258, 18) | iron ladder, 40 ft | −40 → −80 (the shelf is 10 ft above the −90 floor). The **dry route** to the Cache after Mark 4. |
| Spoil Chute | G4 (214, 9) | S1 (194, 21) | steep chute, one-way | −40 → −90 (50 ft drop); cannot be climbed back. |
| Alcove stair | S3 floor (236, 40) | S5 (240, 35) | stone stair, 10 ft | Keeps the Alcove dry through Mark 5. |
| Bell-pull | S1 (192, 16) | G5 (bell) | cord in a pipe | Signal only. |
| East Face Ledge | Crest (parapet edge, x 215–260) | East Stair door (266, 44) | external ledge, 30 ft below | Reached by falling/rope from the south parapet. |
| Drain Pipe | G2 grate (60, 18) | G3 sump (60, 42) | flooded pipe | Swim only. |
| Seepage Crawl | G2 (95, 10) | G5 (150, 8) | crawl | Bypasses the Shaft ring. |
| Service Corridor | G3 (95, 52) | G6 (190, 50) | corridor | Bypasses the Shaft ring; passes beneath it. |
| Tailrace | S1 (150, 55) | daylight (150, 120) | tunnel | Two branches; floods at Mark 3. |
| Overflow Channel | S7 (290, 75) | Old Quarry (off-map) | tunnel | Opened by the Great Wheel. |

---

## 6. Water-State Overlays (draw as optional transparent layers)

Each Mark adds water or closes a route. Draw each as its own overlay so a
table can "step" through the dam failing.

| Mark | Time left | Overlay (what to shade/hatch) |
|---|---|---|
| **1** | 2:30 | Light water (knee): **S9**, **tailrace west branch**. Cistern **G2** full to the lip. |
| **2** | 2:00 | **Collapse** hatch at G11 x 85–108. Light water (ankle): S1 floor, S2, S3. |
| **3** | 1:30 | **Tailrace S10, S8, S9 fully flooded** (dark). **S1 knee-deep** (light). Shaft sump rises to the bottom of the stair. |
| **4** | 1:00 | **S1 chest-deep** (mid). S2, S3 waist-deep. **S7 Cache floor ankle-deep** (knee-deep if Gate 3 has run; dry once the Weir-Gate is open — it drains down the channel). **G2, G3 ankle-deep.** Gate 3 Chamber floor flooded; **shelf and Alcove dry**. Lower 30 ft of the Shaft = whirlpool. |
| **5** | 0:30 | **Entire Sluice Level flooded** (dark) except the **Gate 3 shelf**, the **Cache gantry**, and the **Alcove**; the Cache floor is waist-deep (dry if the Weir-Gate is open). Gallery floors ankle-deep. **Water over the Spill Notch** (C1); Crest Walk ankle-deep with a current toward the south parapet. |
| **6** | 0:00 | Failure: draw a **crack** across the crest at the Spill Notch and a dark arrow of water down the valley toward Lowmill. |

---

## 7. Battle-Map Notes (the tactical rooms)

Grid = **5 ft/square**, standard VTT.

### E1 — The Crest Walk (44 × 7 usable squares)
- A long, narrow arena: the walkway is **y 3–37 → squares 0–7** wide; the
  parapets are 3 ft high (half cover). Four crayfish start between the
  Keeper's House and the Shaft hatch; the **Old Snapper** (Large, 2 × 2
  squares) starts in the Spill Notch and joins on round 2.
- **Slick terrain** everywhere (DC 12 Acrobatics if Dashing). Mark the
  Spill Notch (4 squares wide, dipped) as difficult terrain with a
  grate footbridge.
- A creature dragged off the **north** parapet falls into the Mere (soft).
  Off the **south** parapet: DC 13 Dex to catch the edge, otherwise the
  30-ft drop to the East Face Ledge (3d6) if between x 215–260; otherwise
  the 90-ft fall — **do not place the starting fight within 10 ft of the
  south parapet outside the ledge zone.**

### E2 — The Gear Hall (8 × 4 squares)
- **Catwalk** along the north wall at +8 ft (1.5 squares wide); bow position.
- **Chain-hoist trolley** on an overhead rail (north to south push = a 15-ft
  arc swing).
- **Oil-crate cluster** against the south wall, middle (x 195–205; flammable).
- Greaves starts at the center by the gears; the thugs flank the corridor
  door.

### E3 — The Forge Gallery (9 × 4 squares)
- Furnace and anvil are solid cover (full). Tipped crucible in the SE
  corner (spill area 2×2 squares of fire on a trigger).
- **Parts Cage** along the south wall: borers start gnawing at its bars.
- Mark the **three spare gears** inside the cage (18, 24, 30 teeth).

### E4 — The Central Shaft (7 × 7 squares including wall)
- Draw the great well as concentric circles: **void (r 13 ≈ 5 squares)**,
  ledge (1 square), wall (1 square). The **spiral stair** is a 3-ft strip
  clinging to the wall below the ledge; the **hatch-well** is a 2-square
  circle over the center, joined to the north ledge by a 1-square catwalk.
- Place the **water weird** in the sump on the lowest level (Sluice), or in
  the water that has climbed to the lowest stair when the party arrives.

### E5 — The Tailrace and Gate 2 Outfall (squares: tunnel 2 wide; outfall 7 × 7)
- The **Tailrace** is a 2-square-wide corridor; it floods after Mark 3.
- The **Outfall** is 7 × 7 squares. Mud fills everything south-east of a
  diagonal from the east wall at y 64 to the west wall at y 86; the
  2 squares nearest that line are a sloping **mud bank** (difficult
  terrain), the rest is solid mud. The **Tailrace East Branch** enters on
  the west wall just north of the mud. The **Diversion Mouth** (2 squares
  wide) is buried in the east wall at y 72–80. Through the north grille,
  the Gate 2 Chamber is visible.

### E6 — The Smugglers' Cache (11 × 7 squares)
- **Gantry** along the east end at +15 ft, reached only by the ladder at the
  west edge; the **Great Wheel** is on it.
- **Bale clusters** = half cover; barrels = full cover (if tipped).
- **Lamp-oil barrel** = 3d6 fire burst in 10 ft radius on a trigger.
- The Cache entrance (Overflow Passage) is a **1-square chokepoint** on the
  north wall. Do not widen it.

### E7 — The Crest Run and Silt Elemental (also used for the stoplogs)
- Reuse the Crest Walk map with the Spill Notch at the center-east.
  The elemental climbs over the **north parapet** near x 120–150.
- The **Winch House** (6 × 6 squares) at the east end is a refuge; its door is
  a 1-square chokepoint.

---

## 8. Image-Generation Prompts (copy-paste)

Image models struggle with exact geometry. For best results, **paste the
YAML and the room table for one level at a time** together with the matching
prompt below. If a generator cannot hold the coordinates, ask it to produce
an **SVG** from the YAML instead (the YAML is deliberately complete enough for
that).

### 8.0 Shared style block (prepend to every prompt)

> **Style/medium:** Hand-drawn fantasy dungeon map on aged, slightly
> rain-stained parchment; ink linework with a light blue-green watercolor
> wash for water features. Top-down schematic plan, battle-map/VTT friendly,
> with a faint 5-ft square grid overlay. **Scale:** 1 square = 5 ft. A small
> compass rose and a scale bar. Hand-lettered labels in a clean serif.
> **Orientation:** North (upstream, the reservoir) at the top; the dam runs
> west-to-east. **Do not invent rooms**; draw exactly the rooms, doors and
> features listed.

### 8.1 Level 1 — Crest (DM version)

> *Prepend the shared style block.* **Title banner:** "Highwater — Crest."
> Draw a long stone **dam-top road** running west-to-east (x 40–260 ft, 40 ft
> deep), with a thin low **parapet** along the north and south edges. North of
> it, dark choppy **reservoir water**; south of it, a cliff-edge drop shown
> with stepped hatching. In the **center-east**, a **notch** 20 ft wide where
> the crest dips, with an **iron-grate footbridge** and water lapping the lip.
> At the **center**, a **round iron hatch** (10 ft). At the **west end**, a
> two-room **stone Keeper's House** (kitchen-hall with cold hearth; office
> with a desk) with the dashed outline of a **cellar** beneath. At the **east
> end**, a square **stone Winch House** with three round winch drums on its
> north wall and a ladder to a **roof beacon**. A small **spiral-stair
> turret** at the southeast corner. A thin dashed **ledge** on the south face
> from x 215–265. Label only: "Crest Walk", "Spill Notch", "Keeper's House",
> "Winch House", "Central Shaft hatch", "East Stair". Rain-streak texture.

### 8.2 Level 2 — Gallery (DM version)

> *Prepend the shared style block.* **Title banner:** "Highwater — The
> Gallery (−40 ft)." Draw a single **straight 10-ft corridor** running
> west-to-east through solid masonry. At its center, a **circular well** (26
> ft void, 5-ft ledge ring, spiral stair clinging inside, a small ladder-well
> over its center reached by a catwalk) that the corridor
> joins at its west and east points. **Rooms north of the corridor:** the
> **Cistern** (x 55–95; half-filled with black water, a walkway around it);
> the **Control Gallery** (x 150–180; three levers on the north wall, a
> painted wall chart on the north wall beside them, a heap of broken iron in the middle);
> the **Gear Hall** (x 180–220; three big gears along its long axis, a
> catwalk on the north wall, a hatch in the NE corner). **Rooms south of the
> corridor:** the **Pump Room** (x 55–95; bucket-chain pumps on a small water-wheel, and a deep sump); the
> **Forge Gallery** (x 190–235; furnace, anvil, tipped crucible, a steel
> parts cage). At the **east end**, the **Culvert Junction**: a 10-ft channel
> running north-to-south with a plank bridge, an iron ladder in the NE corner
> (down), and a door in its east wall to a spiral-stair turret (up). At the **west end**, a
> small **landing** with a stair going up. **Bypass routes:** a very thin
> 3-ft **crawlway** running along the north wall from the Cistern to the
> Control Gallery; a 5-ft **service passage** running along the south wall
> from the Pump Room to the Forge, passing beneath the well; a short
> **drain pipe** (dashed) between the Cistern and Pump Room. A hatched block
> on the corridor at x 85–108 labeled "collapse (Mark 2)". Label every
> room by name.

### 8.3 Level 3 — Sluice Level (DM version)

> *Prepend the shared style block.* **Title banner:** "Highwater — Sluice
> Level (−90 ft)." Draw a vaulted central **Valve Hall** (x 100–200, y
> 15–55) with a bank of three brass gauges on its north wall and, at its west
> end, a **round black pit** (the foot of the Central Shaft). To the west, a
> **Gate 1 Chamber** with an iron slab-gate in a slot on its north wall; to
> the east, a **Gate 2 Chamber** with a much wider slab and a barred grille on
> its south wall and a short stair climbing its east wall. South of Gate 1:
> a clear **Outfall**. South of Gate 2: an **Outfall with a brown mud slump**
> piled diagonally against its east wall and across its south mouth, leaving
> a wedge of open channel in its north-west, and a buried arch in its east
> wall. Up the stair east of the Gate 2 chamber: a small raised **Alcove**,
> its south wall holding a **thick iron door**
> (the Old Overflow Door). East of the Alcove: a **Gate 3 Chamber** with a
> raised stone shelf around two walls and a ladder shaft descending into its
> corner. South of the Alcove: a **short 5-ft passage** leading to a **long
> vault** (the Cache) stacked with bales and barrels, with a raised
> rope-and-plank **gantry** at the east end holding a **huge spoked wheel**,
> and a massive **iron door** in the east wall labeled "to Old Quarry (¼
> mi)". A tunnel runs **south** from the Valve Hall to a daylight mouth at the
> bottom of the page, with a **west branch** ending at an iron grate into the Gate 1 Outfall (which has its own open mouth to the south) and an
> **east branch** to the Gate 2 Outfall. Label every room by name; label the
> Old Overflow Door, the Great Wheel, the Weir-Gate and the Mud Slump.

### 8.4 Cross-section (DM or player)

> *Prepend the shared style block, but draw a side-on elevation, not a
> plan.* **Title banner:** "Highwater — Section." A **stepped masonry dam**
> viewed from the west: the **reservoir** on the left (dark water just under
> the crest), a **vertical upstream face**, a **stepped downstream face**
> falling to a valley on the right. Inside, three stacked bands: a thin
> **crest slab**, a **corridor band at −40 ft** with a **wide vertical well**
> dropping from it to the base and a **narrow ladder chimney** rising from it
> to the crest, and a **wide chamber band at −90 ft** with three
> vertical **gate slots** and a **tunnel** exiting to the valley. A thin
> **ledge** on the downstream face 30 ft below the crest. Label "Mere,"
> "Crest," "Gallery," "Sluice Level," "Valley," and "Lowmill (2 mi)".

### 8.5 Player-safe handout (no secrets)

Give the table a handout that shows only what Fenn and the Keeper's
drawings would have: **the Crest, the Gallery corridor and the main rooms, the Valve
Hall, and the three Gates.** Omit the Old Overflow Door, the Alcove's south
wall, the Overflow Passage, the Cache, the Overflow Channel and the Old
Quarry. Replace the area they occupy with plain hatched masonry.

> *Prepend the shared style block.* **Title banner:** "Brindle Dam — Odo
> Fenn's Sketch." Draw a **rough, hand-sketched** version of the Crest,
> Gallery and Sluice Level with only: Crest Walk, Keeper's House, Winch
> House, Central Shaft, the Gallery corridor and rooms, the Valve Hall, and
> Gates I, II, III. Scrawled notes in the margin: "Spillways here!",
> "Three hours", and a question mark by the east end of the Sluice Level.
> No Cache, no overflow channel, no quarry.

### 8.6 Single-room battle maps (optional)

For each of E1–E7 in §7, prompt: *"Top-down 5-ft grid battle map of [room],
[size in squares], featuring [list from §7]. Hand-drawn fantasy style, no
text except small labels, tokens-friendly (clear cover and terrain markers)."*

---

## 9. Validation Checklist (for any generated map)

Check each generated image against these before using it:

- [ ] **North is up** and the reservoir is on the north (top).
- [ ] The dam is **300 ft wide**; the Crest Walk runs **x 40–260**.
- [ ] There is exactly **one Spill Notch**, center-east (x 170–190).
- [ ] The **Central Shaft** is centered near x 130 on every level: a small
      hatch on the Crest, a ringed well (with a ladder-well over its center)
      in the Gallery, a round sump pit in the Valve Hall.
- [ ] The Gallery has **one straight corridor** and **exactly three bypasses**
      (crawl, service corridor, drain pipe) plus the shaft.
- [ ] **Three gate chambers** on the Sluice Level (west, center-east, east)
      with **Gate 2's slab the widest** (20 ft).
- [ ] The **Alcove** has a door in its **south** wall and a **short passage**
      to the Cache.
- [ ] The **Cache** is a long vault with a **gantry and a wheel at the east
      end**, an **iron door** (Weir-Gate) in the east wall, and a **small
      arch** (Diversion Mouth) in the west wall.
- [ ] The **Gate 2 Outfall** has **mud piled diagonally against its east
      wall and south mouth**, with open channel in its north-west where the
      Tailrace branch enters.
- [ ] The **Alcove** is reached by a **stair** from the Gate 2 Chamber and is
      level with the **Gate 3 shelf**.
- [ ] The **Tailrace** runs south from the Valve Hall with **two side
      branches**.
- [ ] **Player-safe** handouts show **no Cache, no Overflow Channel, no
      Quarry**.

If the generator cannot hold these constraints, **ask for an SVG** built from
the YAML in §§2.3, 3.4, 4.3, or build the map manually from the §§2–4 tables.
