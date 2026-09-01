# FULL_WORLD_MAP_LAYERS.md — Full-World Map Layer Definitions

---
type: region
secrecy: mixed
status: static
region: Orrun
factions: [Cinder Ledger, Concord Remnant, Mourners' Circle, Ashen Wardens, Gravecallers, Reachward Compact, Hollow Court]
level_range: 1-20
related: [FULL_WORLD_MAP_AUTHORITY.md, FULL_WORLD_MAP_COORDINATES.md, FULL_WORLD_MAP_PROMPTS.md, WORLD_MAP_LAYERS.md, ../11_mysteries_and_secrets/MYSTERY_WEB.md, ../11_mysteries_and_secrets/REVELATION_MAP.md, ../02_runtime_state/WORLD_CLOCKS.md]
tags: [type:map, secrecy:mixed, function:cartography, layers, orrun, full-continent]
---

## AI Use

Defines the **eight map layers** for the full continent of Orrun. Each is a filtered view of the same base geography (`FULL_WORLD_MAP_COORDINATES.md`). Use this to decide **what to show, label, and hide** when generating a whole-world map, and to keep DM-only geography off player-facing renders. **Layers 2, 4, and 7 are DM-only — never show them to the player.**

**Golden rule:** only **Layer 1**, the player-safe parts of **Layer 6**, the softened player-version of **Layer 5**, and the **Layer 8 standalone zoom map** (campaign area) may be shown to the player. Everything else is prep-only. `WORLD_MAP_LAYERS.md` remains the layer authority for the **campaign-area zoom**; this file governs the **full continent**.

**Important (no inset on the player-safe full-continent map):** the player-safe full-continent map (Prompt 1) is **one continuous map**. The NW campaign frontier is shown directly on the main continent with somewhat higher local detail — **NOT** as an inset, mini-map, overlay, callout map, or "you are here" box. Layer 8 (the campaign-area standalone zoom map) is a **separate** map (Prompt 5); it is **never embedded into Prompt 1**.

---

## Layer 1 — Player-Safe Full-World Map

**Audience:** the player. Safe to render and share.

- **Shown:** the full continent of Orrun; all coasts and the named seas/oceans (Pale Sea W, Sunder Ocean N, Calm Reach SE/S, Hollow Gulf S bay, Saltmere inland sea, Wracking Straits far W); major ranges (Highmark Spine N, Karran Teeth NE, the Greatspine/Sundering Wall central, the Emberfells SE volcanic, Ghostmark S); major rivers (Verdance, Glasswater, Mardenflow, Hethe, plus the NW Mirewend/Ammet); major forests (Tollwood, Hethewood, Sunmark Wilds); the steppe, downs, deltas, and badlands as terrain; all **player-safe regions** with labels; the NW campaign cluster's known settlements; the long-distance roads and sea-lanes as travel threads; the Concord Heartlands shown only as a labeled distant ruin-country ("the fallen Concord heart — ruins, contested").
- **Labels:** continent name "Orrun (world of Vael)"; region names (player-safe ones); sea/ocean/bay names; range, river, forest names; the NW cluster's labels (as on the campaign map); "to overseas lands" edge-arrows S and N.
- **Hidden:** the Concord Deep, the Under-Shrine/keystone truth, all node-network links, all gated dungeon depths, faction *hidden* territory, the deep interior of placeholder regions (show region label + edge, not invented internal detail), the exact nature of the rumored ruins (Cindern works, Drowned Steps, Saltmere drowned towns — show as labeled mystery-landmarks only).
- **Notes:** placeholder regions are drawn **faint / low-detail** (a name and a tinted area) until built. The campaign cluster is the only high-detail zone; everything else is "the known shape of the wider world."

## Layer 2 — DM-Only Full-World Map

**Audience:** AI DM only. **Never render for the player.**

- **Shown:** everything in Layer 1, PLUS — the **node-network** drawn ONLY within the NW campaign cluster (keystone basin ↔ Deep Adit ↔ Sunken Tollhouse ↔ Saint Veddow's Tomb ↔ Drowned Lamp/Skerry Shrine ↔ Sunken Wards ↔ Tollwood deep [oblique]); the **Concord Deep** and **Under-Shrine/Drowned Keystone** as a depth-callout **beneath the NW cluster** (NOT spread across the continent); the surface-Concord ruin-truth of the far regions (the Concord Heartlands as the order's fallen *surface* capital; the Cindern/Saltmere/Drowned Steps as pre-Concord or surface echoes) marked distinctly from the underground keystone; forbidden-zone markers; the off-map note for Surren / the Iron Skards / the Sundered Isles and "other surviving Custodians: undefined, off-map."
- **Labels:** node names and links (cluster only), "keystone (under Hollowmere — vertical)," "surface-Concord ruin (NOT a node)," "pre-Concord echo," forbidden markers, warming-state per `WORLD_CLOCKS.md` clock #1.
- **Critical secrecy:** the network and keystone are **local and vertical**. Do **NOT** draw network lines out to the far continent. Far ruins corroborate the theme; they are not the machine. The endgame is under the starting town.

## Layer 3 — Faction Influence Map

**Audience:** DM (a player-safe simplified version if the player has earned faction intel).

- **Shown:** faction reach across the full continent, over the base geography.
  - **Cinder Ledger:** dense in the NW cluster (HQ Caradril) AND a **continental reach** — its true commercial heartland is the central river-cities (the Glassmere League); trade-web up the Verdance and down the Glasswater to the southern ports. Shade as a trade-web spanning NW→central→S.
  - **Concord Remnant:** seat at Caradril; scholar-traffic toward the Concord Heartlands (they covet the fallen surface capital) and the far Concord ruins (Cindern, Saltmere). Their continental ambition reaches well beyond the cluster.
  - **Mourners' Circle:** strongest in the NW (Vale/Coast) and present as a folk network across the settled south; thin on the steppe and in the volcanic SE.
  - **Ashen Wardens:** NW-cluster-bound (wandering Reach + Vale chapter); essentially absent on the far continent — a frontier order.
  - **Reachward Compact:** NW cluster only; no reach beyond.
  - **Gravecallers:** hidden cells in the NW worst-rite zones; rumored sympathizers in far fallen/drowned places (Saltmere, Sallow Marches) where the dead trouble folk too.
  - **Local far powers (placeholder):** the Glassmere League, Emberfell Theocracy, Wender clans, Karran warlords, Hollow Gulf ports — each dominant in its own region; sketch as region-owned, not campaign-faction-owned.
  - **Hollow Court (DM-only):** no surface territory anywhere; influence radiates only from the NW basin through cutouts. Show on Layer 2 only.
- **Labels:** faction names, "contested," "neutral," "region-power (placeholder)," clock-state markers.
- **Hidden:** Hollow Court reach; hidden agendas (public face only on any player-shown version).

## Layer 4 — Mystery / Revelation Map

**Audience:** DM only.

- **Shown:** mystery clue-sites (M1–M9+) over the base geography. **The overwhelming majority sit in the NW campaign cluster** (per the existing `WORLD_MAP_LAYERS.md` Layer 4) — the campaign's mysteries are local. The full-continent view adds only **distant corroboration sites** (DM-only, far-future): the Concord Heartlands (surface proof of the order's true span/sin — M6/M9 thematic echo), the Saltmere drowned towns and the Drowned Steps (pre-Concord/older-fall echoes that contextualize, never replace, the keystone).
- **Labels:** mystery codes; "primary clue-cluster (NW)," "distant corroboration (far-future)," "revelation gate," act-tier.
- **Hidden:** the answers; M7 (Hollow Court) location until late arc; the fact that far ruins do NOT contain the keystone.
- **Notes:** enforce the three-clue rule **within the NW cluster** — a player who never leaves the frontier can still reach every campaign revelation. Far sites are flavor and confirmation, never required.

## Layer 5 — Level-Tier Danger Map

**Audience:** DM (a softened "safe / rough / deadly" version may be shown).

- **Shown:** color-coded danger bands over the full continent.
  - **L1–4 (green):** the safe NW cluster core (Hollowmere, Reach roads, Vale, near-hubs).
  - **L5–8 (yellow):** deeper NW cluster (Greyfens deep, Sunder Heights, mid-Tollwood, Coast headlands, Caradril intrigue); the near Verdance Reaches.
  - **L9–12 (orange):** Caradril apex politics; **the Verdance Reaches and the Glassmere League** (Ring 2 / the wider settled continent); the Hethewald Holds; the Marrowdowns.
  - **L13–16 (red):** the far frontiers and fallen lands — the Concord Heartlands, the Emberfell Theocracy, the Saltmere Reaches, the Karran Marches, the Highmark Passes; the Concord Deep (subsurface NW); the Old Mast/Skerries deep.
  - **L17–20 (black):** the Under-Shrine / Drowned Keystone (beneath the NW basin).
  - **Beyond-campaign (grey/striped):** overseas (Surren, the Iron Skards), the open ocean lanes, the deep Wender Steppe — places the authored arc never requires.
- **Labels:** level bands; "telegraphed lethal" on gated sites; "beyond campaign" on overseas/striped zones.
- **Hidden:** the *reason* a zone is lethal (DM-only); on the player version, "safe / rough / deadly / unknown lands" only.
- **Notes:** the danger gradient mirrors the NW→SE axis but is **non-monotonic** — pockets of high danger (volcanic SE, fallen Heartlands) sit amid settled mid-tier country. The black endgame zone is **in the NW** (down, not far), and must always carry a visible warning.

## Layer 6 — Long-Distance Travel-Route Map

**Audience:** the player (route geometry is player-safe) + DM (danger annotations).

- **Shown:** all named long-distance routes from `FULL_WORLD_MAP_AUTHORITY.md` §7 plus the NW cluster's local roads/sea-route, with time and danger annotations: the Verdance Road, the Glasswater Run, the Greatspine Passes (Crown Road), the Salt Road, the Hethe Tollway, the South Sea Lanes, the Pale Coast Sea-Route (extended S), the Steppe Tracks.
- **Labels:** route names, rough leg-times (weeks at continental scale), risk level, key gateway points (Caradril = the cluster's gate to the continent; Glassmere = the interior hub).
- **Hidden:** DM-only routes — the node-network "arteries" the NW roads secretly follow (Layer 2), Gravecaller courier paths, smuggler/wrecker runs. Show those only if earned.
- **Notes:** **Caradril is the hinge** — every continental route from the cluster passes through or past it. Mark the Pale Coast Sea-Route as the fast water-way that continues south past the campaign area.

## Layer 7 — Late-Game Hidden Truth Map

**Audience:** DM only. **The deepest secret layer. Never render for the player.**

- **Shown:** the **true shape of the ancient world beneath the current one**, at continental scale. CRITICAL: this is **not** a continent-wide tunnel network — it is the **NW-cluster harvest-network (the Concord Deep)** with the **Hollowmere keystone** at its hub, shown as the buried machine it is, PLUS a continental **context layer**: the Concord's *surface* span (the fallen Heartlands, the far roads/ruins) shown as the order's visible empire, distinct from the hidden machine; pre-Concord things the network was built over (the Barrow of Nine Doors, the Old Mast) and pre-Concord echoes far off (the Drowned Steps, Saltmere drowned towns) marked as *older than the Concord*; the Under-Shrine / Drowned Keystone and the Hollow Court's dormant seat at the very bottom **beneath the NW basin**; the Quiet Country noted as the cosmological "drain" (off-map, non-spatial).
- **Labels:** "keystone (NW, vertical)," "node / relay (NW cluster)," "Concord surface span (fallen)," "pre-Concord (co-opted / echo)," "Quietfall sever-points," "Under-Shrine (endgame)."
- **Hidden:** this layer IS the hidden truth; exists only for DM consistency.
- **Notes:** the **"map beneath the map" is local and vertical.** Continental far-ruins explain how *big the Concord was on the surface*; they do not move the underground heart, which stays under Hollowmere. Do not let any rendered artifact of this layer leak into player-facing files or prompts.

## Layer 8 — Current Campaign Area Standalone Zoom Map

**Audience:** the player + DM (this standalone zoom is the day-to-day play map).

- **Shown:** a **zoomed-in view of the NW cluster** — the Sundering Reach (center) + Ring 1 (Vale S, Tollwood E, Coast W) + Caradril (SE corner) — at the detail of `WORLD_MAP_COORDINATES.md`. All 8 Reach settlements, all Ring 1 hubs/villages, the Greyfens, Sunder Heights, Hollowmere basin, the Mirewend/Ammet, the Pale Sea edge, the named roads and the Coast sea-route, and Caradril as a labeled city.
- **Labels:** everything on the campaign-area player-safe map (Prompt 3 in `WORLD_MAP_PROMPTS.md`).
- **Hidden:** subterranean anything, node-links, keystone truth, dungeon depths (identical secrecy to the campaign-area Layer 1).
- **Notes:** this is the **most-used map in actual play.** It is a **separate standalone zoom map (Prompt 5)** — NOT an inset embedded into the player-safe full-continent map (Prompt 1). It is governed by the existing `WORLD_MAP_LAYERS.md` Layer 1 / Prompt 3.

---

## Layer-to-Prompt Mapping

| Map prompt (in `FULL_WORLD_MAP_PROMPTS.md`) | Layers used |
|---|---|
| 1. Player-safe full-world/continent map | Layers 1–7 main-continent layers used as player-safe (Layer 1 + player-safe Layer 6 route styling + softened Layer 5 danger styling). **Layer 8 (standalone zoom) is NOT embedded into Prompt 1.** |
| 2. DM-only full-world/continent map | Layers 1+2+3+4+5+6+7+8 (full) |
| 3. Parchment full-world map (in-world artifact) | Layer 1 (player-safe; aged/incomplete styling) |
| 4. Clean functional AI/reference map | Layer 1 base + DM toggles for Layers 2–7 |
| 5. Current campaign area standalone zoom map | Layer 8 only (= campaign-area Layer 1 / Prompt 3); a **separate** map, not an inset on Prompt 1 |

> Note: "Layers 1–7 main-continent layers" means the seven continent-scale layers above; for the player-safe Prompt 1 only their player-safe content is rendered (Layers 2, 4, 7 are DM-only and must not appear; Layers 5 and 6 are used in their softened/player-safe form). Layer 8 is the campaign-area standalone zoom and is reserved for Prompt 5.

## Related Files

- [`FULL_WORLD_MAP_AUTHORITY.md`](FULL_WORLD_MAP_AUTHORITY.md) · [`FULL_WORLD_MAP_COORDINATES.md`](FULL_WORLD_MAP_COORDINATES.md) · [`FULL_WORLD_MAP_PROMPTS.md`](FULL_WORLD_MAP_PROMPTS.md)
- [`WORLD_MAP_LAYERS.md`](WORLD_MAP_LAYERS.md) (campaign-area layer authority)
- [`../11_mysteries_and_secrets/MYSTERY_WEB.md`](../11_mysteries_and_secrets/MYSTERY_WEB.md) · [`../11_mysteries_and_secrets/REVELATION_MAP.md`](../11_mysteries_and_secrets/REVELATION_MAP.md)
- [`../02_runtime_state/WORLD_CLOCKS.md`](../02_runtime_state/WORLD_CLOCKS.md)
- [`../03_canon/DM_ONLY_CANON.md`](../03_canon/DM_ONLY_CANON.md) (do not surface)
