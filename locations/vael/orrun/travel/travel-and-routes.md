# TRAVEL_AND_ROUTES.md

---
type: geography
secrecy: player-safe
status: static
location_key: vael/orrun/travel/travel-and-routes
region: Orrun (continent-wide)
tags: [geography, travel, routes, roads, rivers, sea-lanes, tolls, hazards, scale, orrun]
related: [CONTINENT_OVERVIEW.md, regions/, ../02_settlements/, ../04_bestiary/]
---

## AI Use

Load for any travel question: how to get from A to B, how long it takes, what it costs, what goes wrong on the way. This file consolidates Orrun's named roads, rivers, and sea-lanes with general time and risk framing. Region-specific terrain and local custom live in `regions/`.

Risk levels here are **generic travel framing** — "bandit-prone," "treacherous in winter," "tolled" — usable in any game set in Vael.

---

## How Travel Works On Orrun

- **Distance is measured in days, not miles.** Locals give directions by landmarks and overnight stops.
- **The old Concord roads are the best ground anywhere.** Raised stone causeways built by an order that fell a century ago, still carrying most of the continent's traffic. Nobody maintains them. Long stretches have sunk, drowned, or vanished under forest, and the gaps are where trouble happens.
- **Water beats road for cargo.** The great rivers carry most freight, and everyone who owns a stretch of one tolls it.
- **Off-road roughly doubles time and adds real hazard.** Fen, deep forest, marsh, high pass, and open steppe all punish travelers who have no guide.
- **Guides are worth their fee** in fen, forest, delta, steppe, and salt-flat country. In several regions they are the difference between a journey and a disappearance.
- **Tolls are universal.** Bandit-tolls, lord-tolls, lock-tolls, league-tolls, pass-tolls, port-tolls. Budget for them; refusing is sometimes possible and rarely wise.

### Travel Rates

| Mode | Rate | Notes |
|---|---|---|
| Foot, good road, fair weather | ~15–20 miles/day | The default assumption |
| Cart or wagon, good road | ~20–25 miles/day | Slower on gradients; useless off-road |
| Off-road: fen, forest, marsh | Half rate or worse | Plus navigation risk |
| High pass | Highly variable | Closed entirely in winter |
| River barge, downstream | Fast and cheap | Limited by locks and tolls |
| River barge, upstream | Slower than walking | But it carries cargo |
| Coastal ship, fair season | Usually fastest | Weather-dependent; storm season stops it |
| Open-ocean voyage | Weeks | Fair season only |

### Seasons

| Season | Effect |
|---|---|
| Spring | Melt swells every river; fords impassable; mountain passes open late |
| Summer | Best travel season nearly everywhere; grass-fire risk on the steppe; heat lethal on the salt flats |
| Autumn | Floods in the north, gales on the west coast, storm season at sea, leaf-fall confusion in forest country |
| Winter | Northern passes shut; the northern ocean freezes; the northwest frontier becomes genuinely dangerous; southern delta remains workable but wet |

---

## The Northwestern Frontier Routes

The four frontier regions fan around the Sundering Reach — the Vale to the south, the Tollwood east, the Pale Coast west. All three overland roads, plus the Coast's sea-route, converge southeast on the city-state of **Caradril**.

### The South Road — Reach to Ashgarden Vale to Caradril

| Field | Detail |
|---|---|
| **Path** | Hollowmere → Candlewick → Tilbrook → Orchardmere → southern downs → Caradril |
| **Type** | Concord causeway, well kept |
| **Time** | ~5–6 days Hollowmere to Orchardmere; ~5–6 more to Caradril (≈11–12 total) |
| **Terrain** | Fen gives to hedged farmland, then open sheep-downs |
| **Risk** | **Low.** The safest road on the frontier — patrolled, busy with carts and pilgrims |
| **Watch for** | Old barrows on the downs that shepherds leave alone; the odd washed hedge-ford after rain |

### The East Road — Reach to Tollwood to Caradril

| Field | Detail |
|---|---|
| **Path** | Hollowmere → Kettle Bridge → Tollstone Cross → Hartfell → forest edge → Caradril |
| **Type** | Concord toll-causeway, partly overgrown |
| **Time** | ~4–5 days Hollowmere to Hartfell; ~5–6 more to Caradril |
| **Terrain** | Fen dries to old-growth forest; the road is the only safe thread |
| **Risk** | **Moderate. Bandit-prone.** A standing bandit-toll at Tollstone Cross, a drowned causeway stretch called the Green Mile, real predators, and deep forest immediately off the verge |
| **Watch for** | Stay on the road. Leave an offering at the toll-shrines — the locals consider this mandatory. Off-road navigation is genuinely hard |

### The Pale Road — Reach to Pale Coast

| Field | Detail |
|---|---|
| **Path** | Hollowmere → Saltmargin → Cobble Strand → Wrackmouth |
| **Type** | Marsh track then cliff-road |
| **Time** | ~5 days to Saltmargin; ~3 more to Wrackmouth (≈7–8 total) |
| **Terrain** | Salt-marsh gives to sea-cliffs and shingle coves |
| **Risk** | **Moderate.** Cliff-falls, sea-fog, and wreckers and smugglers on the wild coast |
| **Watch for** | Fog closing on an exposed cliff-road; tide-cut sections |

### The Coastal and River Route — Pale Coast to Caradril

| Field | Detail |
|---|---|
| **Path** | Wrackmouth → by sea down the coast → the Verdance mouth → upriver → the Stillwater → Caradril |
| **Type** | Coastal sea-lane then navigable river |
| **Time** | ~6–7 days by ship, weather permitting. An overland alternative south along the coast runs ~8–9 days and is rougher |
| **Risk** | **Moderate at sea, low on the river.** Storms and tides offshore; calm and lawful once on the Verdance |
| **Watch for** | Storm season. Keep well clear of the Skerries — the offshore reefs are the coast's wreck-ground and no local will take a small boat near them |

**Which frontier route to take:** the sea-route is fastest and safest, the Vale road is the gentlest overland, the forest road is the riskiest and the most direct east.

---

## The Continental Routes

### The Verdance Road — Caradril to the Glassmere League

| Field | Detail |
|---|---|
| **Path** | Caradril → Marrowfen Stair → the Nine Locks → Glassmere |
| **Type** | River corridor: towpath, road, and barge |
| **Time** | ~12–16 days by road; about two weeks by barge if the locks run well |
| **Risk** | **Low–moderate. Heavily tolled.** Lock-tolls, lordling-tolls, river-pirates past the Locks who prefer a toll to a fight; flooding in spring |
| **Notes** | The standard first step from the northwestern frontier into settled inland Orrun. A parallel bluff road runs slower but toll-free |

### The Glasswater Run — Glassmere to the Hollow Gulf

| Field | Detail |
|---|---|
| **Path** | Glassmere → Cairnwater → the Mardenflow confluence → Calderport |
| **Type** | Great-river trade corridor |
| **Time** | ~3–4 weeks downstream |
| **Risk** | **Moderate. Tolled at every opportunity.** River piracy in the middle reaches, delta fever at the southern end, seasonal floods |
| **Notes** | The continent's main commercial artery. Everything moves on it |

### The Crown Road (the Greatspine Passes) — Glassmere to the Concord Heartlands and south

| Field | Detail |
|---|---|
| **Path** | Glassmere → the Greatspine pass → Crownmouth → onward south |
| **Type** | Mountain-pass road |
| **Time** | ~2–3 weeks to the ruin-country; well-traveled as far as Crownmouth, effectively abandoned past it |
| **Risk** | **High. Contested.** Warlord checkpoints, scavenger-tolls, mountain weather, and rival expeditions. The passes are shut by snow for months |
| **Notes** | Beyond Crownmouth's gate there is no law of any kind |

### The Salt Road — Pale Coast to the Saltmere Reaches

| Field | Detail |
|---|---|
| **Path** | Wrackmouth → the Mirewend Sinks edge → mid-continent → Marrowmoot → Brackhold → the Saltmere |
| **Type** | Overland caravan track |
| **Time** | Weeks; the chalk-downs leg alone runs about a week |
| **Risk** | **Moderate, rising east. Thinning and tolled.** Bog fords, shire-tolls, long exposed stretches, and salt-clan raiders at the far end |
| **Notes** | A long haul through emptying country. Caravan masters run it on a schedule; solo travelers should attach themselves to one |

### The Hethe Tollway — Karran Marches to the eastern coast

| Field | Detail |
|---|---|
| **Path** | Karran-Gate → Tollreach → Hethemoot reach → the Calm Reach coast |
| **Type** | Forest-river toll corridor |
| **Time** | Weeks end to end |
| **Risk** | **High. Outlaw-shadowed and heavily tolled.** An outlaw river-toll camp sits on the water-road; toll-lords take their cut at both ends; the deep forest is prohibited by the free-holds themselves |
| **Notes** | Tollreach is a **danger waypoint, not a stop** — no inn, no resupply, no safe rest. Travelers pay, negotiate, or take a deep-wood bypass ford that needs real woodcraft. The nearest service town is Hethemoot |

### The South Sea Lanes — the Hollow Gulf to lands overseas

| Field | Detail |
|---|---|
| **Path** | Calderport / Saltgate → open water → the far southern continent |
| **Type** | Open-ocean shipping lane |
| **Time** | Weeks |
| **Risk** | **High out of season.** Open-ocean storms and privateers; fair-season sailing only |
| **Notes** | The only regular way off Orrun. Passage is expensive and berths are booked around the storm calendar |

### The Steppe Tracks — the Wender Steppe and the settled south

| Field | Detail |
|---|---|
| **Path** | Seasonal migration and trade lines between the winter-camp, the Summer-Riding's circuit, and the Spine-Foot trade-meet |
| **Type** | Unroaded seasonal tracks |
| **Time** | Highly variable |
| **Risk** | **High without a clan guide.** No tolls, no safety, no law. Cold, distance, water, blizzards, grass-fires, and raiders |
| **Notes** | Guest-law is the only protection that means anything out here — and it means a great deal. Travelers frequently move with the clan-host because doing otherwise is worse |

### Regional And Approach Routes

| Route | Where | Character | Risk |
|---|---|---|---|
| **The Ash Roads** | Western approach to the volcanic theocracy | Warden-post pilgrim way; the only sanctioned entry | Controlled; environmentally harsh |
| **The Green Roads** | Between the southern sacred groves | Carved-stone pilgrim paths, kept clear | Low for the respectful |
| **The Mardenflow river-road** | The southern delta, north to south | Channels, ferries, and flood-cut tracks | Moderate; fever, tide, and shifting water |
| **The Fever Channels** | Deep southern delta | Smuggler water; local pilots only | Very high unpiloted |
| **The Reach Lanes** | Between the southern Gulf ports | Busy coastal hops | Low–moderate; privateers |
| **The Bonepan Track** | Salt sea to the southern coast | Dry-season desert crossing, 4–6 days | High; water carried in, heat and glare |
| **The Iron Road** | The northeastern mining frontier | Partly Concord-paved north-south spine | Moderate–high; warlord tolls, snow |
| **The Ghostmark Pass** | Salt sea north to the ruin-country | Poorly kept mountain route | High; weeks of exposure |
| **The Highmark Passes** | The far northern barrier range | Uninhabited high crossings | Extreme; no settlements, no help, closed most of the year |

---

## Route Selection At A Glance

| Going from | To | Best route | Why |
|---|---|---|---|
| The northwestern frontier | Caradril | The Coast's sea-and-river route | Fastest and safest; ~6–7 days from Wrackmouth |
| Caradril | Inland Orrun | The Verdance Road | The standard corridor into the settled interior |
| The river-cities | The southern coast | The Glasswater Run | Cheap, tolled, and unavoidable for cargo |
| The southern coast | Overseas | The South Sea Lanes | The only way off the continent |
| The river-cities | The central ruins | The Crown Road | Contested, and there is no better option |
| The northwest | The salt sea | The Salt Road | Long, thin, and best done with a caravan |
| The northeast | The eastern coast | The Hethe Tollway | Fast on the water, expensive at the tolls |
| Anywhere | The steppe | Attach to a clan | There is no other reliable way to cross it |

---

## Related Files

- [`CONTINENT_OVERVIEW.md`](../CONTINENT.md) — the shape of the world these routes cross
- [`regions/`](../regions/) — terrain, custom, and local conditions region by region
- [`../02_settlements/`](../settlements/) — the towns at the ends of these roads
- [`../04_bestiary/`](../bestiary/) — wandering threats and hazards by terrain
