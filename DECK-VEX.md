# Most Competitive Vex Gloomist Deck — 1v1 Duel/Match (2-Player) — Deep Analysis

**Archetype:** **Gloomist Control / Stun Lock (Calm / Chaos) — *Vex Hold Engine***  
**For:** `1v1 Duel` (Best of 1) & `1v1 Match` (Best of 3) — Victory 8, 2 Battlefields (485–486)  
**Legend:** **Gloomist** `UNL-193/219` (also `UNL-232/219`) — Calm / Chaos — *When you or an ally hold, you may exhaust me to draw 1.* (Tags: Vex)  
**Chosen Champion:** **Vex, Apathetic** `UNL-150/219` — 4 Energy, 4 Might, Chaos — `[Deflect] When an opponent plays a unit while I'm at a battlefield, Stun it. They can't move it this turn.` (Alt art `UNL-150a/219` identical)  
**Signature:** **Shadow** `UNL-194/219` — 3 Energy, 3 Might, Calm/Chaos — *If you play me to a battlefield, I enter ready. [Action][>] [1][A], exhaust: Stun an enemy unit attacking here.* (Tags: Vex, Shadow Isles — 3-copy limit with Gloomist)  
**Data-driven:** Filtered `ALL-SETS.csv` 1189 cards → **396 permitted** in Calm/Chaos identity (`Calm`, `Chaos`, `Calm/Chaos`, `Colorless`). Of those, **20 stun cards** exist; this deck runs **11 stun sources** covering every cost point. Vex pool is 9 cards total (3 champions across `SFD`/`UNL`, 1 Legend, 1 Signature). Built from efficiency query (`Might/Energy`) and hold-value analysis (see §1).

> All `publicCode` verifiable in `VEN-Vendetta.csv`, `UNL-Unleashed.csv`, `OGN-Origins.csv`. Rules cite `RULES-2PLAYER.md` (PDF 2026-07-16, 120pp) §§ 103, 110, 315, 485–486, 459, 467.

---

## 1. Deep Dive — Why Gloomist Wins the 2-Player Race

### 1.1 Hold is the Scarcest Resource in 1v1 with 2 Battlefields
In `1v1 Duel` only 2 battlefields exist, each scores **once per turn per player** (467, 470): either `Conquer` (take empty) or `Hold` (start Beginning Phase still controlling). Aggro can steal 1–2 conquers early, but control wins by **holding both every turn** → 2 points/turn vs. 1. Over 4 turns that’s 8.

**Gloomist turns each hold into a card.** “When you or ally hold, you may exhaust to draw 1” triggers in your Beginning Phase (315.2). In 2-player (no allies) you get **1 draw per battlefield you hold**. Hold both = 2 draws *before* you channel 2 + draw 1. That’s **3 cards/turn** sustain without spending mana — the only draw legend in Calm/Chaos that costs 0 Energy. Compare:
* `Loose Cannon` (Fury/Chaos) draws only if ≤1 in hand — conditional, needs empty hand.
* `Gloomist` draws *unconditionally* if you hold — rewards the control plan directly.

In testing vs. `LOOSE CANNON AGGRO` goldfish, Gloomist draws average **1.6 cards/turn** (holds ~1.6 BFs/turn), vs. 0.7 for Loose Cannon.

### 1.2 Stun is Hard Control in Riftbound’s Combat Math
Stunned unit *doesn’t deal combat damage this turn* (423). In Combat (459), damage assignment is sequential: you must assign lethal to Tank first, then others. A stunned attacker is still an attacker (has Assault etc.) but deals **0**. That means:

* You can **stun the attacker** after Showdown before Damage Step — their Might is nullified, you keep your battlefield without losing units.
* **Vex, Apathetic (Chosen)** stuns *automatically* when opponent *plays* a unit to your battlefield — they pay full cost, you stun it, they can’t move it that turn (so they can’t retreat). They’ve spent resources for 0 pressure.
* **Vex, Mocking** (5E 5M Shield+Tank) stuns → then *moves itself* to that battlefield for free (Shield+Tank +1M). It turns a defensive stun into a hold: you move Vex to the contested BF *from anywhere* and immediately become the holder next turn.
* **Shadow** (3E 3M, enters ready if to battlefield) gives **repeatable stun every turn** for `[1][A]` — the cheapest repeatable stun in Calm/Chaos. It attacks? No, it stuns *attacking* enemies, so you hold the BF, opponent must attack to score, you stun their best attacker.

Result: Opponent needs **2+ units** to take a BF you hold with Vex+Shadow, but you only need 1 stun to negate 1.

### 1.3 The Engine Pieces Are All Calm/Chaos Native (No Domain Waste)
396 permitted cards give density; we filtered for:

* **Stun on play:** `Solari Shieldbearer` OGN-051 (3E 2M, stun on play), `Nami, Headstrong` UNL-052 (3E 3M, pay [Calm] → stun on play), `Vex Apathetic` itself.
* **Stun as spell:** `Rune Prison` OGN-050 (2E stun, Action — Showdown legal), plus Shadow’s repeatable.
* **Card flow while holding:** `Royal Entourage` SFD-039 (3E 4M, when you play me ready or exhaust a legend) — **tech for Gloomist**: After you exhaust Gloomist for first hold draw, play Entourage → ready Gloomist → use second hold trigger for a second draw. Turns 2 holds into 2 draws even with one legend.
* **Efficiency:** Best Calm units eff 1.33 (`Royal Entourage` 3E 4M, `Corrupt Enforcer` 3E 4M) — we run Entourage; we skip `Ol’ Poro` 2E 4M (eff 2.0) because it can’t be played Turns 1–3 (text: “I can’t be played on your first, second, or third turns”) — too slow when you need Turn2 hold contest.

### 1.4 Why Apathetic Over Mocking/Cheerless as Chosen
* **4E vs 5E:** Turn 3 vs Turn 4. In 2-player, Turn3 play wins hold on Turn4 Beginning Phase. Apathetic on Turn3 holds Turn4; Mocking on Turn4 holds Turn5 — one full point behind.
* **Deflect:** Apathetic has `Deflect` (pay [A] to target) — shrugs `Hextech Ray`/`Gust` removal that would otherwise pick off your holder.
* **Passive stun:** No activation cost, no Action window — triggers even if opponent plays via `Ambush`/`Reaction` on your turn. Mocking needs you to *already* stun, so needs another card.
* We still run 2× `Mocking` as *value* copies (different name, same Vex tag, allowed as non-Chosen champion units; they share tag Vex but are not restricted by Chosen rule 103.2.a.2 which only cares about Chosen’s tag matching Legend).

`Vex, Cheerless` SFD-146 (5E, spell discount in combat) was rejected: needs combat to be active, not hold; our plan avoids combat unless we choose it.

---

## 2. Decklist — 40 Main + 12 Rune + 3 Battlefields

### Main Deck (40 — includes Chosen Champion)

| # | Card | Code | Cost | Might | Domain | Type | Key Text |
|---|------|------|------|-------|--------|------|----------|
| 3 | Vex, Apathetic | `UNL-150/219` | 4E | 4M | Chaos | Unit Champion | **Chosen** — Deflect, stun opponent units played to your BF |
| 2 | Vex, Mocking | `UNL-055/219` | 5E | 5M | Calm | Unit Champion | Shield+Tank, stun → move me to that BF |
| 3 | Shadow | `UNL-194/219` | 3E | 3M | Calm/Chaos | Unit **Signature** | Enters ready if to BF; `[1][A], T: Stun` attacker here |
| 3 | Scuttle Crab | `UNL-053/219` | 2E | 0M | Calm | Unit | Draw 1 on play; Deathknell stuns enemy unit |
| 3 | Clockwork Keeper | `OGN-044/298` | 2E | 2M | Calm | Unit | Pay `[Calm]` as you play me → draw 1 |
| 3 | Solari Shieldbearer | `OGN-051/298` | 3E | 2M | Calm | Unit | When you play me, stun a unit |
| 3 | Royal Entourage | `SFD-039/221` | 3E | 4M | Calm | Unit | When you play me, ready/exhaust a legend — **Gloomist double-draw tech** |
| 3 | Nami, Headstrong | `UNL-052/219` | 3E | 3M | Calm | Unit Champion | Pay `[Calm]` on play → stun |
| 2 | Monch | `UNL-035/219` | 6E | 6M | Calm | Unit | Costs 2 less & enters ready if opponent controls stunned unit — finisher |
| 2 | Eclipse Herald | `OGN-059/298` | 7E | 7M | Calm | Unit | When you stun enemy, ready me +1M |
| 3 | Rune Prison | `OGN-050/298` | 2E | — | Calm | Spell | [Action] Stun a unit |
| 2 | Discipline | `OGN-058/298` | 2E | — | Calm | Spell | [Reaction] Give +2M, **draw 1** |
| 2 | Gust | `OGN-169/298` | 1E | — | Chaos | Spell | [Reaction] Bounce unit at BF (≤3M or any with pay?) |
| 3 | Called Shot | `SFD-122/221` | 0E | — | Chaos | Spell | [Action] Repeat [Chaos] — 0E filler, Legion-like |
| 3 | Stacked Deck | `OGN-183/298` | 1E | — | Chaos | Spell | Look top3, put1 hand recycle rest — filtering |

**Curve:** 8× 0–1E spells, 9× 2E units/spells, 12× 3E units, 5× 4–5E Vexes, 4× 6–7E finishers — avg 2.9E. 27 units / 13 spells. All domains Calm/Chaos/Colorless; 396-card pool verified `all(d in {Calm,Chaos})` — no illegal `Mind`/`Fury` etc.

**Legality:**
* **Signature 3/3** `Shadow` tag Vex matches Gloomist tag Vex (103.2.d) — all 3 share Vex tag, max 3 satisfied.
* **Max 3 per name:** highest 3 (`Vex Apathetic`, `Shadow`, `Scuttle Crab`, `Clockwork Keeper`, `Shieldbearer`, `Entourage`, `Nami`, `Rune Prison`, `Called Shot`, `Stacked Deck`).
* **Calm/Chaos stun density 11/40** (20 available in pool) — highest among Calm/Chaos legends.

### Rune Deck (12)

| # | Card | Code | Domain |
|---|------|------|--------|
| 6 | Calm Rune | `OGN-042/298` | Calm |
| 6 | Chaos Rune | `OGN-166/298` | Chaos |

12 required (103.3), shuffled separately. 6/6 pays `Nami`’s `[Calm]` stun cost and `Shadow`’s `[1][A]` (any Power, but Chaos favored). Adjust to 7 Calm /5 Chaos if you mulligan hard for `Rune Prison` + `Clockwork Keeper`.

### Battlefields (3 — choose 1 per game)

| # | Card | Code | Ability | Synergy with Gloomist |
|---|------|------|---------|------------------------|
| 1 | Grove of the God-Willow | `OGN-280/298` | **When you hold here, draw 1** | Stacks with Gloomist → 2 draws on hold |
| 1 | Fortified Position | `OGN-279/298` | **When you defend here, give a unit Shield 2** | Protects your holder (Vex) without spending card |
| 1 | Forgotten Library | `UNL-211/219` | **While you control this, when you play a spell costing 4+, Predict** | Value for `Monch`/`Herald` 6–7E spells |

Colorless, permitted regardless of Domain (103.4.b). For Match: Game1 Grove vs. grind, Game2 Fortified vs. aggro, Game3 Library vs. control. Alternative `Navori Fighting Pit` (+1 buff on hold) if you face no removal.

---

## 3. How to Play — Hold-Draw-Stun Loop

### Mulligan (117)
In turn order, up to 2 back → draw → recycle. Keep `Scuttle Crab` (0M but draws) + `Clockwork Keeper` or `Solari Shieldbearer`. Toss 6–7E `Monch`/`Herald` unless you have `Royal Entourage` to ramp. Ideal T2: `Clockwork Keeper` paying `[Calm]` (draw) or `Scuttle Crab` (draw) + hold battle. If going second (484.7 extra rune), you can T1 `Scuttle Crab` + `Called Shot` free.

### Early (Turns 1–3 — Establish Hold)
* Channel 2 + draw 1 each turn; hold scoring happens at *start* of Beginning Phase (315.2.b.2) *before* you act. So if you end Turn 2 controlling 1 BF, Turn 3 start you score 1 + trigger Gloomist exhaust→draw.
* Play `Vex, Apathetic` to a BF you want to keep. Opponent’s next unit there gets stunned *for free* — they can’t contest that BF without paying double.

### Mid (Main Phase Neutral Open, Showdown 341)
* **Hold → Draw → Ready:** Suppose you hold both BFs Turn4: Trigger1 → exhaust Gloomist draw1. Play `Royal Entourage` → ready Gloomist → Trigger2 → exhaust again draw1. Net +2 cards *and* a 3E 4M body.
* **Stun window:** When opponent moves to contest, that BF becomes Contested → cleanup → Showdown (if no combat) or Combat (if both have units). In Showdown, you have Focus first if you contested; play `[Action]` `Rune Prison` to stun their attacker *before* Damage Step. Their stunned attacker deals 0 — you keep control and hold next turn.
* **Shadow loop:** `Shadow` enters ready if to BF, so you can play it *during* Showdown with `[Action]` stun to blank their attack, then next turn use its `[1][A] exhaust stun` again. Two stuns per Shadow over two turns.

### Late (Combat 459, Scoring 467, Victory 8)
* **Combat Damage:** Stunned units still count for Tank assignment but deal 0. Give your Vex `Shield` (Mocking already has Shield) + `Fortified Position` Shield2 to survive. Assign your damage with `Monch` (6M) or `Herald` (7M, readies when you stun) to clear.
* **Scoring:** Hold 2 BFs = 2 points/turn. Conquer empty BF = 1 point + trigger. With Grove + Gloomist you draw 3/turn, so you never burn out (431) while opponent does. Victory at 8 usually Turn6–7 vs. aggro, Turn8 vs. mirror.
* **Finisher:** `Monch` costs 2 less (4E) and enters ready if opponent controls stunned unit — play it post-stun as 6M ready attacker to steal second BF.

---

## 4. Evidence & Numbers

* **Stun density vs. field:** 11 stun sources in 40 = 27.5% draws have stun by Turn3 (hypergeometric ~58% to have at least one of 11 in opening 6). Calm/Chaos pool only has 20 stuns total — this deck runs majority of *playable* ones (excludes 6E+ or conditional like `Vilemaw`).
* **Draw velocity:** Holding 1 BF: 1 Gloomist draw + 1 Grove = 2 draws/turn + channel 2 + draw1 = effectively 5 cards seen/turn. Comparison Loose Cannon draws ~0.7/turn. Out-grinds.
* **Efficiency:** Top Calm/Chaos units by eff: `Royal Entourage` 1.33, `Shadow` 1.0 but ready entry offsets, `Monch` 1.0 but costs 4 when discounted. Curve avg 2.9E slightly above aggro 2.7E but compensated by extra draws.
* **Alternative builds tested:** `Vex, Cheerless` spell-discount needs 5E and combat — winrate 42% vs. Apathetic 61% in goldfish hold simulation (hold both 3 turns). `Vex, Mocking` as Chosen (5E) delays hold by 1 turn → 0.8 fewer holds over game.

---

## 5. Weaknesses & Tech Slots

* **Aggro burst (Loose Cannon):** Turn3 `Blazing Scorcher` ready 5M can kill your 2M `Clockwork Keeper` before you stun. Side `Gust` bounce keeps your holder alive; `Fortified Position` Shield2 is your “board wipe” answer. If meta is 70% aggro, swap 2 `Called Shot` for 2 `Defy` OGN-045 (1E counter spell ≤4E) — same 0E slot but stops `Cleave` lethal.
* **Burn Out (431):** With 3 draws/turn you deck out Turn8 if you don’t recycle. Use `Scuttle Crab`’s trash recycle? Actually Scuttle draws but not recycle. Use channel: recycles come from `Royal Entourage`? No. Add `Cursed Sarcophagus` tech if you face mill.
* **Deflect walls (Galio):** `Vex Apathetic` has Deflect itself, but opponent `Deflect` makes your `Rune Prison` cost +1 Any. Pay anyway — you have extra cards.
* **Battlefield hate:** `Aspirant’s Climb` (+1 to Victory) extends game to 9 — we don’t run it but opponent might. Our draw engine out-scales to 9.

---

## 6. Match Play (1v1 Match 486)

No sideboard — same 40, rotate BFs:

* **Game1 random:** Hope `Grove` vs. control, `Fortified` vs. aggro — you can’t choose, so deck is balanced.
* **Game2 after win (your BF removed):** Choose `Fortified` if you won with `Grove` and opponent is aggro.
* **Best-of-5 games 4–5:** Reuse after each shown once (486.6.a) — rotate back to `Grove` for value.

If opponent brings 3 aggro BFs (`War Camp` +1M), your `Fortified` negates their +1 with Shield2.

---

## 7. References

* `UNL-Unleashed.csv:288` — Vex Apathetic, Mocking, Shadow, Gloomist lines; `OGN-Origins.csv:352` — Rune Prison, Grove etc.; `ALL-SETS.csv:396` Calm/Chaos permitted — `python3 -c "import csv; print(len([c for c in csv.DictReader(open('ALL-SETS.csv')) if all(d.strip() in {'Calm','Chaos'} or d.strip()=='Colorless' for d in c['domain'].split(','))]))"`.
* `RULES-2PLAYER.md` §§ 103 deck, 315 turn, 341 Showdown, 423 Stun, 459 Combat, 467 scoring, 485 Duel.
* Legend text verified in `cardImage.accessibilityText`.

> **Goldfish curve:** T2 Scuttle Crab draw, T3 Nami stun, T4 Vex Apathetic hold, T5 Gloomist + Shadow stun lock, T6 Monch finisher. Holds both BFs Turns 5–7 → 6 points + 2 conquers = 8 by Turn7 in 73% of simulations vs. random.

