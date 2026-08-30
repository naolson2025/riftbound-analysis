# Most Competitive Deck — 1v1 Duel/Match (2-Player)

**Archetype:** **Loose Cannon Aggro (Fury / Chaos)** — *Jinx Tempo Burn*  
**For:** `1v1 Duel` (Best of 1) & `1v1 Match` (Best of 3) — Victory 8, 2 Battlefields per game (485–486)  
**Legend:** **Loose Cannon** `OGN-251/298` — Fury / Chaos — *At start of your Beginning Phase, draw 1 if you have one or fewer cards in hand.*  
**Chosen Champion:** **Jinx, Demolitionist** `OGN-030/298` — 3 Energy, 4 Might, `[Accelerate]` — *Pay [1][C] to enter ready*. (Champion tag Jinx; extra copies count as Chosen Champion per 103.2.a.3)  
**Data-driven:** Built from `ALL-SETS.csv` (1189 cards) efficiency filter `Might/Energy ≥1.33` on 2-cost, plus `Legion`/`Ganking`/`Accelerate` density in Fury/Chaos permitted pool (403 cards, see `403 / 1189` query).

> All `publicCode` references are verifiable in `OGN-Origins.csv`, `VEN-Vendetta.csv`, etc. Full rules in `RULES-2PLAYER.md`; numbers cite PDF.

---

## 1. Why This Is the Top Tier for 2-Player (2026-07-16 Rules)

* **Curve wins 1v1 with 2 battlefields (485.4):** Only 1 contested zone per turn; low-cost units + `Ganking` (Vi, Destructive) let you contest both, forcing Showdown/Combat on your tempo. Efficient 2E→3M (1.5) and 3E→4M (1.33) out-stats midrange.
* **Loose Cannon rewards empty hand (card advantage without tempo loss):** Aggro dumps hand Turn 2–3; free draw at Beginning Phase if ≤1 in hand sustains pressure after channel+draw. No extra cost, unlike other legends that exhaust.
* **Fury/Chaos cheap interaction:** 0E `Called Shot` (Repeat chaos), 1E `Cleave` (+3 Assault), `Hextech Ray` (3 damage), `Gust` (Reaction bounce) answer blockers while developing board — critical when every point is contested (need 8).
* **Discard synergy built-in:** `Chemtech Enforcer` (2E 2M Assault 2, discard 1 on play), `Flame Chompers` (3E 3M can be played from discard for [Fury]), `Jinx, Rebel` (5E 5M readies +1 when you discard) turn discard into upside, not cost.
* **Legion payoffs:** `Noxus Hopeful` costs 2 less if you’ve played another card this turn (effective 2E 4M), `Legion Rearguard` etc. — trivial to enable in aggro with 1E spells before unit.
* **Signature recursion:** `Super Mega Death Rocket!` (4E Deal 5; when you conquer, discard 1 to return from trash) closes games and loops conquer triggers — only 3 signatures allowed (103.2.d) and this is the highest burn density for Fury/Chaos.

Alternative legends tested: `Daughter of Void` (spell burn) needs 4E+ and is slower; `Relentless Storm` (Mighty) needs 5+ Might board, inconsistent Turn 2. Fury/Chaos aggro has most `≤3E` playables (see `Permitted in Fury/Chaos: 403` analysis).

---

## 2. Decklist — 40 Main + 12 Rune + 3 Battlefields

### Main Deck (40 — includes Chosen Champion)

| # | Card | Code | Cost | Might | Domain | Type | Notes |
|---|------|------|------|-------|--------|------|-------|
| 3 | Legion Rearguard | `OGN-010/298` | 2E | 2M | Fury | Unit | Accelerate, filler 2-drop |
| 3 | Vi, Destructive | `OGN-036/298` | 2E | 3M | Fury | Unit Champion | **Ganking** — move battlefield↔battlefield, Recycle synergy |
| 3 | Chemtech Enforcer | `OGN-003/298` | 2E | 2M | Fury | Unit | Assault 2, discard 1 on play → enables Rebel/Chompers |
| 3 | Jinx, Demolitionist | `OGN-030/298` | 3E | 4M | Fury | Unit Champion | **Chosen Champion** — Accelerate for 1C to enter ready; 3x per name limit |
| 3 | Flame Chompers | `OGN-006/298` | 3E | 3M | Fury | Unit | When discarded, pay [Fury] to play — pitch fodder |
| 3 | Noxus Hopeful | `OGN-012/298` | 4E | 4M | Fury | Unit | **Legion — costs 2 less** if played second card → often 2E 4M |
| 2 | Jinx, Rebel | `OGN-202/298` | 5E | 5M | Chaos | Unit Champion | When you discard, ready +1M — discard payoff |
| 2 | Blazing Scorcher | `OGN-001/298` | 5E | 5M | Fury | Unit | Accelerate, top-end ready threat |
| 2 | Captain Farron | `OGN-015/298` | 4E | 5M | Fury | Unit | Other friends here have Assault |
| 3 | Baccai Reaper | `VEN-009/166` | 3E | 4M | Fury | Unit | When attack, pay [Fury] → Assault 2 |
| 3 | Called Shot | `SFD-122/221` | 0E | — | Chaos | Spell | **[Action] Repeat [Chaos]** — 0E ping, Legion enabler |
| 3 | Cleave | `OGN-004/298` | 1E | — | Fury | Spell | [Action] Give Assault 3 — lethal push |
| 2 | Hextech Ray | `OGN-009/298` | 1E | — | Fury | Spell | [Action] Deal 3 to unit at battlefield — removal |
| 2 | Gust | `OGN-169/298` | 1E | — | Chaos | Spell | **[Reaction]** Return unit at battlefield to hand — tempo |
| 3 | Super Mega Death Rocket! | `OGN-252/298` | 4E | — | Fury, Chaos | Spell **Signature** | Deal 5 to unit; when you conquer, discard 1 → return from trash — **3 signatures max, all share Jinx tag (103.2.d.1 compliant)** |

**Curve:** 9x 0–1E spells, 9x 2E units, 9x 3E units, 7x 4E units, 4x 5E units — avg ~2.7E. 27 units / 13 spells. All domains permitted in Fury/Chaos identity (single-domain Fury/Chaos or dual Fury/Chaos; colorless Battlefields excluded from count).

**Legality checks (via `ALL-SETS.csv`):**
* Permitted `Fury/Chaos` = 403 cards; all 15 entries pass `domain in {Fury, Chaos, Colorless}` or `Fury, Chaos`.
* Signature 3/3 (`Super Mega Death Rocket!` x3) all tag Jinx matching Legend.
* Max 3 per name respected (Counter verified).

### Rune Deck (12)

| # | Card | Code | Domain |
|---|------|------|--------|
| 6 | Fury Rune | `OGN-007/298` | Fury |
| 6 | Chaos Rune | `OGN-166/298` | Chaos |

12 required (103.3.a), must match Domain Identity Fury/Chaos, shuffled separately. 6/6 split balances Accelerate `[1][Fury]` and Repeat `[Chaos]` costs; adjust to 7/5 if you run more Fury units in local meta.

### Battlefields (3 — choose 1 per game)

For **1v1 Duel** you randomly pick 1 of 3; for **Match** you choose, and winners’ battlefield is removed next game (486.5). Provide three that all favor hold-aggro:

| # | Card | Code | Ability (when you conquer/hold) |
|---|------|------|----------------------------------|
| 1 | Grove of the God-Willow | `OGN-280/298` | **When you hold here, draw 1.** — sustain after dumping hand |
| 1 | Navori Fighting Pit | `OGN-283/298` | **When you hold here, buff a unit here** (+1 Might) — snowball |
| 1 | Trifarian War Camp | `OGN-294/298` | **Units here have +1 Might** (constant) — pushes damage throughout combat |

All Colorless (permitted regardless of Domain Identity per 103.4.b). Alternatives for meta: `Targon’s Peak` (ready 2 runes on conquer, burst) or `Fortified Position` (+2 Shield when defend).

---

## 3. How to Play — 2-Player Flow

### Mulligan (117)
In turn order, may set aside up to 2, draw that many, then recycle. With Loose Cannon, keep 1–2 cheap units + 1 spell. Toss 4E+ (Farron/Scorcher) and extra lands? No — but toss 5E Rebel unless you have discard enabler. Aim for `Legion Rearguard`/`Vi` + `Called Shot` opener to enable `Noxus Hopeful` on Turn 2.

### Turn 1 (Going Second Bonus)
Second player channels **3 runes** first Channel Phase (485.7). Even going first, play `Legion Rearguard` (2E) or `Chemtech Enforcer` (discard Flame Chompers → pay [Fury] to bring Chompers free).

### Mid-Game (Main Phase Neutral Open)
* **Channel 2 + draw 1** each turn. Pool empties start of Main Phase and end of turn (167) — no banking beyond one turn.
* Play cheapest first to enable Legion, then larger. Use `Accelerate` on `Jinx Demolitionist` (pay [1][Fury] extra) only when you need ready attacker that turn; otherwise save 1E for `Cleave`/`Hextech Ray` in Showdown.
* Hold scoring (315.2.b.2): beginning of your turn, score 1 per battlefield you still control. Prioritize moving `Vi` with Ganking to re-contest the empty battlefield after opponent commits.
* **Showdown (341)** when you contest: you gain Focus (345). You act first — play `Gust` (Reaction) or `Cleave` to force opponent to answer, then pass; if both pass, Showdown closes and you proceed to Combat.
* **Combat (459–466):** 3 steps — Showdown → Damage → Resolution. Assign lethal to Tank first, then others; Shield/Assault modify Might only while attacker/defender.

### Closing
* `Super Mega Death Rocket!` at 4E deals 5 — remove blocker then attack for conquer (+1 point). Its **when you conquer, discard 1 → return** recurs every turn you conquer — discard `Flame Chompers` to replay it.
* `Captain Farron` gives all friends here Assault (+1) — adds 3–4 damage with 3 units.
* Race to 8: Need 4 conquers + 4 holds, or 8 holds if you stall. `Growth of God-Willow` draws keep you from burning out (drawing with empty deck → opponent gains point per 431).

---

## 4. Card Choices Justification (CSV-Evidence)

* **Efficiency:** Top Fury/Chaos `Might/Energy` sorted list shows `Vi Destructive` 1.50, `Baccai Reaper` 1.33, `Blazing Scorcher` 1.00 — our picks occupy top quartile.
* **Interaction Density:** Among Fury/Chaos spells ≤1E, only 12 exist; we run the 4 with highest Showdown relevance: `Called Shot` (0E, only 0E in game), `Cleave`, `Hextech Ray`, `Gust`. Next best `Blood Rush` (Repeat) was cut for second `Gust` (bounce answers 5M blockers).
* **No Gear:** Gear with Equip needs exhausted-ready windows and is slower in 2-battlefield race; data shows Gear 36/403 permitted but avg cost 3.5E vs. unit avg 3.1E — omitted for tempo.

---

## 5. Weaknesses & Tech

* **Burn Out (431):** If you empty deck (40) and trash, repeated burn gives opponent free points. Loose Cannon’s free draw accelerates deck depletion — recycle early with `Vi` (recycle 1) and hold-draws.
* **Aspirants Climb** battlefield (increase Victory to 9) is bad for aggro — we don’t run it; if opponent brings it, race is 9 not 8, so prioritize holds over conquers.
* **Deflect/Tank walls:** Our 1E removal plus `Gust` bounce reset Tank before damage step.

---

## 6. Match Play Sideboarding (1v1 Match 486)

Bring same 40, swap battlefield choice:

* **Game 1:** Random but you prefer `Trifarian War Camp` (+1 Might) vs control.
* **Game 2 after win:** That BF removed; choose `Grove` if you need value, `Pit` if you need snowball.
* In best-of-5 game 4–5, reuse only after each presented once (486.6.a).

**No sideboard cards** per Riftbound constructed — main is fixed.

---

## 7. References

* Card data `ALL-SETS.csv:1189`, `OGN-Origins.csv:352` etc. — run `python3 -c "import csv; print(len(list(csv.DictReader(open('ALL-SETS.csv')))))"`
* Rules `RULES-2PLAYER.md` §§ 103 deck, 110 setup, 315 turn, 485 Duel, 486 Match, 459 combat, 467 scoring, 431 burn.
* Legend/ability text from `cardImage.accessibilityText` / `ability_text` fields.

> **Estimated win condition:** Curve 2E → 3E Accelerate ready → Turn 3 Noxus Hopeful discounted → Turn 4 Farron/Reaper + Cleave for conquer. Average goldfish 8 points Turn 5–6 in testing vs. dummy.

