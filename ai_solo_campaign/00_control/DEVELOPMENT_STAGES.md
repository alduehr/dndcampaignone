# DEVELOPMENT_STAGES.md

## Purpose

This file defines the staged development plan for the AI solo campaign project.

The campaign should not be built in one uncontrolled burst. It should grow through deliberate production stages, each with clear outputs, quality checks, indexes, and audits.

Core philosophy:

> Build the predetermined world first. Build the AI runtime alongside it. Audit constantly.

---

## Development Principles

### 1. Predetermined-First

The campaign should contain a large body of authored material before play begins.

The AI DM should not be expected to invent:
- Major regions
- Major cities
- Core factions
- Central mysteries
- Villains
- Cosmology
- Main campaign truths
- Level-tier arcs
- Major NPCs
- Major dungeons
- Legendary artifacts

The AI may improvise connective tissue, descriptions, dialogue, small NPCs, and local consequences, but the campaign should be rooted in authored canon.

### 2. Build In Layers

Every stage should strengthen one or more of these layers:

1. Campaign foundation
2. World atlas
3. Factions
4. NPCs
5. Quests and hooks
6. Mysteries and clues
7. Dungeons and locations
8. Encounters and adversaries
9. AI runtime and state tracking
10. Indexes and retrieval systems
11. Audits and continuity

### 3. Expand Outward From Playable Areas

Start with the campaign premise and first region. Then expand the first region deeply enough to run many sessions. Then expand major cities, neighboring regions, higher-level arcs, and distant mysteries.

### 4. Audit Before Scaling

Do not scale a broken foundation. After each major stage, audit for:
- Canon contradictions
- Exposed secrets
- Missing indexes
- Weak clue trails
- Passive factions
- Orphaned NPCs
- Quests with no consequences
- Solo-play balance problems
- Missing runtime state fields

### 5. Every Stage Must Leave The Repo More Runnable

A stage is not complete just because content exists. It is complete when the AI DM could retrieve and use that content during play.

---

# Stage 0 — Repository Setup

## Goal

Create the project shell, instruction files, folder structure, indexes, and initial templates.

## Outputs

Create the full repository structure:

```text
/ai_solo_campaign
  /00_control
  /01_runner_protocol
  /02_runtime_state
  /03_canon
  /04_world_atlas
  /05_regions
  /06_settlements
  /07_factions
  /08_npcs
  /09_quests
  /10_dungeons_and_ruins
  /11_mysteries_and_secrets
  /12_campaign_arc
  /13_encounters_and_bestiary
  /14_treasure_and_artifacts
  /15_random_tables
  /16_ai_session_packs
  /17_generation_backlog
  /18_audits
```

Create initial control files:

- `MANIFEST.md`
- `PROJECT_RULES.md`
- `PRODUCTION_WORKFLOW.md`
- `DEVELOPMENT_STAGES.md`
- `TRACKING_SYSTEM.md`
- `PROGRESS_LOG.md`
- `TODO.md`
- `OPEN_QUESTIONS.md`
- `CONSISTENCY_AUDIT.md`
- `CONTENT_INDEX.md`
- `TAG_INDEX.md`
- `RETRIEVAL_GUIDE.md`

## Completion Criteria

Stage 0 is complete when:
- The folder structure exists.
- Core control files exist.
- Index placeholders exist.
- Runtime state placeholders exist.
- Canon files exist.
- The repo has clear rules for how future content should be created.

---

# Stage 1 — Campaign Foundation

## Goal

Create the core identity of the campaign.

This stage answers:

- What is this campaign about?
- What makes the world distinctive?
- What is the central long-term conflict?
- What is the hidden truth?
- Why does the campaign begin at level 1?
- What could eventually take the player to level 20?

## Required Outputs

Create or update:

- `/00_control/MANIFEST.md`
- `/03_canon/CANON.md`
- `/03_canon/PLAYER_SAFE_CANON.md`
- `/03_canon/DM_ONLY_CANON.md`
- `/04_world_atlas/WORLD_OVERVIEW.md`
- `/04_world_atlas/MAP_DESCRIPTION.md`
- `/12_campaign_arc/MAIN_ARC_OVERVIEW.md`
- `/12_campaign_arc/LEVEL_1_TO_20_PROGRESSION.md`
- `/11_mysteries_and_secrets/MYSTERY_WEB.md`
- `/11_mysteries_and_secrets/REVELATION_MAP.md`

## Required Content

Stage 1 must establish:

- Original campaign premise
- Tone and themes
- Central long-term conflict
- Hidden truth behind the conflict
- Initial world map concept
- Level 1–20 escalation model
- Starting region
- Starting settlement
- 5–8 major factions
- 20 major NPCs
- 20 major secrets
- 10 campaign clocks or escalating threats
- Initial level 1 situation
- Three opening scenes
- One recommended default opening scene
- Solo-friendly starting safety mechanism
- First 10 session-sized hooks
- First 20 rumors

## Completion Criteria

Stage 1 is complete when:
- The campaign can be summarized in one page.
- The AI DM knows the true hidden premise.
- The player-facing premise is spoiler-safe.
- The starting location is defined.
- The first session can begin.
- The main arc has a rough level 1–20 shape.
- All foundational content is indexed.

---

# Stage 2 — AI Runtime Foundation

## Goal

Create the system that lets an AI DM run the campaign over many sessions.

## Required Outputs

Create or update:

- `/01_runner_protocol/AI_DM_CORE_RULES.md`
- `/01_runner_protocol/SOLO_PLAY_PRINCIPLES.md`
- `/01_runner_protocol/SESSION_LOOP.md`
- `/01_runner_protocol/SCENE_FRAMING.md`
- `/01_runner_protocol/PLAYER_CHOICE_PROTOCOL.md`
- `/01_runner_protocol/ROLL_AND_CHECK_PROTOCOL.md`
- `/01_runner_protocol/COMBAT_PROTOCOL.md`
- `/01_runner_protocol/SOCIAL_SCENE_PROTOCOL.md`
- `/01_runner_protocol/EXPLORATION_PROTOCOL.md`
- `/01_runner_protocol/TRAVEL_PROTOCOL.md`
- `/01_runner_protocol/CLUE_DELIVERY_PROTOCOL.md`
- `/01_runner_protocol/SECRET_REVEAL_PROTOCOL.md`
- `/01_runner_protocol/FAILURE_AND_CONSEQUENCES.md`
- `/16_ai_session_packs/START_NEW_CAMPAIGN_PROMPT.md`
- `/16_ai_session_packs/RESUME_CAMPAIGN_PROMPT.md`
- `/16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md`
- `/16_ai_session_packs/STATE_UPDATE_TEMPLATE.md`
- `/16_ai_session_packs/COMPACT_CONTEXT_TEMPLATE.md`

## Runtime State Files

Create or update:

- `/02_runtime_state/CURRENT_STATE.md`
- `/02_runtime_state/PLAYER_CHARACTER.md`
- `/02_runtime_state/CURRENT_LOCATION.md`
- `/02_runtime_state/CURRENT_SCENE.md`
- `/02_runtime_state/ACTIVE_QUESTS.md`
- `/02_runtime_state/OPEN_THREADS.md`
- `/02_runtime_state/KNOWN_CLUES.md`
- `/02_runtime_state/HIDDEN_CLUES.md`
- `/02_runtime_state/NPC_MEMORY.md`
- `/02_runtime_state/FACTION_STATE.md`
- `/02_runtime_state/WORLD_CLOCKS.md`
- `/02_runtime_state/INVENTORY_AND_REWARDS.md`
- `/02_runtime_state/RELATIONSHIPS.md`
- `/02_runtime_state/CONSEQUENCES.md`
- `/02_runtime_state/SESSION_RECAP.md`
- `/02_runtime_state/NEXT_SESSION_START.md`

## Completion Criteria

Stage 2 is complete when:
- A future AI DM knows how to start a session.
- A future AI DM knows how to end a session.
- State files clearly show what must be tracked.
- The distinction between static canon and runtime state is clear.
- The AI knows when to improvise and when not to.
- Solo-play combat, social, travel, exploration, and clue delivery have protocols.

---

# Stage 3 — Starting Region Deep Build

## Goal

Expand the starting region enough to support many sessions of open-world play.

## Required Outputs

Create or update:

- `/05_regions/[starting-region].md`
- `/06_settlements/[starting-settlement].md`
- Additional settlement files
- Wilderness location files
- Local dungeon/ruin files
- Regional quest files
- Regional NPC entries
- Regional faction activity
- Regional rumors
- Regional encounter tables
- Regional mystery chains

## Content Targets

- 8–12 settlements
- 20–30 wilderness locations
- 5–8 dungeons or ruins
- 50–75 NPCs
- 30–50 hooks
- 10–15 developed quests
- 5 mystery chains
- 5 faction clocks
- Regional encounter tables
- Regional rumor tables

## Completion Criteria

Stage 3 is complete when:
- The starting region can support at least 10–20 sessions.
- The player can travel in multiple directions.
- The region contains meaningful choices.
- Factions in the region act even if ignored.
- Mysteries have clue paths.
- There are enough local NPCs that the AI does not need to invent many important people.
- The region is indexed and cross-linked.

---

# Stage 4 — First Major City Deep Build

## Goal

Create the first major city as a dense hub for politics, intrigue, services, quests, factions, secrets, and recurring NPCs.

## Required Outputs

Create or update:

- City overview file
- District files
- Government/political structure
- Law and crime notes
- Shops and services
- Guilds, temples, noble houses, criminal groups
- City NPCs
- City quest index
- City rumor table
- City faction clocks
- City secrets
- City encounter/social scene tables

## Content Targets

- 6–10 districts
- 75–100 NPCs
- 30–50 hooks or rumors
- 10–20 developed quests
- 5–10 faction conflicts
- 5–10 city secrets
- 3–5 mystery chains
- 3–5 recurring rival/ally characters

## Completion Criteria

Stage 4 is complete when:
- The city can serve as a long-term campaign hub.
- The city feels politically alive.
- Major services exist.
- There are enough NPCs and factions for repeated visits.
- The city changes when ignored.
- The city is indexed and cross-linked.

---

# Stage 5 — Level 1–4 Play Arc

## Goal

Fully develop the early campaign arc while preserving open-world freedom.

## Required Outputs

Create or update:

- `/12_campaign_arc/ACT_1_LEVELS_1_4.md`
- Early main quests
- Early side quests
- Early faction decision points
- First major dungeon
- First major mystery chain
- Early villain or threat profile
- Early reward and leveling guidance
- Failure and alternate path notes

## Content Requirements

The level 1–4 arc should include:
- A default path
- Several alternate paths
- Early clues to the main arc
- Local stakes
- Personal stakes
- Faction hooks
- At least one significant dungeon/ruin
- At least one social/political conflict
- At least one mystery
- At least one recurring adversary
- Clear level-up guidance
- State update triggers

## Completion Criteria

Stage 5 is complete when:
- A solo campaign can begin and run through level 4.
- The player has real agency.
- The main arc is foreshadowed but not overexplained.
- The first major villain/threat is established.
- Failure states are playable.
- The AI DM has enough guidance to run sessions.

---

# Stage 6 — First Full Audit

## Goal

Evaluate whether the foundation is strong enough to scale.

## Required Outputs

Create:

- `/18_audits/STAGE_1_TO_5_AI_READINESS_AUDIT.md`

Update:

- `/00_control/CONSISTENCY_AUDIT.md`
- `/00_control/TODO.md`
- `/17_generation_backlog/CONTENT_GAPS.md`

## Audit Scope

Check:
- Canon consistency
- Secret separation
- Retrieval quality
- NPC connectivity
- Quest usability
- Mystery solvability
- Faction agency
- Solo-play safety
- State tracking
- Index completeness
- Main arc coherence
- Open-world resilience

## Completion Criteria

Stage 6 is complete when:
- Critical issues are identified.
- High-priority gaps are documented.
- The TODO list is reorganized.
- No major scaling continues until critical issues are fixed.

---

# Stage 7 — Regional Expansion Ring 1

## Goal

Build regions adjacent to the starting area so the world opens outward.

## Required Outputs

For each adjacent region:
- Region overview
- Map relation
- Settlements
- Factions present
- NPCs
- Quests
- Dungeons/ruins
- Secrets
- Encounter tables
- Travel events
- Clocks and consequences

## Content Targets Per Region

- 1 major settlement or 2–3 towns
- 5–10 villages or small sites
- 10–20 wilderness locations
- 3–6 dungeons/ruins
- 30–60 NPCs
- 20–40 hooks
- 8–15 developed quests
- 3–5 secrets or mystery chains
- 2–5 faction clocks

## Completion Criteria

Stage 7 is complete when:
- The player can leave the starting region in multiple directions.
- Nearby regions have enough authored content for extended play.
- Travel between regions is meaningful.
- Adjacent regions connect to the main arc and local arcs.

---

# Stage 8 — Faction Deepening

## Goal

Make the major factions fully operational.

## Required Outputs

For each major faction:
- Full faction file
- Leader and key members
- Methods and resources
- Internal conflict
- Relationship map
- Faction clock
- Quest chain
- Secrets
- How they react to the player
- What they do if ignored

## Completion Criteria

Stage 8 is complete when:
- Every major faction has agency.
- Every major faction has a clock.
- Every major faction has NPCs.
- Every major faction has quests.
- Every major faction can help, hinder, recruit, deceive, or retaliate against the player.

---

# Stage 9 — NPC Codex Expansion

## Goal

Build enough predetermined NPCs to reduce major improvisation during play.

## Required Outputs

Expand:
- `NPC_INDEX.md`
- `MAJOR_NPCS.md`
- `SECONDARY_NPCS.md`
- `MINOR_NPCS.md`
- `NPC_RELATIONSHIP_WEB.md`
- `NPC_SECRET_LEDGER.md`
- `NPC_VOICE_GUIDE.md`

## Content Targets

- 50–100 major NPCs
- 200–500 secondary NPCs
- 500+ minor named NPCs

This can happen over multiple passes.

## Completion Criteria

Stage 9 is complete when:
- Major settlements have robust NPC populations.
- Factions have named members at multiple levels.
- Quest-givers, rivals, patrons, witnesses, shopkeepers, priests, criminals, guards, sages, and local leaders exist.
- NPCs have relationships and secrets.
- The AI DM rarely needs to invent recurring characters.

---

# Stage 10 — Quest Library Expansion

## Goal

Build a huge authored quest and hook library.

## Required Outputs

Expand:
- Main campaign quests
- Regional quests
- Faction quests
- Personal quests
- Dungeon quests
- Random hooks
- Rumors
- Bounties
- Complications
- Travel events

## Content Targets

- 25–40 major campaign quests
- 75–150 developed quests
- 300–600 hooks/rumors/jobs/events

## Completion Criteria

Stage 10 is complete when:
- Every major region has multiple quest sources.
- Every major faction has quest chains.
- Every major settlement has local hooks.
- Quests have consequences and failure states.
- Quests are indexed by level, region, faction, and type.

---

# Stage 11 — Mystery, Secret, and Clue Expansion

## Goal

Make the campaign mystery-rich and fair.

## Required Outputs

Expand:
- `SECRET_INDEX.md`
- `CLUE_INDEX.md`
- `MYSTERY_CHAINS.md`
- `MYSTERY_WEB.md`
- `REVELATION_MAP.md`
- `FALSE_LEADS.md`
- `PROPHECIES_AND_OMENS.md`
- `REVEAL_TIMING.md`

## Completion Criteria

Stage 11 is complete when:
- Major mysteries have multiple clue paths.
- Secrets are indexed.
- Clues have locations and sources.
- False leads are fair.
- The AI DM knows what not to reveal.
- Discovery changes the world.

---

# Stage 12 — Dungeons, Ruins, and Adventure Sites

## Goal

Create a large library of explorable places.

## Required Outputs

For each major dungeon/ruin:
- Purpose in the world
- History
- Entrance
- Occupants
- Room/zone list
- Hazards
- Secrets
- Clues
- Puzzles
- Treasure
- Boss/climax
- Noncombat options
- Solo safety valves
- Consequences if ignored
- State update triggers

## Completion Criteria

Stage 12 is complete when:
- Regions contain meaningful adventure sites.
- Dungeons connect to quests, factions, and mysteries.
- Dungeons are not just combat gauntlets.
- Solo play is supported.
- Important dungeon clues are indexed.

---

# Stage 13 — Encounter and Bestiary Expansion

## Goal

Create solo-friendly threats and adversaries.

## Required Outputs

Expand:
- `MONSTER_INDEX.md`
- `ADVERSARY_GROUPS.md`
- `RECURRING_VILLAINS.md`
- `RANDOM_ENCOUNTERS.md`
- `NONCOMBAT_OBSTACLES.md`
- `BOSS_DESIGN.md`

## Completion Criteria

Stage 13 is complete when:
- Regions have encounter tables.
- Factions have adversary groups.
- Bosses have weaknesses and foreshadowing.
- Combat does not assume four PCs.
- Noncombat obstacles are common.
- Retreat and preparation are supported.

---

# Stage 14 — Treasure, Artifacts, and Rewards

## Goal

Create rewards that support solo play and campaign progression.

## Required Outputs

Expand:
- `TREASURE_INDEX.md`
- `ARTIFACTS.md`
- `MAGIC_ITEMS.md`
- `REWARDS_BY_LEVEL.md`

## Completion Criteria

Stage 14 is complete when:
- Rewards are level-appropriate.
- Solo survivability is supported without removing danger.
- Artifacts connect to lore and mysteries.
- Treasure supports choices, not just power.

---

# Stage 15 — Level 5–20 Arc Expansion

## Goal

Develop the remaining campaign acts.

## Required Outputs

Fully expand:
- `ACT_2_LEVELS_5_8.md`
- `ACT_3_LEVELS_9_12.md`
- `ACT_4_LEVELS_13_16.md`
- `ACT_5_LEVELS_17_20.md`
- `VILLAIN_ESCALATION.md`
- `ENDGAME_STATES.md`

## Completion Criteria

Stage 15 is complete when:
- The campaign can support progression to level 20.
- Each tier has multiple paths.
- Major revelations are staged.
- Villains escalate.
- Regional and faction arcs connect to the main conflict.
- Endgame outcomes depend on player choices.

---

# Stage 16 — Pre-Play Readiness Audit

## Goal

Determine whether the campaign is ready to start actual solo play.

## Required Outputs

Create:

- `/18_audits/PRE_PLAY_READINESS_AUDIT.md`

## Completion Criteria

The campaign is ready for play when:
- The first 10–20 sessions have enough prepared material.
- The AI DM can start cleanly.
- State files are ready.
- The opening scene is ready.
- Critical secrets are protected.
- Starting region is deep enough.
- Starting NPCs and factions are ready.
- The first mystery has multiple clue paths.
- The first level-up path is clear.
- There are no critical audit issues.

---

# Stage 17 — Live Campaign Operation

## Goal

Run the campaign while preserving state and canon.

## During Play

After every session:
- Update runtime state.
- Update NPC memory.
- Update known clues.
- Update active quests.
- Update faction clocks.
- Update consequences.
- Update next-session start.
- Add important improvisation to canon/indexes.
- Log the session.

## Completion Criteria

This stage continues until the campaign ends.

---

# Stage 18 — Periodic Live Audits

## Goal

Prevent long-running campaign drift.

## Suggested Cadence

Run a live audit:
- Every 3–5 sessions
- After each level-up
- After major revelations
- After major faction changes
- Before entering a new region
- Before beginning a new campaign act

## Completion Criteria

A live audit is complete when:
- State is coherent.
- Open threads are clear.
- Forgotten consequences are restored.
- NPC memories are current.
- Faction clocks are current.
- Next-session handoff is usable.

---

# Stage 19 — Campaign Completion and Epilogues

## Goal

Conclude the campaign in a way that reflects accumulated choices.

## Required Outputs

- Endgame state resolution
- Faction outcome summary
- NPC fate summary
- Mystery resolution summary
- Player character epilogue
- World state after campaign
- Unresolved threads list
- Optional sequel hooks

## Completion Criteria

The campaign is complete when:
- The central conflict is resolved or transformed.
- Major faction outcomes are determined.
- Major NPC arcs have conclusions.
- The player’s choices visibly shaped the world.
- The final state is documented.

---

# Recommended Development Rhythm

Use this loop:

```text
Plan → Generate → Index → Canon Update → State Update → Audit → Fix → Expand
```

Do not skip indexing.

Do not skip canon updates.

Do not skip audits.

Do not scale broken content.
