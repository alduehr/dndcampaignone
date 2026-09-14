# WORLD_MAP_LAYERS.md — Map Layer Definitions

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: [Cinder Ledger, Concord Remnant, Mourners' Circle, Ashen Wardens, Gravecallers, Reachward Compact, Hollow Court]
level_range: 1-20
related: [WORLD_MAP_AUTHORITY.md, WORLD_MAP_COORDINATES.md, WORLD_MAP_PROMPTS.md, ../11_mysteries_and_secrets/MYSTERY_WEB.md, ../11_mysteries_and_secrets/REVELATION_MAP.md, ../02_runtime_state/WORLD_CLOCKS.md]
tags: [type:map, secrecy:mixed, function:cartography, layers, orrun]
---

## AI Use

Defines the **seven map layers** for Vael/Orrun's NW quarter. Each layer is a filtered view of the same base geography (`WORLD_MAP_COORDINATES.md`). Use this to decide **what to show, label, and hide** when generating a specific map, and to keep DM-only geography off player-facing renders. Layers 2 and 7 are **DM-only** — never show them to the player.

**Golden rule:** only **Layer 1** (and the player-safe parts of Layer 5/6) may be shown to the player. Everything else is prep-only.

---

## Layer 1 — Player-Safe World Map

**Audience:** the player. Safe to render and share.

- **Shown:** the 5 regions (Reach, Vale, Tollwood, Coast, Caradril) with labels; the Pale Sea; the Verdance, Mirewend, and Ammet rivers; the Stillwater; the Sunder Heights; the Greyfens; the southern downs; the Highmark Spine as a far-N mountain edge; all known settlements (Reach 8, Ring 1 hubs/villages, Caradril); the named roads (South/East/Pale Roads, Concord causeways) and the Coast sea-route; the Hollowmere basin as a labeled flooded landmark.
- **Labels:** region names, settlement names, river names, road names, "Pale Sea," "Sunder Heights," "the Highmark Spine" (loose far-N label), "Hollowmere basin (drowned Concord ruin)."
- **Hidden:** the drowned-shrine **interior/keystone truth**, the Concord Deep, the Under-Shrine, all node-network links, all gated dungeon lower-levels, faction *hidden* territory, the Verdance Reaches' specifics (show only an edge-arrow "to Caradril & inland Orrun").
- **Notes:** the basin may be drawn ominous but unexplained. Show the Old Mast, the Skerries, and the Drowned Lamp only as **labeled hazard landmarks** ("deep wood — do not enter," "wrecking reef," "ruined lighthouse"), never as nodes.

## Layer 2 — DM-Only World Map

**Audience:** AI DM only. **Never render for the player.**

- **Shown:** everything in Layer 1, PLUS — the **node-network** as connecting lines (keystone basin ↔ Deep Adit [Harrowgast] ↔ Sunken Tollhouse [Kettle Bridge] ↔ Saint Veddow's Tomb [Vale] ↔ Drowned Lamp/Skerry Shrine [Coast] ↔ Sunken Wards [Caradril] ↔ Tollwood deep [oblique]); the **Concord Deep** (subsurface network sink under the basin); the **Under-Shrine / Drowned Keystone** (endgame, beneath Hollowmere); the gated dungeon lower-levels; the Gravecaller cells (Greyfens Drowned Blind, Hanging Oaks, Coast wreckers); the Hollow Court's seat (under the basin).
- **Labels:** node names, network links, "keystone," "secondary node," "minor node/relay," "pre-Concord (built over)," forbidden-zone markers.
- **Hidden from this layer too:** nothing of the mapped quarter; but the broader Orrun continent and other surviving Custodians (if any) remain off-map/future.
- **Notes:** mark which nodes are **warming** (driven by `WORLD_CLOCKS.md` master clock #1). The endgame is **vertical** (down from the basin), so render it as a depth-callout, not a lateral region.

## Layer 3 — Faction Influence Map

**Audience:** DM (a player-safe simplified version can be shown if the player has earned faction intel).

- **Shown:** faction territories, contested zones, neutral ground, over the base geography.
  - **Cinder Ledger:** strongest at Caradril (HQ) and the Pale Coast salt-trade; relic-carts on every road; Vale mortgages; Tollwood logging. Shade as a **trade-web**, not a border.
  - **Reachward Compact:** nominal across the Reach and Ring 1; real grip only near Hollowmere; fades toward Caradril (which is outside it).
  - **Mourners' Circle:** strongest in the Vale (oldest chapter) and Coast (salt-and-tide); present everywhere; the folk-truth network runs region-to-region.
  - **Ashen Wardens:** wandering Reach-wide; resident chapter at Saint Veddow's (Vale); thin on the Coast/Tollwood.
  - **Gravecallers:** hidden cells — Greyfens (Reach), Hanging Oaks (Tollwood), wrecker coves (Coast); strongest where rites fail worst.
  - **Concord Remnant:** seat at Caradril (Lantern Reach); scholar-traffic to Saint Veddow's, the Drowned Lamp, the Tollwood toll-roads; Reclamation crews at the Deep Adit.
  - **Hollow Court (DM-only):** no surface territory — influence radiates from the basin through agents; show only on Layer 2.
- **Labels:** faction names, "contested," "neutral," clock-state markers.
- **Hidden:** Hollow Court influence (DM-only); hidden agendas (show public face only on any player-facing version).

## Layer 4 — Mystery / Revelation Map

**Audience:** DM only.

- **Shown:** locations tied to each mystery (M1–M9) and revelation gates, over the base geography.
  - **M2 (the source/network):** basin, Surfacing Ruin, Sunken Tollhouse, Saint Veddow's, Drowned Lamp, Sunken Wards.
  - **M3 (Remembrance is collected/sold):** Ledger Vault (Hollowmere), Ashmarket/Counting-Quays (Caradril), Pellow Grange (Vale), sea-relic trade (Coast), "old glass" (Harrowgast).
  - **M5 (failures radiate outward from the keystone):** the honest windows — Tilbrook (Vale), Coldhearth (Tollwood), Cobble Strand (Coast), Greywater Holm (Reach); Sashe's mapped drift converging on the basin.
  - **M6/M9 (the Concord's sin / deliberate Quietfall):** the Sealed Archive (Caradril), the Whispering Cairn (Reach), the Barrow of Nine Doors, the Vale Mourners (Combe), the Tollwood deep witness (gated/oblique).
  - **M7 (the Hollow Court — apex):** the Under-Shrine only (Layer 2/late-arc).
- **Labels:** mystery codes (M1–M9), "clue site," "revelation gate," act-tier.
- **Hidden:** the **answers** themselves; M7 location until late arc.
- **Notes:** enforce the three-clue rule visually — each revelation should show ≥3 lit sites across different regions, so a player who avoids one region is never blocked.

## Layer 5 — Level-Tier Danger Map

**Audience:** DM (a softened player-safe version — "rough country / very dangerous" — can be shown).

- **Shown:** color-coded danger bands over the base geography.
  - **Lvl 1–4 (green):** Hollowmere, Reedford, Candlewick, the central/south Concord roads, the Ashwalk Rest, Tilbrook, Orchardmere, the South Road, near-Wrackmouth/Cobble Strand, the East Road near Hartfell.
  - **Lvl 5–8 (yellow):** the Greyfens deep, the Sunder Heights/Harrowgast, the mid-Tollwood, the Coast coves/Drowned Lamp headland, Caradril's deeper intrigues and the Sunken Wards upper.
  - **Lvl 9–12 (orange):** Caradril's apex politics, the Sealed Archive, deeper Reclamation sites, Ring 2 (the Verdance Reaches).
  - **Lvl 13–16 (red):** the Concord Deep, the Old Mast deep, the Skerries deep, the path to the keystone.
  - **Lvl 17–20 (black):** the Under-Shrine / Drowned Keystone (beneath the basin).
- **Labels:** level bands; "telegraphed lethal" markers on gated sites.
- **Hidden:** the *reason* a zone is lethal (DM-only); on the player version, show only "rough"/"deadly," not node-truth.
- **Notes:** every gated/black zone must carry a **visible warning** so a low-level PC is never ambushed into the endgame.

## Layer 6 — Travel-Route Map

**Audience:** the player (route geometry is player-safe) + DM (danger annotations).

- **Shown:** all 6 named routes from `TRAVEL_ROUTES_RING1.md` plus in-Reach roads, with time and danger annotations.
  - Route 1 South Road (Reach→Vale, ~5–6 d, low risk).
  - Route 2 East Road (Reach→Tollwood, ~4–5 d, moderate).
  - Route 3 Pale Road (Reach→Coast, ~7–8 d, moderate).
  - Route 4 Vale→Caradril (~5–6 d, low-moderate).
  - Route 5 Tollwood→Caradril (~5–6 d, moderate).
  - Route 6 Coast→Caradril sea/Verdance (~6–7 d, the fast water-route).
- **Labels:** route names, day-counts, risk level, gateway towns (Candlewick/Kettle Bridge/Saltmargin).
- **Hidden:** secret/DM-only routes — the **node-network "arteries"** the roads secretly follow (Layer 2), Gravecaller courier paths, smuggler runs (Gull's line). Show smuggler/wrecker routes only if the player has earned that intel.
- **Notes:** all routes funnel to Caradril (SE). Mark the Coast water-route as fastest/safest.

## Layer 7 — Late-Game Hidden Truth Map

**Audience:** DM only. **The deepest secret layer. Never render for the player.**

- **Shown:** the **true shape of the ancient world beneath the current one** — the **Concord Deep**: the continental harvest-network as the Concord built it, with the **Hollowmere basin keystone** as the hub and every surface ruin (Reach nodes, Saint Veddow's, the Drowned Lamp/Skerry Shrine, the Sunken Wards, the Sunken Tollhouse, the Deep Adit) as a tapped node; the **pre-Concord things the network was built OVER** (the Barrow of Nine Doors, the Tollwood's Old Mast) marked distinctly as *older than the Concord*; the **Under-Shrine / Drowned Keystone** and the Hollow Court's dormant seat at the very bottom; the **Quiet Country** noted as the cosmological "drain" the whole machine fed (off-map, non-spatial).
- **Labels:** "keystone," "node," "relay," "pre-Concord (co-opted)," "Quietfall sever-points," "Under-Shrine (endgame)," warming-state per clock #1.
- **Hidden:** this layer IS the hidden truth — it exists only for the DM to keep the underground geography consistent across the campaign.
- **Notes:** this is the **"map beneath the map."** The surface roads the player walks are the machine's arteries. The endgame is reached by going **down** through the keystone, not across. Do not let any rendered artifact of this layer leak into player-facing files or prompts.

---

## Layer-to-Prompt Mapping

| Map prompt (in `WORLD_MAP_PROMPTS.md`) | Layers used |
|---|---|
| 1. Player-safe full-world map | Layer 1 (+ player-safe Layer 6 routes) |
| 2. DM-only full-world map | Layers 1+2+3+4+5+6+7 (full) |
| 3. Parchment regional reference (Reach + Ring 1) | Layer 1 cropped + player-safe Layer 6 |
| 4. Clean functional AI/reference map | Layer 1 base + DM toggles for Layers 2–7 (prep use) |

## Related Files

- [`WORLD_MAP_AUTHORITY.md`](WORLD_MAP_AUTHORITY.md) · [`WORLD_MAP_COORDINATES.md`](WORLD_MAP_COORDINATES.md) · [`WORLD_MAP_PROMPTS.md`](WORLD_MAP_PROMPTS.md)
- [`TRAVEL_ROUTES_RING1.md`](TRAVEL_ROUTES_RING1.md)
- [`../11_mysteries_and_secrets/MYSTERY_WEB.md`](../11_mysteries_and_secrets/MYSTERY_WEB.md) · [`../11_mysteries_and_secrets/REVELATION_MAP.md`](../11_mysteries_and_secrets/REVELATION_MAP.md)
- [`../02_runtime_state/WORLD_CLOCKS.md`](../02_runtime_state/WORLD_CLOCKS.md)
- [`../03_canon/DM_ONLY_CANON.md`](../03_canon/DM_ONLY_CANON.md) (do not surface)
