# Orrun (Vael) — World Reference (Non-Campaign)

## What This Folder Is

`/locations/vael/orrun` is a **world-level reference library**, sibling to `/ai_solo_campaign`, not part of it. It exists so the setting of Vael/Orrun can be used independently of "The Long Remembering" (the predetermined solo campaign in `/ai_solo_campaign`) — for one-shots, other campaigns, NPC walk-ons, or just general reference to the world's geography, cities, and everyday dangers. It also has a second, newer role: the DungeonMaster app onboards locations and campaigns as separate units, and mounts this folder into a campaign's namespace as `vael-orrun` (see `dm.location.json` below).

**Everything in this folder is spoiler-free with respect to the campaign's central mystery.** It contains no hidden-truth material, no faction hidden agendas, no campaign quest hooks, and no DM-only campaign secrets — and it deliberately does not name or hint at what any of them are. It is safe to read, share, or hand to a player of "The Long Remembering" without spoiling anything.

## Canonical Keys

Every place in this folder is addressed by a **canonical key**, not a file path: `<world>/<continent>/<kind>/<slug>`. World is `vael`, continent is `orrun`. For example, Ashgarden Vale is `vael/orrun/regions/ashgarden-vale`, at `locations/vael/orrun/regions/ashgarden-vale.md`. Campaign files in `/ai_solo_campaign` cite these keys directly (in backticks) rather than linking to a path — a `location_ref:` front-matter field marks which key a campaign file overlays. Every file in this folder that represents an addressable place carries a matching `location_key:` front-matter field equal to its own key.

Not every file is a place. Index files (`GAZETTEER_INDEX.md`, `sites/site-index.md`, and the five `*-settlements.md`/`*-sites.md` group indexes left behind when a grouped file was split into individual places) and the top-level overview docs (`README.md`, `CONTINENT.md`, `AUDIT_2026-08-01.md`) carry no `location_key` — they're reference material about places, not places themselves.

## Relationship To `/ai_solo_campaign`

| | `/ai_solo_campaign` | `/locations/vael/orrun` |
|---|---|---|
| Purpose | Runs one specific predetermined campaign | General-purpose world reference |
| Canon authority | **Authoritative** for anything campaign-related | Derived from campaign canon, curated for reuse |
| Secrets | Contains DM-only campaign truths | Contains none — public/general knowledge only |
| Contents | Regions, settlements, NPCs, quests, factions, mysteries, dungeons — all wired into the main arc | Geography, cities, generic wandering encounters, culture, and the world's alternate-timeline cosmology |
| Who uses it | The AI DM running the campaign | Anyone running anything else in this world |
| Addressed by | File paths (its own internal cross-links) | Canonical keys (`vael/orrun/<kind>/<slug>`) |

If `/ai_solo_campaign` and `/locations/vael/orrun` ever disagree on a plain geography or culture fact, `/ai_solo_campaign` wins — `/locations/vael/orrun` is a curated extract, not a second source of truth. Do not add campaign-specific plot content here. If you need campaign material, it belongs in `/ai_solo_campaign` instead.

## Folder Structure

```text
/locations/vael/orrun
  README.md          — this file
  CONTINENT.md         — Orrun at a glance (no location_key; overview, not a place)
  GAZETTEER_INDEX.md    — full file index by category (no location_key)
  AUDIT_2026-08-01.md    — cohesion + secrecy audit (no location_key)
  dm.location.json      — DungeonMaster app location-manifest contract
  /regions            — 16 region files, one per place
  /wilderness          — 7 wilderness zones: terrain, hazards, fauna, resources
  /settlements         — 44 individual settlements/cities, one file per place, plus 5 group indexes
                          (sundering-reach-settlements.md, ashgarden-vale-settlements.md,
                          tollwood-settlements.md, pale-coast-settlements.md, far-continent-anchors.md —
                          none of these five carry a location_key; they're regional indexes with links
                          out to the individual place files, kept for the shared regional-character prose)
  /sites             — 34 individual ruins/adventure sites, one file per place, plus 4 group indexes
                          and site-index.md (the master index; none of these five carry a location_key)
  /culture            — calendar, gods and faiths, languages, general history
  /bestiary            — generic wandering monsters and hazards, by terrain
  /timelines           — the Unmade: alternate-timeline cosmology, including the Last Telling
  /travel             — travel rates, routes, and hazards across the continent
  /maps              — mirrored map manifest + image assets (see "Maps" below)
```

## Maps

`/locations/vael/orrun/maps` holds `manifest.json` + `assets/` — the **authoritative** map catalog (previously mirrored from `/ai_solo_campaign/maps`; that campaign-side copy has been removed, since the two were always byte-identical and keeping one location is simpler). Each manifest entry's `region` field is a canonical key (e.g. `vael/orrun/regions/ashgarden-vale`), not a bare slug. `dm.campaign.json`'s `contentRoot` still points at `ai_solo_campaign` for the campaign's own content; the maps now live with the rest of this location library instead.

Three manifest entries don't resolve to a specific place file, by design (a map can exist before or without a dedicated location page, and vice versa): `orrun-full-continent` and `cluster-northwest-orrun` resolve to the bare continent key `vael/orrun` (there is no single-region file for "the whole continent" or "the NW cluster"); `region-highmark-passes` resolves to `vael/orrun/regions/highmark-passes`, which has no file yet — the Highmark Passes are documented only within `CONTINENT.md` and `travel/travel-and-routes.md` as uninhabited barrier country.

## Canonical Key Examples

- A region: `vael/orrun/regions/tollwood` → `regions/tollwood.md`
- A settlement: `vael/orrun/settlements/hollowmere` → `settlements/hollowmere.md`
- A city (stays one file regardless of internal districts): `vael/orrun/settlements/caradril` → `settlements/caradril.md`
- A site: `vael/orrun/sites/peat-chapel` → `sites/peat-chapel.md` (a leading "The" and any parenthetical are dropped when a display name is turned into a slug)
- A wilderness zone: `vael/orrun/wilderness/greyfens` → `wilderness/greyfens.md`

## The Timelines Folder

`/timelines` is new world lore, not previously part of the setting: **the Unmade**, the cosmological fact that Vael's history is one "Telling" among countless unrealized ones. It defines a costly, dangerous, but learnable ritual (**the Rite of the Broken Threshold**) that lets a determined traveler — from anywhere in the world, with no fixed shrine required — cross into a neighboring Telling, up to and including **the Last Telling**, the worst one anybody has confirmed exists. Getting there is expensive and risky by design. Getting back is easier, but never free.

This is genuinely new setting content and has been registered in `ai_solo_campaign/00_control/NAMING_REGISTRY.md` per project rules, since future campaign or one-shot content may reference it.

## DungeonMaster App Onboarding

`dm.location.json` (in this folder) is the location-manifest contract the DungeonMaster app reads to onboard this folder as a standalone, mountable location unit, independent of any one campaign. `dm.campaign.json` (repo root) lists this location under a top-level `locations` key, giving it a `mountPath` of `locations/vael/orrun` — that mount is how "The Long Remembering" pulls this library into its own namespace at runtime, without the two being the same content tree. `world`/`continent` in `dm.location.json` are descriptive only; resolution happens by mount path, not by folder name, on purpose — that's part of what keeps this folder reusable by other campaigns.

## Maintenance

- This folder is **not** covered by `SESSION_END_UPDATE_CHECKLIST.md` or the campaign's runtime state — nothing here changes during play of "The Long Remembering."
- When campaign canon changes in a way that affects public-facing geography/culture, update the corresponding `/locations/vael/orrun` file too, but only with information that is genuinely public/spoiler-free.
- New settlements, regions, or generic bestiary entries created for other purposes (one-shots, future campaigns) should go here, not in `/ai_solo_campaign`.
- Every new place file needs a `location_key:` front-matter field equal to its own canonical key. Every campaign file that overlays a place needs a matching `location_ref:` field.
