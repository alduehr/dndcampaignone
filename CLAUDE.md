# CLAUDE.md

## Prime Directive

This project is a large, predetermined, AI-run solo D&D campaign.

**Predetermined-first, improvisation-second.**

The goal is to build a deeply authored original campaign world that an AI DM can run for one player over many sessions. The AI DM should rely on prepared world material wherever possible and improvise only as much as a skilled human DM would at the table.

The project must support play from level 1 to level 20.

---

## Non-Negotiable Rules

- Preserve established canon.
- Separate player-facing information from DM-only information.
- Use existing authored content before inventing new major content.
- Record important improvisation into canon, state, or indexes.
- Design for one player character, not a standard four-person party.
- Avoid railroading.
- Let factions act even when the player ignores them.
- Make mysteries solvable through multiple clue paths.
- Do not reveal hidden truths until discovered.
- Do not create generic filler just to hit a quota.
- Update indexes after adding or materially changing content.
- Update state files when campaign state changes.
- Do not ask endless clarifying questions; make strong creative decisions and document them.
- Follow the canon authority hierarchy in CANON_AUTHORITY.md when files disagree.
- Follow GENERATION_GUARDRAILS.md before creating major new content.
- Check NAMING_REGISTRY.md before creating major NPCs, factions, regions, settlements, gods, artifacts, ancient orders, or specialized setting terms.
- Follow RULESET_ASSUMPTIONS.md for D&D 5e / 2024-compatible mechanics.

---

## Hard Constraints

- The campaign world must be original.
- Do not use copyrighted D&D settings, characters, factions, gods, cities, or lore from Forgotten Realms, Eberron, Greyhawk, Dragonlance, Critical Role, etc.
- D&D 5e / 2024 compatibility is allowed, but keep custom mechanics lightweight and adaptable.
- Do not overwrite established canon without documenting the revision.
- Do not create lore that has no play function.
- Do not design content that assumes a four-character party unless explicitly marked as dangerous.

---

## Core Project Files To Read First

For most significant work, read these first:

@ai_solo_campaign/00_control/PROJECT_RULES.md
@ai_solo_campaign/00_control/CANON_AUTHORITY.md
@ai_solo_campaign/00_control/GENERATION_GUARDRAILS.md
@ai_solo_campaign/00_control/PRODUCTION_WORKFLOW.md
@ai_solo_campaign/00_control/CONTENT_STANDARDS.md

For all campaign content, always preserve D&D 5e / 2024-compatible mechanical usability. This project must not drift into a generic fantasy RPG, rules-light system, or mechanics-free story setting.  To maintain these requirements, read:

@ai_solo_campaign/00_control/DND_MECHANICS_REQUIREMENTS.md

For canon, naming, ruleset assumptions, and drift prevention, read these before creating or revising major campaign content:

@ai_solo_campaign/00_control/NAMING_REGISTRY.md
@ai_solo_campaign/00_control/RULESET_ASSUMPTIONS.md

For AI DM runtime or session-running work, also read:

@ai_solo_campaign/01_runner_protocol/AI_DM_CORE_RULES.md
@ai_solo_campaign/16_ai_session_packs/SESSION_END_UPDATE_CHECKLIST.md
@ai_solo_campaign/00_control/DEVELOPMENT_STAGES.md
@ai_solo_campaign/00_control/TRACKING_SYSTEM.md

---

## Specialist Instructions

Load only the relevant specialist file when doing focused work.

For world, regions, maps, settlements, and travel:

@ai_solo_campaign/00_control/WORLDBUILDING_STANDARDS.md

For factions, politics, guilds, cults, churches, noble houses, criminal groups, armies, and faction clocks:

@ai_solo_campaign/00_control/FACTION_STANDARDS.md

For NPCs:

@ai_solo_campaign/00_control/NPC_STANDARDS.md

For quests, hooks, rumors, arcs, failure states, and consequences:

@ai_solo_campaign/00_control/QUEST_STANDARDS.md

For mysteries, secrets, clues, revelations, puzzles, false leads, and prophecy:

@ai_solo_campaign/00_control/MYSTERY_STANDARDS.md

For audits, continuity checks, AI-readiness reviews, and gap reports:

@ai_solo_campaign/00_control/AUDIT_STANDARDS.md

---

## Specialist Agents

All specialist agents are defined in `.claude/agents/` and are tracked in version control. Use them for focused production passes.

| Agent | Purpose |
|---|---|
| `campaign-architect` | Overall structure, roadmap, level 1–20 arc, content quotas |
| `ai-dm-runtime-engineer` | Runtime rules, session loop, state files, solo-play protocols |
| `canon-continuity-auditor` | Audits, contradictions, secret exposure, AI-readiness |
| `world-atlas-builder` | Regions, settlements, maps, travel, wilderness |
| `faction-weaver` | Factions, guilds, cults, clocks, political groups |
| `npc-codex-builder` | NPCs, relationships, voice, secrets, memory |
| `quest-arc-designer` | Quests, hooks, rumors, arcs, failure states |
| `mystery-clue-engineer` | Mysteries, clues, secrets, revelations, false leads |
| `encounter-bestiary-designer` | Encounters, monsters, bosses, treasure logic |
| `indexer-librarian` | Indexes, tags, cross-links, retrieval guides |
| `player-experience-reviewer` | Player-perspective review, pacing, agency, fairness |

Do not add local Claude Code session files (e.g. `settings.local.json`, `projects/`) to version control. Only `.claude/agents/` is tracked.

---

## Repository Shape

Use this structure unless the user explicitly changes it:

```text
/.claude
  /agents              — Specialist agent definitions (tracked)
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

---

## Required Work Pattern

For any major production pass:

1. Read relevant control and canon files.
2. Identify current project state.
3. Make a concise plan.
4. Create or edit files.
5. Cross-link related material.
6. Update indexes.
7. Update canon/state files if new facts were created.
8. Update progress log.
9. Update TODO or content gaps.
10. Run a small consistency check.
11. Summarize what changed and what should happen next.

Do not do long exploratory loops without producing useful content.

Before creating new major content, check:

* `CANON_AUTHORITY.md` for source-of-truth rules.
* `GENERATION_GUARDRAILS.md` for drift prevention.
* `NAMING_REGISTRY.md` for duplicate or conflicting names.
* `RULESET_ASSUMPTIONS.md` for D&D mechanical assumptions.

---

## Output Expectations

When completing a task, report:

- Files created or changed
- Major canon established
- Indexes updated
- State files updated, if any
- What remains incomplete
- Recommended next production pass

Do not claim a file was updated unless it actually was.
