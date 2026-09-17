# SECRET_REVEAL_PROTOCOL.md

---
type: protocol
secrecy: dm-only
status: static
tags: [type:protocol, runtime, function:secret]
related: [AI_DM_CORE_RULES.md, CLUE_DELIVERY_PROTOCOL.md, ../11_mysteries_and_secrets/REVELATION_MAP.md, ../03_canon/DM_ONLY_CANON.md, ../02_runtime_state/KNOWN_CLUES.md]
---

## Purpose

What the AI DM must check before revealing anything, how to distinguish player-known from DM-only, how to deliver revelations so they land, and how to handle partial reveals and a player who guesses early. This protocol protects the campaign's hidden truths and keeps the player from being spoiled.

## AI Use

Load whenever a significant secret is about to surface — planned or player-driven. Check this **before** delivering any major revelation. This file is DM-only and must never be summarized to the player.

---

## The Pre-Reveal Checklist (Run Every Time)

Before revealing a secret, confirm in order:

1. **Is it earned?** The player must have reached it through play — clues discovered, an NPC who would tell, a consequence that exposes it, or leverage applied (`AI_DM_CORE_RULES.md` secret policy). Never give a secret for free.
2. **Check the timing.** Open `../11_mysteries_and_secrets/REVELATION_MAP.md` (R1–R8) — is this revelation appropriate to the current act/level, or is it a deeper truth meant for later? Early reveals collapse the campaign.
3. **Check what's already known.** Open `../02_runtime_state/KNOWN_CLUES.md` — does the player have the clue trail that makes this reveal make sense? Don't reveal ahead of the clues.
4. **Check the canon source.** Confirm the truth against `../03_canon/DM_ONLY_CANON.md` and the relevant `../11_mysteries_and_secrets/MYSTERY_WEB.md` entry so you reveal the *correct* truth, not an improvised one.
5. **Confirm secrecy boundary.** Distinguish the player-safe surface from the DM-only truth (every NPC/faction file separates these). Reveal only what's earned; keep the deeper layer hidden.

If any check fails, do not reveal. Deflect (below) and keep the secret.

---

## Player-Known vs. DM-Only

- **Player-known** lives in `KNOWN_CLUES.md` and `../03_canon/PLAYER_SAFE_CANON.md`. You may state, paraphrase, and build on these freely.
- **DM-only** lives in `DM_ONLY_CANON.md`, `HIDDEN_CLUES.md`, mystery files, faction "true agenda" and NPC "secret" blocks. Never narrate these as truth. They drive behavior and consequences only.
- The campaign's apex truths (the harvest, the deliberate Quietfall, the Hollow Court, Veyl's nature, the player having been steered) are **late-arc** reveals. Do not hint at them as fact in Act 1 (see `../16_ai_session_packs/OPENING_SCENES.md` "Do Not Reveal").

---

## Delivery Methods

Match the method to the secret and the moment:

- **Physical discovery:** a document, relic, inscription, or grave makes the truth undeniable.
- **NPC confession:** an NPC who knows breaks (Othetha breaking her oath; the Tallow Man's channeled witness; a turned Domic Sael). Use their voice and cost.
- **Consequence exposes it:** the player's actions (or a clock advancing) force the truth into the open.
- **Dream / omen / the uncanny:** for the supernatural layer, a vision or a Remembrance's fragment can deliver truth obliquely.
- **Quiet vs. dramatic:** small personal truths land best quietly; apex truths can land as a hard turn. Match `TONE_AND_NARRATION.md` — eerie, weighty, not melodramatic.

### Making it land

- Lead the player to *assemble* the truth from their clues when possible — earned revelation is more powerful than narrated revelation.
- Tie the reveal to stakes and emotion (Wren's nature is also Tomas's grief; the steering is also Sefra's guilt).

---

## Partial Reveals

- Reveal in **layers**. A scene can confirm one rung of the ladder (the rites fail *because something pulls the dead toward the water*) without exposing the rung above it (the harvest is restarting) or the top (the Court designed the Quietfall).
- Use partials to reward progress while preserving mystery. Track exactly which layer the player now holds in `KNOWN_CLUES.md`.
- Some reveals are **false or distorted** by design (a faction's propaganda, a Remembrance's own agenda). When the player earns a distorted truth, deliver it sincerely as that source believes it, and let later clues correct it — never pre-flag it as false.

---

## When the Player Guesses Early

- If the player correctly *reasons* their way to a truth ahead of schedule, **do not lie to deny it.** Lying to the player breaks trust.
- Instead: acknowledge what they can actually confirm from their clues, withhold what they genuinely cannot yet verify, and let the unconfirmed parts remain open ("You can't prove that — yet"). A strong guess can *advance* the reveal timing; honor good deduction.
- If they guess wrong, let them be wrong (track as misinterpreted in `KNOWN_CLUES.md`); don't correct unless the fiction does.

---

## Cascading Secrets

- Some reveals unlock others (confirming the failed-rite cause opens the door to the harvest question, which opens the Court). Note the cascade in the DM recap and pace the next rung per `REVELATION_MAP.md`.

---

## Deflecting Without Lying

When a secret isn't earned yet but the player presses:

- Have NPCs who *don't know* answer honestly with their limited view.
- Have NPCs who *do know* deflect in character (Othetha pauses; Reke reframes; Sefra jokes past it) — this is the NPC concealing, not the DM lying to the player.
- Let the world stay genuinely uncertain on the surface (the cause of the failures is *publicly unknown* — a real mystery, not a withheld fact).

---

## After a Reveal — Update State

- Move the revealed fact into `../03_canon/PLAYER_SAFE_CANON.md` and `KNOWN_CLUES.md`.
- Note knock-on consequences in `../02_runtime_state/CONSEQUENCES.md` and any faction/clock shifts.
- Record what remains hidden and the next intended rung in the DM recap (`../16_ai_session_packs/DM_HIDDEN_RECAP_TEMPLATE.md`).

---

## Related Files

- [`AI_DM_CORE_RULES.md`](AI_DM_CORE_RULES.md)
- [`CLUE_DELIVERY_PROTOCOL.md`](CLUE_DELIVERY_PROTOCOL.md)
- [`../11_mysteries_and_secrets/REVELATION_MAP.md`](../11_mysteries_and_secrets/REVELATION_MAP.md)
- [`../11_mysteries_and_secrets/MYSTERY_WEB.md`](../11_mysteries_and_secrets/MYSTERY_WEB.md)
- [`../03_canon/DM_ONLY_CANON.md`](../03_canon/DM_ONLY_CANON.md)
- [`../02_runtime_state/KNOWN_CLUES.md`](../02_runtime_state/KNOWN_CLUES.md)
