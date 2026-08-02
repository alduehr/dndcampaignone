# Orrun — World Reference (Non-Campaign)

## What This Folder Is

`/Orrun` is a **world-level reference library**, sibling to `/ai_solo_campaign`, not part of it. It exists so the setting of Vael/Orrun can be used independently of "The Long Remembering" (the predetermined solo campaign in `/ai_solo_campaign`) — for one-shots, other campaigns, NPC walk-ons, or just general reference to the world's geography, cities, and everyday dangers.

**Everything in this folder is spoiler-free with respect to the campaign's central mystery.** It contains no hidden-truth material, no faction hidden agendas, no campaign quest hooks, and no DM-only campaign secrets — and it deliberately does not name or hint at what any of them are. It is safe to read, share, or hand to a player of "The Long Remembering" without spoiling anything.

## Relationship To `/ai_solo_campaign`

| | `/ai_solo_campaign` | `/Orrun` |
|---|---|---|
| Purpose | Runs one specific predetermined campaign | General-purpose world reference |
| Canon authority | **Authoritative** for anything campaign-related | Derived from campaign canon, curated for reuse |
| Secrets | Contains DM-only campaign truths | Contains none — public/general knowledge only |
| Contents | Regions, settlements, NPCs, quests, factions, mysteries, dungeons — all wired into the main arc | Geography, cities, generic wandering encounters, culture, and the world's alternate-timeline cosmology |
| Who uses it | The AI DM running the campaign | Anyone running anything else in this world |

If `/ai_solo_campaign` and `/Orrun` ever disagree on a plain geography or culture fact, `/ai_solo_campaign` wins — `/Orrun` is a curated extract, not a second source of truth. Do not add campaign-specific plot content here. If you need campaign material, it belongs in `/ai_solo_campaign` instead.

## Folder Structure

```text
/Orrun
  /00_overview       — world summary, gazetteer index, audits
  /01_geography       — continent, regions, travel routes
    /regions          — 16 region files
    /wilderness        — 7 wilderness zones: terrain, hazards, fauna, resources
  /02_settlements      — cities, towns, and villages (public-facing)
  /03_culture         — calendar, gods and faiths, languages, general history
  /04_bestiary        — generic wandering monsters and hazards, by terrain
  /05_timelines        — the Unmade: alternate-timeline cosmology, including the Last Telling
  /06_sites          — 34 ruins and adventure sites as physical places
```

## The Timelines Folder

`/05_timelines` is new world lore, not previously part of the setting: **the Unmade**, the cosmological fact that Vael's history is one "Telling" among countless unrealized ones. It defines a costly, dangerous, but learnable ritual (**the Rite of the Broken Threshold**) that lets a determined traveler — from anywhere in the world, with no fixed shrine required — cross into a neighboring Telling, up to and including **the Last Telling**, the worst one anybody has confirmed exists. Getting there is expensive and risky by design. Getting back is easier, but never free.

This is genuinely new setting content and has been registered in `ai_solo_campaign/00_control/NAMING_REGISTRY.md` per project rules, since future campaign or one-shot content may reference it.

## Maintenance

- This folder is **not** covered by `SESSION_END_UPDATE_CHECKLIST.md` or the campaign's runtime state — nothing here changes during play of "The Long Remembering."
- When campaign canon changes in a way that affects public-facing geography/culture, update the corresponding `/Orrun` file too, but only with information that is genuinely public/spoiler-free.
- New settlements, regions, or generic bestiary entries created for other purposes (one-shots, future campaigns) should go here, not in `/ai_solo_campaign`.
