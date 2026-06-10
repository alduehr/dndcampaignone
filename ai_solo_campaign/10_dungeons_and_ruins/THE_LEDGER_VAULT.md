# The Ledger Vault (Hollowmere Counting-House)

---
type: dungeon
secrecy: mixed
status: static
region: Sundering Reach
settlement: Hollowmere
factions: [Cinder Ledger, Concord Remnant]
level_range: 2-4
related: [../06_settlements/HOLLOWMERE.md, ../07_factions/major_factions/CINDER_LEDGER.md, ../11_mysteries_and_secrets/MYSTERY_WEB.md]
tags: [type:dungeon, secrecy:mixed, region:sundering-reach, level:2-4, heist, function:clue, function:social]
---

## AI Use

Load for the M3 clue path "the Ledger vault relic" (C-M3-3) — a **social/stealth heist**, not a monster dungeon. The Cinder Ledger's Hollowmere counting-house holds a vault relic that "remembers" the harvest. The intended primary path is **turning Factor Domic Sael** (social), with a stealth break-in as the harder alternative. **Low combat danger; high consequence danger** (crossing the Ledger). A showcase of noncombat dungeon design.

## One-Sentence Identity

The Cinder Ledger's locked Hollowmere vault, where a relic that remembers a dead person waits behind ledgers, locks, and a nervous factor's conscience.

## History

The counting-house is a solid stone building on the Rim, the Ledger's local seat. **Truly (DM):** Mother Vyre had a particular relic moved here for safe study — a Remembrance relic that *demonstrably stores a dead person* (C-M3-3) and is the clearest mercantile proof of the harvest's nature. Domic Sael knows it's there, thinks Vyre's obsession is reckless, and is quietly documenting it — making him turnable.

## Entrance

Front: the public counting-room (open by day; Domic and clerks present). Back: a guarded strong-room corridor to the vault. **Telegraphed:** the player learns of the relic via rumor (Rumor 6), Domic's unease (Hook 3 follow-up), or Mourner/Remnant interest. Multiple ways in — talk, sneak, or (worst) force.

## Solo Danger Rating

**Low combat / high consequence (level 2–4).** Almost no lethal threat; the danger is getting caught and earning the Ledger's enmity (debt, blacklist, enforcers, a powerful enemy faction). A deliberate "the stakes aren't HP" set-piece.

## Zone / Room List

1. **The Counting-Room** — public; Domic, 1–2 clerks, the day-ledgers. Social hub; the turn-Domic path lives here.
2. **The Records Office** — where Domic keeps his quiet documentation (a clue to Vyre's scheme; **C-M4-4 / Secret 12 support**). Lightly secured.
3. **The Strong-Room Corridor** — guarded passage to the vault; the Ledger tough (Tallytooth Ren) patrols.
4. **The Vault** — the locked relic-room: the **vault relic (C-M3-3)**, the Ledger's coin-reserve, and salvage stock. The objective.

## Encounter List

- **The Counting-Room:** **Domic Sael** (secondary; noncombatant) + 1–2 clerks (commoners). **Social, not combat.**
- **The Strong-Room Corridor:** **Tallytooth Ren** (secondary — registered Ledger enforcer; **Thug/Spy-like**, AC 13, ~40 HP, intimidation-focused) and possibly 1 guard (**Guard-like**, AC 16, ~11 HP). Prefer to catch, eject, and report rather than kill.
- **The Vault:** no creatures; locks and a possible alarm.
- **Caught anywhere:** the Ledger's response is **legal/economic ruin first, violence last** — telegraphed warnings, not a kill-squad.

## Traps / Hazards (DCs)

- **Vault lock:** quality Ledger lock — Thieves' Tools DC 17 (DC 13 with Domic's key/help). Failure (hard fail) trips a bell-alarm.
- **Bell-alarm:** ringing it brings Ren + guards within 1 round (a chase/escape scene, not a death-trap).
- **Records Office lock:** DC 13 Thieves' Tools.
- **Watch patrol timing:** Ren patrols the corridor; Stealth (DC 14) or distraction to pass; failure = detection (social consequence, not damage).

## Puzzle / Clue Checks

- **Turning Domic (primary path):** a social "puzzle." Domic can be turned with evidence of Vyre's recklessness, an appeal to conscience, or leverage (Persuasion/Insight DC 14; lower if the player has helped him or holds the Peat Chapel relic). A turned Domic *gives* the player vault access and the relic's meaning — the intended, low-risk route.
- **The relic itself (C-M3-3):** examining it (Arcana/Religion DC 15, or simply using it) reveals it **stores a dead person's identity** — the mercantile proof of M3. A clean, fair clue.
- **Domic's documentation (Records Office):** reading it (Investigation DC 13) exposes Vyre's monopoly scheme (Secret 12; M4 support).

## Resting Constraints

This is an urban site — the player rests at the Drowned Lantern. No in-site rest (you don't sleep in a vault). Time pressure is social (patrols, opening hours), not survival.

## Treasure

- **The vault relic** (C-M3-3; the clue-prize — and a hot potato every faction wants).
- Ledger coin-reserve (~200 gp, but taking it makes the player a hunted thief — a trap for the greedy).
- Domic's documentation (Secret 12 proof — arguably worth more than the gold).

## Boss / Climax Mechanics

No combat boss by design. The "boss" is the **fork:** turn Domic (clean, makes an ally, low risk), sneak the vault (risky, may make the Ledger an enemy), or rob it outright (high reward, high heat — Vyre marks the player). Tallytooth Ren is a **catch-and-intimidate** obstacle, not a kill: AC 13, ~40 HP, grapple + threats; he'd rather march a caught intruder to the reeve (or Vyre) than spill blood in the counting-house.

## Retreat Options

Always available — it's a building in a friendly town. The cost of a botched job is reputation and a powerful enemy, not death. The player can walk away and try the social path instead.

## Scaling Notes

- **Level 2:** Ren alone, simpler lock (DC 15); generous Domic-turn.
- **Level 4:** add 2 guards, a better lock (DC 18), a Remnant agent *also* trying for the relic (a three-way heist; ties to the Vyre–Quorrin deal).

## Consequences If Ignored

If the player never pursues the relic, M3 is still reachable (Gravecallers, Peat Chapel, Deep Adit), but the Ledger quietly ships the relic to Caradril for the Vyre–Quorrin deal (advancing the Monopoly and Reclamation clocks) and Domic, unturned, stays a wasted potential ally — or is silenced when Vyre learns he documented her.

## State Update Triggers

- Domic turned: update `RELATIONSHIPS.md` (ally), `FACTION_STATE.md` (Ledger internal crack); mark Secret 12 progress.
- Relic obtained: `INVENTORY_AND_REWARDS.md`; mark C-M3-3 in `KNOWN_CLUES.md`.
- Caught/robbed: `FACTION_STATE.md` (Ledger → suspicious/hostile), `CONSEQUENCES.md` (debt/blacklist/bounty), `NPC_MEMORY.md` (Domic, Ren, Vyre).

## Related Files

- [`../06_settlements/HOLLOWMERE.md`](../06_settlements/HOLLOWMERE.md)
- [`../07_factions/major_factions/CINDER_LEDGER.md`](../07_factions/major_factions/CINDER_LEDGER.md)
- [`../08_npcs/SECONDARY_NPCS.md`](../08_npcs/SECONDARY_NPCS.md)
- [`../11_mysteries_and_secrets/MYSTERY_WEB.md`](../11_mysteries_and_secrets/MYSTERY_WEB.md)
