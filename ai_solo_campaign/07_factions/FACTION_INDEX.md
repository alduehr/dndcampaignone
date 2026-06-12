# FACTION_INDEX.md

---
type: index
secrecy: mixed
status: static
tags: [index, factions]
---

## AI Use

Master list of all factions. Load to find which faction file to open. Public faces are player-safe; hidden agendas are DM-only (see each file's DM-Only section and `../03_canon/DM_ONLY_CANON.md`). For the full pairwise relationship map see `FACTION_RELATIONSHIP_MAP.md`; for between-session faction behavior see `FACTION_TURN_RULES.md`.

## Stage 8 Faction Deepening Companion Files

| File | Purpose |
|---|---|
| `FACTION_RELATIONSHIP_MAP.md` | Full pairwise relationships (every pair + the Hollow Court's hidden ties); blocs for faction turns |
| `FACTION_TURN_RULES.md` | When/how the AI DM runs faction turns between sessions; clock advancement; rumors; state updates |
| `../09_quests/faction_quests/[FACTION]/` | Each faction's 4-quest chain (intro → trust → moral complication → internal-conflict decision point) |

## Major Factions

| Faction | File | Scope | Public Face | Hidden Agenda (DM) | Clock | Player can | Quest Chain |
|---|---|---|---|---|---|---|---|
| Ashen Wardens | `major_factions/ASHEN_WARDENS.md` | Reach/Orrun | Lay the restless dead to rest | Unknowing guardians of the seal | The Wardens Break | join / aid / ignore | `../09_quests/faction_quests/ASHEN_WARDENS/` (QW1-4) |
| Cinder Ledger | `major_factions/CINDER_LEDGER.md` | Orrun | Bank/merchants; buy salvage | Monopolize and sell the Remembrance | The Monopoly Closes | work for / oppose / ignore | `../09_quests/faction_quests/CINDER_LEDGER/` (QL1-4) |
| Mourners' Circle | `major_factions/MOURNERS_CIRCLE.md` | Reach | Folk grief-faith; tend the dead | Closest to the moral truth; may destroy the shrines | The Circle Turns Militant | join / aid / oppose | `../09_quests/faction_quests/MOURNERS_CIRCLE/` (QM1-4) |
| Reachward Compact | `major_factions/REACHWARD_COMPACT.md` | Reach | Frontier council/government | Infiltrated; steered to reopen the shrine | The Basin Drains (master infrastructure clock) | serve / reform / oppose | `../09_quests/faction_quests/REACHWARD_COMPACT/` (QC1-4) |
| Gravecallers | `major_factions/GRAVECALLERS.md` | Reach | Outlawed cult that speaks to the dead | Right about the harvest; would break it catastrophically | The Breaking | join / learn from / oppose | `../09_quests/faction_quests/GRAVECALLERS/` (QG1-4) |
| Concord Remnant | `major_factions/CONCORD_REMNANT.md` | Orrun/Caradril | Scholars rebuilding the Concord | Inner circle would seize the harvest | The Reclamation | study with / expose / join | `../09_quests/faction_quests/CONCORD_REMNANT/` (QR1-4) |
| Hollow Court | `major_factions/HOLLOW_COURT.md` | Sundering Reach (under-shrine) | Legend / ghost story | **Apex power: surviving Custodians restarting the harvest** | The Harvest Restarts (MASTER CLOCK) | uncover / oppose / (late) join | `../09_quests/faction_quests/HOLLOW_COURT/` (QH1-4, **DM-only**; no early recruit) |

## Caradril City Factions (Stage 4 — city-internal)

> City-internal power blocs of the first major city. Detailed in the Caradril settlement/district files, not in `major_factions/`. The Cinder Ledger (HQ: Ledger Keep) and Concord Remnant (seat: Lantern Reach) — listed above as major factions — have their headquarters in Caradril; the Vyre–Quorrin deal is negotiated here.

| Faction | File | Scope | Public Face | Hidden Agenda (DM) | Clock |
|---|---|---|---|---|---|
| Tidewater Council / Charter Houses | `../06_settlements/caradril_districts/THE_MAGISTERIUM.md` | Caradril | The city-state's merchant government | Complacent; the Stilling masks the harvest's pause; a magister corresponds with Reke (lead only) | C2 The Council Sleeps |
| Tide-Watch | `../06_settlements/caradril_districts/THE_MAGISTERIUM.md` | Caradril | The city watch/law | Class-biased; Kade privately turnable | (tied to C2) |
| Salt Syndicate | `../06_settlements/caradril_districts/THE_ASHMARKET.md` | Caradril | Smugglers / black market | Sells relics that hold the dead, unknowing (M3); shelters the Sill | (feeds C1/C3) |
| The Hush | `../06_settlements/caradril_districts/THE_SILL.md` | Caradril | Information brokers | Sells mid-arc clue-fragments; every secret carries a hidden price | (feeds C1/C2) |

## Faction Relationship Map

| Faction | Relationship | Public Reason | Hidden Reason | Current Tension |
|---|---|---|---|---|
| Wardens ↔ Mourners | Allied | Both revere letting the dead rest | Wardens secretly guard the seal | Both overwhelmed by failures |
| Wardens ↔ Gravecallers | Enemies | Gravecallers "call" the dead Wardens lay | Wardens guard the seal the Gravecallers would break | Rising; Gravecallers gaining ground |
| Mourners ↔ Gravecallers | Enemies (but radicals overlap) | Gravecallers defile the dead | Both want the harvest ended | Iola Wend bridges them secretly |
| Ledger ↔ Mourners | Enemies | Ledger buys grave-relics | Ledger's monopoly desecrates the dead | Mob action brewing |
| Ledger ↔ Remnant | Secret allies | (hidden) | Vyre + Quorrin plan a Remembrance monopoly | Mutual mistrust; both want control |
| Ledger ↔ Compact | Allied | Ledger funds Compact works | Funds the basin scheme that reopens the shrine | None public |
| Compact ↔ Mourners | Strained | Basin scheme vs. grave-reverence | Reke (Court agent) pushes the scheme | High; Circle furious |
| Remnant ↔ Hollow Court | Rivals (unaware) | n/a (Court is "legend") | Both want the harvest; rivals for the keystone | Hidden race |
| Hollow Court ↔ Compact | Infiltration | n/a | Reke is a Court agent | Invisible to all but Reke |
| Hollow Court ↔ Wardens | Natural enemies | n/a | Court restarts what Wardens unknowingly seal | Invisible; the campaign's deep conflict |
| Ledger ↔ Charter Houses (Tolm) | Rivals | Old money vs. the upstart bank | Tolm would aid the player vs. Vyre, for his own ends | The open-charter contest (Caradril) |
| Tide-Watch ↔ Salt Syndicate | Enemies (uneven) | Law vs. crime | The Watch favors the rich; the Syndicate feeds the Sill | `Q_THE_TIDE_TURNS` (Caradril) |
| Salt Syndicate ↔ The Hush | Rivals | Two underworlds | The Hush sells the Syndicate out | Caradril underworld struggle |
| Hush ↔ everyone | Leverage | "Knows things" | Brokers the deal/correspondent/Wards secrets | Citywide (Caradril) |

## Related Files

- [`FACTION_RELATIONSHIP_MAP.md`](FACTION_RELATIONSHIP_MAP.md)
- [`FACTION_TURN_RULES.md`](FACTION_TURN_RULES.md)
- [`../03_canon/DM_ONLY_CANON.md`](../03_canon/DM_ONLY_CANON.md)
- [`../02_runtime_state/FACTION_STATE.md`](../02_runtime_state/FACTION_STATE.md)
- [`../02_runtime_state/WORLD_CLOCKS.md`](../02_runtime_state/WORLD_CLOCKS.md)
