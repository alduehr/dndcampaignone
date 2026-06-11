# TRAVEL_ROUTES_RING1.md — Ring 1 Travel Routes

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: [Cinder Ledger, Reachward Compact, Gravecallers]
level_range: 1-8
related: [MAP_DESCRIPTION.md, ../05_regions/SUNDERING_REACH.md, ../05_regions/ASHGARDEN_VALE.md, ../05_regions/TOLLWOOD.md, ../05_regions/PALE_COAST.md, ../06_settlements/CARADRIL.md]
tags: [type:travel, secrecy:mixed, ring-1, function:travel]
---

## AI Use

Load for any overland or sea travel between the Sundering Reach and its three Ring 1 neighbors (Ashgarden Vale, Tollwood, Pale Coast) and on to Caradril. Holds route options, times, dangers, terrain, faction presence, and travel events per route. Use with `../01_runner_protocol/TRAVEL_PROTOCOL.md` and the relevant regional encounter table. Travel here should create *decisions*, not empty filler.

## Ring 1 Travel Map (Relative)

```
                 SUNDER HEIGHTS (N)
                       |
   PALE COAST (W) — SUNDERING REACH — TOLLWOOD (E)
        |   \          |                    \   |
        |    \   ASHGARDEN VALE (S)          \  |
        |     \________|_____________________ \ |
        \              |                       CARADRIL (SE)
         \____ (sea + Verdance river) _________/
```

- **From the Reach, the player can leave in three overland directions** — south (Vale, via Candlewick), east (Tollwood, via Kettle Bridge), west (Pale Coast, via Saltmargin) — **and all three roads, plus the Coast's sea-route, converge on Caradril (SE).**
- **Gateway towns (already built in the Reach):** Candlewick (→ Vale), Kettle Bridge (→ Tollwood), Saltmargin (→ Pale Coast). These are the player's on-ramps outward.

## Scale & Assumptions

- Point-to-point on foot/cart unless a ship is noted. Off-road travel doubles or triples time and adds hazard.
- Times assume fair-to-poor autumn weather (campaign start = Greyfall). Storms, floods, and the worsening dead can lengthen any route.
- Use `TRAVEL_PROTOCOL.md` for journey pacing (travel checks, watches, rests) and the regional encounter tables for events.

---

## Route 1 — Reach → Ashgarden Vale (South Road)

| Field | Detail |
|---|---|
| **Path** | Hollowmere → Candlewick (S edge of the Reach) → **South Road (Concord causeway)** → Tilbrook → Orchardmere |
| **Time** | Hollowmere → Candlewick ~1–2 days (in-Reach); Candlewick → Tilbrook ~1–2 days; Tilbrook → Orchardmere ~1–2 days. **~5–6 days total** Hollowmere → Orchardmere. |
| **Terrain** | Rising firm ground; fen gives to hedged farmland; the safest, best-kept road in Ring 1. |
| **Risk** | **Low.** Patrolled by harvest-moot wardens; busy with carts and pilgrims. |
| **Faction presence** | Reachward Compact (nominal), Cinder Ledger (carts, the salt-trade north), Mourners' Circle (shrine-country). |
| **Encounter table** | `ASHGARDEN_VALE_ENCOUNTERS.md` (Zone 1) once in the Vale; Reach Roads table before. |
| **Events/complications** | A field-shrine the orchard grew around (M2 seed); a "saint's relic" peddler (M3); a reburied grave that won't hold (M5/the Vale's denial); a Ledger relic-cart bound south (M3/Monopoly). |

## Route 2 — Reach → Tollwood (East Road)

| Field | Detail |
|---|---|
| **Path** | Hollowmere → Kettle Bridge (E toll-town) → **East Road (Concord toll-causeway)** → Tollstone Cross → Hartfell |
| **Time** | Hollowmere → Kettle Bridge ~1 day (in-Reach); Kettle Bridge → Tollstone Cross ~2 days; Tollstone Cross → Hartfell ~2 days. **~4–5 days total** to Hartfell. |
| **Terrain** | Fen dries to old-growth forest; the road is the only safe thread; off-road = getting lost (Survival DC 14+). |
| **Risk** | **Moderate.** Bandit-tolls (Tollstone Cross), washed-out causeway (the Green Mile), real predators (dire wolves), and the deep wood off-road. |
| **Faction presence** | Cinder Ledger (logging, road-trade), Reachward Compact (thin road-watch), Gravecallers (sheltered cells deeper), woodfolk (the forest-rules). |
| **Encounter table** | `TOLLWOOD_ENCOUNTERS.md` (Zone 1 on the road; Zones 2–3 only if going deep). |
| **Events/complications** | The toll-chain (negotiate/pay/fight); a Coppice Shrine offering (safe-passage custom); the Green Mile (drowned road; M2/M5 fragment); a logging crew back short a man (the deep-cutting danger); dire wolves at dusk. **Stay on the road — the deep wood is gated and dangerous.** |

## Route 3 — Reach → Pale Coast (Pale Road)

| Field | Detail |
|---|---|
| **Path** | Hollowmere → Saltmargin (W salt-town) → **Pale Road (coast road)** → Cobble Strand → Wrackmouth |
| **Time** | Hollowmere → Saltmargin ~5 days (in-Reach, salt-marsh — *already established*); Saltmargin → Cobble Strand ~2 days; Cobble Strand → Wrackmouth ~1–2 days. **~7–8 days total** to Wrackmouth. |
| **Terrain** | Salt-marsh gives to sea-cliffs and coves; the cliff-road is the safe thread; the sea and tides are the great hazard. |
| **Risk** | **Moderate.** Cliff-falls, sea-fog, the drowned-tide, wreckers and smugglers on the wild coast. |
| **Faction presence** | Cinder Ledger (the salt monopoly; Saltmargin → Wrackmouth), Mourners' Circle (the salt-and-tide faith), Gravecallers (a cove/wrecker current), smugglers (Gull's line reaches here). |
| **Encounter table** | `PALE_COAST_ENCOUNTERS.md` (Zone 1 on the cliff-road; Zones 2–3 for the coves/sea). |
| **Events/complications** | A headland sea-shrine offering; a drowned-cairn that won't hold (M5); a Ledger sea-relic cart (M3/Monopoly); sea-fog on the cliff-road; the Drowned Lamp "lighting" in the fog (M2 telegraph, gated). |

## Route 4 — Ashgarden Vale → Caradril (Southern Approach)

| Field | Detail |
|---|---|
| **Path** | Orchardmere → **South Road** across the southern downs → Caradril's northern hinterland → Caradril |
| **Time** | **~5–6 days** Orchardmere → Caradril. (Hollowmere → Caradril via the Vale ≈ 11–12 days total, matching `MAP_DESCRIPTION.md`.) |
| **Terrain** | Open sheep-downs; the best road to the city; drovers and trade. |
| **Risk** | **Low-moderate.** Open, patrolled near the city; a few pre-Concord barrows on the downs best left alone; the odd Vale-leakage Remembrance. |
| **Faction presence** | Cinder Ledger (the city trade; relic-carts south), Reachward Compact (fades toward Caradril's reach), Concord Remnant (scholar-traffic to the city). |
| **Events/complications** | A relic-cart bound for the Ashmarket (M3; links to Caradril's quiet-coin); a Remnant scholar traveling to the Lantern Reach; a down-barrow's old dead; the city's wealth and watch increasing as you near. |

## Route 5 — Tollwood → Caradril (Eastern Approach)

| Field | Detail |
|---|---|
| **Path** | Hartfell → **East Road** on through the forest's eastern edge → Caradril's eastern hinterland → Caradril |
| **Time** | **~5–6 days** Hartfell → Caradril. |
| **Terrain** | Forest thins to farmland near the city; the East Road improves as it nears Caradril. |
| **Risk** | **Moderate near Hartfell** (the toll-war, the deep wood) **easing toward the city.** The road's safety depends on the toll-war's state. |
| **Faction presence** | Cinder Ledger (timber/charcoal trade to the city), Reachward Compact (fades), Gravecallers (couriers between the wood-cells and the city). |
| **Events/complications** | The toll-war's state determines safety (clear it via `Q_THE_TOLL_WAR` to ease this route); a timber-cart convoy; a Gravecaller courier bound for the city; the forest's old dead thinning as the wood opens. |

## Route 6 — Pale Coast → Caradril (Coastal / Verdance River Route)

| Field | Detail |
|---|---|
| **Path** | Wrackmouth → **by sea down the coast → up the Verdance river → the Stillwater → Caradril** (the Coast's distinctive water-route) |
| **Time** | **~6–7 days by ship/boat**, weather permitting — **often faster and safer than the overland routes**, and a real reason to favor the Coast. An overland alternative (Wrackmouth → south along the coast → Caradril's hinterland) runs ~8–9 days and is rougher. |
| **Terrain** | Open sea, then the broad Verdance into the Stillwater (Caradril's harbor-lake) — a grand arrival by water. |
| **Risk** | **Moderate (the sea).** Storms, tides, and (off the wild coast) wreckers; once on the Verdance, calm and lawful. **Gated:** do not route a low-level boat near the Skerries. |
| **Faction presence** | Cinder Ledger (the salt/relic shipping; the same hulls), honest skippers (Wenna Roke — the player's lift), the Tide-Watch at the Stillwater. |
| **Events/complications** | A storm or fair wind (Survival/seamanship; the route's defining check); a Ledger relic-hull bound for the Counting-Quays (M3/Monopoly; a thread into Caradril); the grand arrival at the Stillwater quays; a wrecker scare off the wild coast (avoid the Skerries — gated). |

---

## Cross-Region Notes

- **All routes funnel to Caradril (SE):** the player can reach the mid-game hub from any Ring 1 region, by their preferred terrain (downs, forest, or sea). The Coast's water-route is the fastest/safest; the Vale's is the gentlest overland; the Tollwood's is the riskiest.
- **The Mourners' folk-truth network** (Wend → Combe → Sennet → Bryd) runs *between* the regions; carrying their messages (AV-H20, TW-H20, PC-H17) is a slow, gated M6 thread that links the regional Mourners and rewards the well-traveled player.
- **The Ledger's relic-carts and hulls** move on every route, all bound for Caradril (the Monopoly clock's logistics made visible; M3). Following the carts is a through-line from any Ring 1 region into the city's Counting-Quays/Ashmarket.
- **Faction consequences travel:** clearing the Tollwood toll-war eases Route 5; easing the Coast salt-gouge eases the whole frontier; the Vale's denial cracking sends Mourners and scholars onto the roads. Travel reflects the world-state.

## Related Files

- [`MAP_DESCRIPTION.md`](MAP_DESCRIPTION.md)
- [`../05_regions/SUNDERING_REACH.md`](../05_regions/SUNDERING_REACH.md) · [`../05_regions/ASHGARDEN_VALE.md`](../05_regions/ASHGARDEN_VALE.md) · [`../05_regions/TOLLWOOD.md`](../05_regions/TOLLWOOD.md) · [`../05_regions/PALE_COAST.md`](../05_regions/PALE_COAST.md)
- [`../06_settlements/CARADRIL.md`](../06_settlements/CARADRIL.md)
- [`../01_runner_protocol/TRAVEL_PROTOCOL.md`](../01_runner_protocol/TRAVEL_PROTOCOL.md)
- Regional encounter tables: `../13_encounters_and_bestiary/ASHGARDEN_VALE_ENCOUNTERS.md` · `TOLLWOOD_ENCOUNTERS.md` · `PALE_COAST_ENCOUNTERS.md`
