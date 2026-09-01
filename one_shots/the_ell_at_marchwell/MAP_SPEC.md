# MAP SPEC — The Ell at Marchwell

*Companion to [`THE_ELL_AT_MARCHWELL.md`](THE_ELL_AT_MARCHWELL.md).*

---

# PART 1 — THE ELL AS A WHOLE

## The rooms are real. Only the connections move.

**Do not draw a floorplan.** But do not tell the players the Ell is
unmappable, because it isn't — and a party that works this out has earned
something real.

**Every room is a fixed, permanent, unchanging place.** The room with the
anchor in it is always the room with the anchor in it. It has the same
dimensions, the same furniture, the same four doors, forever. Nothing about a
room ever changes.

**What moves is which door leads where** — and even that isn't random. A
doorway belongs to a *set* of identical doorways, and 2-sets are perfectly
deterministic. **The Ell is not a maze. It is a fixed catalogue of rooms
connected by unreliable doors, and the unreliability follows a rule.**

### So the correct map is a catalogue, not a floorplan

This is exactly what Hesper has, and exactly how she navigates. Her map is not
a plan of the Ell — there is no such thing. It's **a numbered list of rooms,
each with its distinguishing features, and notes on which doorways are twinned
with which.**

With that, you navigate by *routing*: *"We want the gallows room. From here,
the north door is twinned with the door in the well room. From the well room,
the east door is a 2-set with the anchor room. From the anchor room it's two
real doors to the gallows."* Slow, laborious, entirely reliable.

**And that's the arc of the campaign.** They arrive lost. They learn the rule.
They start cataloguing rooms and marking frames. By session 4 they can move
through the Ell on purpose — which is precisely the transition from prey to
people who understand the machine.

### How to run it at the table

**Keep a room register.** Number each room as the party first enters it and
note three things: what's in it, its distinguishing feature (or *none*, which
matters), and which set each doorway belongs to.

| # | Room | Distinguishing feature | Doors |
|---|---|---|---|
| 7 | Parlour, blue chairs | Water stain, ceiling | N: set A · E: set C · S: unique |
| 12 | Bedroom, ship's anchor | **Anchor (unique) — rest-safe** | W: set A · E: set F |

**When the party maps, let their map be right.** If they've recorded that room
7's north door is twinned with room 12's west door, then it is, every time,
and they can use it. Reward the bookkeeping — it's the hardest-won thing in the
adventure.

**Cutting a mark edits the catalogue.** Deface a frame and it leaves its set;
copy a mark and it joins one. The party is not just reading the map, they are
**writing to it**, which is the best thing a player can discover here.

**What they can't do** is derive a floorplan — distances and directions between
rooms are meaningless, because two rooms joined by a twinned door aren't near
each other in any sense. Anyone trying to draw the Ell to scale is doing the
one genuinely impossible thing, and should be gently told so by Hesper: *"You
can't draw it. You can only list it."*

### Depth is the other coordinate

Depth is real and stable. The party is always at a depth, and going deeper is
always available and never blocked.

> **The only navigation ruling you need:** going *deeper* always works. Going
> *back* works only to rooms they have made unique. Everything else is a fold.

## Structural spec

| Depth | Extent | Fixed nodes (must pass) | Optional nodes | Exits |
|---|---|---|---|---|
| **0** | Marchwell House, 4 down / 3 up | The pantry | Loft, press-house | Every exterior door → D1. Windows → the still orchard (loops back to the house) |
| **1** | 5 copies of the house, degrading | Copies 1→5 in order | — | Copy 5's kitchen (**Four Casses**) → D2 |
| **2** | Open sprawl, ~20–30 rooms | Coat Closet · Ambry's squat · **the oblex chamber** · the "way home" kitchen (*Change #9: a fresh reconstruction built at depth 2, not a literal return to a depth-1 copy — it destabilizes and pushes the party onward rather than looping them back*) | Wrong-object rooms (d20 table), corridors | Down, anywhere, after the way-home betrayal |
| **3** | A fixed 12-room bank (see the adventure's Depth 3 traversal table); parties visit 6–10 | Room 5, the drafted orchard (every branch converges here) | The other 11 rooms, entered via 3 starting doors and their branches | Room 5 → Depth 4 |
| **4** | All 6 rule-rooms fully detailed; run 3–5 per party size | 3–5 rule-rooms (DM's pick) | Real Cass's kitchen · Hesper's camps · the Cutter's Rest is Depth 3, not here | Down |
| **5** | The substrate. One vast continuous space | The plan-floor · the deep-time layers · the survey count · the reconstruction station | Scattered inert equipment · the Veyr shrine · the dead surveyor and his warning-verse | **The way out** (Hesper leads them) |

**Room budget per session:** S1 ~12 rooms · S2 ~20 · S3 ~15 · S4 ~6 large ones.

## The three fixed points

Everything else can move. These cannot:

1. **The pantry door** — the way in, and the tally is on its frame (and on
   every other exterior frame, identically).
2. **The "way home" kitchen** (a fresh depth-2 reconstruction, not a
   literal copy 2 — Change #9) — the S2 betrayal.
3. **The way out** at depth 5 — the finale room.

## Rest-safe rooms

A room is rest-safe if it's **unique**: party-marked, contains a one-of-a-kind
object (anchor, gallows, well, milestone), or is somebody's old camp. Keep a
running list as they make them — those are the only rooms they can reliably
return to, and by session 3 that list is effectively their map.

---

# PART 2 — BATTLE MAPS

Five needed. Everything else is theatre-of-mind.

**Universal:** from depth 2 down, light is **tallow-coloured, sourceless, and
shadowless** — treat as bright light everywhere, no darkvision advantage, no
hiding in shadow, and torches do nothing. Ceilings 9 ft unless noted.

---

## 1. THE FIFTH KITCHEN — *The Four Casses* (S1)

**Grid: 30 × 30 ft (6 × 6 squares).** A farmhouse kitchen with generic
furniture — *a* table, not *that* table.

- **Four doors**, one per wall. **All four are identical** — same frame, same
  latch, same paint. That's a 4-set: the Casses step through one and emerge
  from another at random, every round, and the party can see it happening.
- **Centre:** a long table, 10 × 4 ft. Difficult terrain to cross, half cover.
- **Range wall:** a cold cast-iron range, 5 ft. Full cover for a Medium
  creature crouching.
- **The chair** with its back to the party, 5 ft from the far door. Cass #1
  stands up out of it.
- **No windows.** Nothing to escape through. This is deliberate — session 1's
  fight is the first time the party can't leave a room.

*Tactics:* they open with Surprise Attack, spread to all four quarters, and
door-hop to break focus fire. **A party that jams the doors shuts down the
whole gimmick — let them, and let it feel smart.**

**Change #6:** the fight's other lesson lives here too — physically damaging
one of the four doorframes (a bad miss into it, a shove, deliberate
vandalism) removes it from the 4-set. Track which doorframe, if any, gets
wrecked; a Cass that tries to fold through it afterward fumbles and loses
its turn instead. If nobody damages one by round 3, force it: have a Cass
miss, get shoved, or collide with a frame, then have the next Cass fail to
fold through that same door a moment later. See the adventure's Session 1
climax for the full scripted version.

---

## 2. THE LANDING & COAT CLOSET — *rugs of smothering* (S2)

**Grid: 25 × 25 ft landing + a 10 × 30 ft closet.**

- **The closet is far deeper than the landing has room for** — that's visible
  from outside and worth describing before anyone steps in.
- **Two rows of hooks** down the closet's long walls, ~60 coats. Coats are
  difficult terrain to move through and block line of sight down the row.
- **The closet mouth is 5 ft wide.** The choke point is the whole tactical
  problem: three or four grapplers in a corridor where only one PC can be in
  front.
- **The heavy one** hangs at the far end and takes two rounds to work itself
  off its hook. Visible the whole time.
- **Landing:** a stair up (nowhere) and two doors out. Open enough to fight
  properly *if* the party backs out of the closet, which is the correct play.

*Tactics:* they grapple and drag toward the closet's back. Rescuing a
swallowed character is the whole fight.

---

## 3. AMBRY'S SQUAT — *three mimics* (S2)

**Grid: 20 × 25 ft.** A furnished room somebody lived in for three weeks.

- **FIVE DOORS.** Mark which three are mimics before play and don't change your
  mind. The other two are real and the party cannot tell.
- **The nest:** curtains and coats in a corner, 10 × 10 ft, difficult terrain.
- **Sixty preserve jars** stacked by size along one wall — knock the stack over
  and it's difficult terrain plus noise.
- **The tally wall** is the long wall opposite the nest. The glove sits on top
  of the nest.

*Tactics:* they stay doors until touched or until someone commits to opening
one. The fight starts when a PC has a hand on a doorknob — **that character is
adjacent to a mimic and gets grappled first.** Everyone else is 10–15 ft away
across a cluttered room.

---

## 4. THE OBLEX CHAMBER — *the midpoint* (S2)

**Grid: 40 × 60 ft.** A long hall, well-lit by nothing. **The biggest room in
the campaign so far and it should feel like it.**

- **Twelve duplicates** standing at conversational distances throughout —
  scatter them, don't cluster. **Six are live `Oblex Spawn` (CR ¼)**; the
  other six are inert set dressing. Don't tell the party which is which — both
  block line of sight and make the room feel awful, and the spawn only reveal
  themselves by acting.
- **Ambry** is roped to a chair leg at the far third, ~40 ft in. **His
  duplicate stands 4 ft from him.**
- **Furniture:** scattered chairs and two long side tables. Half cover,
  plentiful.
- **Two doors:** the one they came in by, and the one out — which leads to the
  "way home" kitchen. Not identical. No folding in this fight.
- **The oblex body** starts hidden among the duplicates. It reveals on its turn.

*Tactics:* it stays at range, uses duplicates as cover, and targets whoever
goes for Ambry. Freeing him costs an action and a cut cord.

---

## 5. THE WAY OUT — *Hesper, and the other pillar* (S4)

**Grid: 40 × 40 ft**, in the substrate: one continuous pale surface, floor to
ceiling, with the plan cut into the floor. **Ceiling 20 ft.**

- **THE EXIT DOORWAY** is centred on one wall. Just a door — no special rule
  governs it anymore; the party can leave through it at any point, at the
  normal cost of disengaging from a fight.
- **EIGHT OTHER DOORWAYS**, two per wall, cut straight into the substrate.
  Doppelganger copies enter through these, one per round from round 2 (see
  the adventure). Hesper's *Fold* also uses these, purely for mobility — no
  need to pre-pair them into sets anymore.
- **Three low plan-ridges of varying height and width**, cutting the floor
  unevenly — half cover, decorative/tactical terrain only now.
- **TWO PILLARS**, off to one side, squared-off, waist-to-shoulder height,
  identical to each other — unmarked on any map you show the players and not
  called out differently from each other on yours either. **One of them is a
  Roper** in False Appearance, reflavored as arms rather than tentacles
  (mechanically still its printed Tendril attacks). **Trigger note (Change
  #18): it activates on Hesper's first turn, not its own initiative — don't
  roll initiative for it at all.** See the adventure's "The Other Pillar"
  section for the exact timing.
- **No furniture. No clutter.** The room is deliberately austere.
- **Party copies** (0–5, one per long rest) start spread along the far wall.

**If you're running this with physical minis or a VTT:** use two identical
plain pillar pieces, or nothing at all, until one moves — don't put anything
monster-shaped on the table before the reveal. The moment it acts, **swap
that one pillar for a pillar-with-arms piece**, leaving its twin as it was;
one dramatic terrain swap sells the reveal better than a model that was
sitting there in plain sight the whole fight.

*Tactics:* see the adventure's finale section. Hesper fights straightforwardly
until her own first turn triggers the Roper's scripted reveal, which removes
her; after that it's a normal fight against the Roper and any surviving
copies.

---

## LIGHT SPECS — the two avoidable S3 fights

Run these theatre-of-mind unless the party engages.

**The 500-foot hallway** *(the late cats)* — 10 ft wide, 500 ft long, one
window at the far end. **Two** displacer beasts doze at the ~250 ft mark, a
few feet apart. **They see them from 400 ft away.** No cover for its whole
length; backing out is a 250 ft withdrawal and neither pursues past the
doorway.

**The drafted orchard** *(the still bears)* — a hall with no visible end,
trees on a perfect 20 ft grid, no bark. Trees give half cover and block line
of sight past ~60 ft. **Three** owlbears stand motionless, spaced out among
the trees. **They react to movement toward them, not past them** — the outer
rows are a clean bypass, and the grid makes "are we still going around them"
a legible question on a map.

---

## Related Files

- [`THE_ELL_AT_MARCHWELL.md`](THE_ELL_AT_MARCHWELL.md) — the adventure
- [`DM_SCREEN.md`](DM_SCREEN.md) · [`CHARACTERS.md`](CHARACTERS.md) ·
  [`REWARDS.md`](REWARDS.md)
