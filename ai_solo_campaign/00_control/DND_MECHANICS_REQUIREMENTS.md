# DND_MECHANICS_REQUIREMENTS.md

## Purpose

This project is an AI-run solo campaign for D&D 5e / 2024-compatible play.

The campaign must not become a generic fantasy RPG, rules-light storygame, or custom system unless the user explicitly requests that later.

The world can be original, but the gameplay assumptions should remain D&D-compatible.

---

## Core Requirement

All campaign content must be usable for D&D 5e / 2024-compatible play.

This means the campaign must support:

* Character levels 1–20
* Classes and subclasses
* Ability checks
* Saving throws
* Armor Class
* Hit points
* Initiative
* Conditions
* Spellcasting
* Proficiency bonus assumptions
* Skill checks
* Combat rounds when needed
* Challenge scaling for one player character
* Magic items and treasure by level
* Resting assumptions
* Encounter danger assessment
* NPC and monster stat references

---

## Do Not Create A New RPG System

Do not invent a replacement rules system.

Do not replace D&D mechanics with:

* Custom narrative resolution systems
* Pure story tags
* Generic “threat levels” only
* Homebrew dice mechanics
* Non-D&D classes
* Non-D&D spell systems
* Non-D&D advancement rules

Light custom mechanics are allowed only when they sit on top of D&D 5e / 2024 assumptions.

---

## NPC Mechanical Standards

Not every NPC needs a full stat block.

Use these tiers:

### Tier 1: Major Combat-Relevant NPCs

Required for:

* Villains
* Recurring adversaries
* Major allies or companions
* Rival adventurers
* Faction champions
* Bosses
* Important spellcasters
* NPCs likely to fight, travel with, or oppose the player directly

Must include:

* Suggested level or challenge role
* Creature type
* Size
* Armor Class
* Hit points or HP range
* Speed
* Ability score emphasis
* Saving throw proficiencies
* Skill proficiencies
* Senses, if relevant
* Languages
* Proficiency bonus or CR-equivalent guidance
* Main attacks/actions
* Bonus actions, if relevant
* Reactions, if relevant
* Spellcasting, if relevant
* Signature abilities
* Tactics
* Morale
* Solo-play danger rating
* Noncombat ways to handle them
* Notes for scaling up/down

These NPCs may have a class/subclass if appropriate, but do not automatically build every important NPC as a full PC.

### Tier 2: Important Noncombat NPCs

Required for:

* Political leaders
* Patrons
* Priests
* Sages
* Merchants
* Quest-givers
* Criminal contacts
* Witnesses
* Social rivals
* Important townspeople

Must include:

* Approximate level of competence
* Relevant ability strengths
* Relevant skills
* Passive Insight / Perception if useful
* Social leverage
* Resources
* Whether they are dangerous in combat
* Suggested fallback stat block if combat unexpectedly occurs
* Important spells or abilities if any

Example fallback language:
“Use Noble-like social profile, noncombatant unless cornered.”
“Use Spy-like profile with stronger Insight and Deception.”
“Use Priest-like profile with access to low-level divine magic.”

### Tier 3: Minor NPCs

Required for:

* Shopkeepers
* Guards
* Villagers
* Travelers
* Servants
* Minor criminals
* Local color NPCs

Must include:

* Name
* Role
* Location
* Personality hook
* Useful detail
* Combat relevance: none / commoner-like / guard-like / specialist
* Any notable skill or tool proficiency

Minor NPCs do not need full stats unless they become important.

---

## Monster and Adversary Standards

Every custom monster or adversary group must include D&D-compatible mechanical guidance.

At minimum:

* Creature type
* Size
* Role
* Approximate CR or level range
* Armor Class
* Hit point range
* Speed
* Key ability scores or modifiers
* Saving throws
* Skills
* Damage resistances/immunities/vulnerabilities, if any
* Condition immunities, if any
* Senses
* Languages
* Main actions
* Special traits
* Tactics
* Morale
* Encounter role
* Solo-play danger notes
* Scaling guidance

Do not create monsters that only have narrative descriptions.

---

## Quest Mechanical Standards

Every developed quest must include:

* Recommended character level or level range
* Expected danger level for a solo PC
* Likely checks and DC ranges
* Possible combat encounters
* Possible noncombat solutions
* Rewards appropriate to level
* Rest opportunities or time pressure
* Failure consequences
* Scaling notes

Use D&D-style DCs:

* DC 10: Easy
* DC 15: Moderate
* DC 20: Hard
* DC 25: Very hard
* DC 30: Nearly impossible

Do not require a single successful roll to continue the story.

---

## Dungeon Mechanical Standards

Every dungeon or ruin must include:

* Recommended level range
* Expected solo danger rating
* Encounter list
* Trap DCs and effects
* Puzzle DCs or clue checks, if any
* Resting constraints
* Wandering danger, if any
* Treasure
* Boss or climax mechanics
* Scaling notes
* Retreat options

---

## Encounter Design For Solo D&D

Because the campaign is for one player character:

* Do not assume a four-character party.
* Avoid large enemy groups unless there are clear tactical advantages, allies, stealth routes, or escape routes.
* Dangerous fights must be telegraphed.
* Bosses should have weaknesses, terrain options, or noncombat alternatives.
* Use morale and enemy goals; not every enemy fights to the death.
* Include ways to scout, negotiate, bypass, prepare, or retreat.
* Death can happen, but cheap death is bad design.

Every dangerous encounter should include:

* Warning signs
* Enemy goals
* Tactics
* Morale
* Escape options
* Noncombat alternatives
* Scaling advice

---

## Companion and Ally Mechanics

If the campaign provides a recurring companion, sidekick, patron, summoned aid, or hireling, include:

* Role
* Level or scaling model
* AC
* HP
* Key abilities
* Main actions
* Limitations
* Personality
* Loyalty triggers
* Risk of death/injury
* How they avoid overshadowing the player

Companions should support the solo PC, not solve the campaign.

---

## Leveling Requirements

The campaign must support progression from level 1 to level 20.

Maintain:

* `/03_canon/LEVELING_ASSUMPTIONS.md`
* `/12_campaign_arc/LEVEL_1_TO_20_PROGRESSION.md`
* Level ranges on quests, regions, dungeons, and major threats
* Reward guidance by tier

Level tiers:

* Levels 1–4: Local danger, survival, first mysteries
* Levels 5–8: Regional influence, stronger factions, supernatural escalation
* Levels 9–12: Major political and magical consequences
* Levels 13–16: World-scale threats and ancient powers
* Levels 17–20: Endgame, legendary threats, final truths

---

## Stat Block Creation Rule

When creating a major combat-relevant NPC, monster, boss, or companion, do not leave mechanics as “TBD” unless explicitly creating a placeholder.

Use one of these approaches:

1. Full custom stat block
2. D&D-compatible abbreviated stat profile
3. Reference-style profile such as “use a veteran-like baseline, modified as follows,” without copying copyrighted text
4. Scaling profile by level tier

Avoid copying official stat blocks verbatim.

---

## Mechanical Completeness Check

Before marking a region, quest, dungeon, faction arc, or campaign act complete, check:

* Are level ranges listed?
* Are combat-relevant NPCs mechanically usable?
* Are monsters mechanically usable?
* Are quests assigned recommended levels?
* Are DCs included where checks are likely?
* Are rewards appropriate to level?
* Are solo-play danger notes included?
* Are scaling notes included?
* Are companions/allies mechanically described?
* Are major threats more than just narrative descriptions?

If not, mark the content as mechanically incomplete in TODO.md or CONTENT_GAPS.md.
