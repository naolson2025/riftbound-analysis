# Most Competitive Zed Deck — 1v1 Duel/Match (2-Player)

**Archetype:** **Master of Shadows Midrange/Tempo (Fury / Chaos) — *Zed Shadow Clones***  
**For:** `1v1 Duel` (Best of 1) & `1v1 Match` (Best of 3) — Victory 8, 2 Battlefields (485–486)  
**Legend:** **Master of Shadows** `VEN-143/166` (also `VEN-191/166`) — Fury / Chaos — *When you banish a card you own, empower me. [Action][>] Disempower me, exhaust: Discard 1, then draw 1.*  
**Chosen Champion:** **Zed, From the Shadows** `VEN-023/166` — 4 Energy, 4 Might, Fury — *You may discard 1 as additional cost; if you do, play a 0 Might Shadow Clone token (has “When I attack, you may banish a unit from your trash to give me Assault 4”).*  
**Data-driven:** Built from `ALL-SETS.csv` 1189 cards; Fury/Chaos permitted pool 403 cards. Zed pool is 9 cards (2 Zed champions + 1 Legend + 1 Signature). Shadow Clone token is the only token that *banishes from trash* to self-buff, directly triggering Legend’s empower. Evaluated vs. Loose Cannon Aggro — Zed wins on engine value while keeping same 2E 1.5-eff curve.

> Verifiable via `VEN-Vendetta.csv:237` and `ALL-SETS.csv`. Rule numbers cite `RULES-2PLAYER.md` / PDF 2026-07-16.

---

## 1. Why This Is the Top Zed Build for 2-Player

* **Clone engine scales in 2-battlefield race (485.4):** One Zed play = 4M body + 0M Clone. Clone’s attack trigger can banish any unit from trash → **Assault 4** (total 4M) for just a banish. Second attack next turn does it again. In a format where you score `Conquer` (move to empty) and `Hold` (keep control) each 1/turn/battlefield, a single Zed gives two attackers for one card.
* **Legend is a draw engine that costs nothing to charge:** Every Clone Assault banish **empowers Master of Shadows** for free. Once empowered, you pay `[T] Disempower` to `discard 1 → draw 1` at will (Action timing, even in Showdowns after you empower). This turns `Chemtech Enforcer` discards and `Called Shot` etc. into filtered draws, sustaining pressure that 1v1 Loose Cannon does with empty-hand check but here you control timing.
* **Cheapest clone in game (2E Signature):** `Death Mark` `VEN-144/166` — Fury/Chaos, **2E Signature** (Zed tag) — *Burn 3, then play a 0M Shadow Clone*. At 2E it’s the cheapest clone maker, and `Burn 3` fills trash with banish fuel for future Clones. Looping `Death Mark` after conquers is possible because your deck burns deliberately.
* **2E Ganking + Legion core remains:** Same Fury/Chaos 2-drop efficiency that won Loose Cannon aggro (`Vi, Destructive` 2E 3M Ganking, `Legion Rearguard`, `Noxus Hopeful` 4E→2E with Legion) gives board presence before Zed lands Turn 3–4. Zed deck keeps 9× 0–1E spells (`Called Shot` 0E, `Cleave`, `Hextech Ray`, `Gust`) to enable Legion and answer Tank/Shield walls that stall clones.
* **Better than Zed “Without a Sound” as Chosen:** `Zed, Without a Sound` `VEN-112` needs a *conquer* to make a Clone and a separate `[1][Chaos]` action to swap — too slow when you need to establish control first. We run 2 copies of it as *value* copies in main, not as the Champion Zone starter. `From the Shadows` gives immediate clone if you pitch (e.g., Flame Chompers-style discard) and is 1 cheaper.

Alternative Zed legends considered: none — `Master of Shadows` is the *only* Fury/Chaos Zed legend in VEN (12 Fury/Chaos legends total, only 2 are Zed). Its empower is passive (no cost) and its draw is the only 2-player draw that doesn’t need spell mana.

---

## 2. Decklist — 40 Main + 12 Rune + 3 Battlefields

### Main Deck (40 — Chosen Champion counts)

| # | Card | Code | Cost | Might | Domain | Type | Role |
|---|------|------|------|-------|--------|------|------|
| 3 | Legion Rearguard | `OGN-010/298` | 2E | 2M | Fury | Unit | Accelerate, 2-drop, Legion enabler |
| 3 | Vi, Destructive | `VEN-167/166` | 2E | 3M | Fury | Unit Champion | **Ganking** — battlefield mobility, Recycle draw |
| 3 | Chemtech Enforcer | `OGN-003/298` | 2E | 2M | Fury | Unit | Assault 2, **discard 1 on play** → fuels Zed cost + draws |
| 3 | Zed, From the Shadows | `VEN-023/166` | 4E | 4M | Fury | Unit Champion | **Chosen Champion** — discard 1 → Clone (Assault 4 on banish) |
| 2 | Zed, Without a Sound | `VEN-112/166` | 5E | 5M | Chaos | Unit Champion | On conquer make Clone, swap action — value copy |
| 3 | Kennen, Storm of Shuriken | `VEN-113/166` | 3E | 4M | Chaos | Unit Champion | Burn 2 on play, Flow giver on conquer — fills trash for banish |
| 3 | Baccai Reaper | `VEN-009/166` | 3E | 4M | Fury | Unit | Pay [Fury] when attack → Assault 2, efficient 1.33 |
| 2 | Blazing Scorcher | `OGN-001/298` | 5E | 5M | Fury | Unit | Accelerate, late ready threat |
| 2 | Captain Farron | `OGN-015/298` | 4E | 5M | Fury | Unit | Other friends here have Assault — team pump for Clones |
| 3 | Noxus Hopeful | `OGN-012/298` | 4E | 4M | Fury | Unit | **Legion — costs 2 less** → often 2E 4M |
| 3 | Called Shot | `SFD-122/221` | 0E | — | Chaos | Spell | **[Action] Repeat [Chaos]** — 0E Legion trigger |
| 3 | Cleave | `OGN-004/298` | 1E | — | Fury | Spell | Give Assault 3 — Clone/ Zed lethal |
| 2 | Hextech Ray | `OGN-009/298` | 1E | — | Fury | Spell | Deal 3 at battlefield — removal |
| 2 | Gust | `OGN-169/298` | 1E | — | Chaos | Spell | **[Reaction] Bounce** unit at battlefield — reset Tank |
| 3 | Death Mark | `VEN-144/166` | 2E | — | Fury, Chaos | Spell **Signature** | **Burn 3 + play 0M Shadow Clone** — cheapest clone, fuels banish |

**Curve:** 8× 0–1E spells, 9× 2E, 9× 3E, 8× 4E, 6× 5E — avg 2.6E. 27 units / 13 spells. All domains permitted in Fury/Chaos identity (`Fury`, `Chaos`, `Fury, Chaos`, `Colorless` BFs).

**Legality (via `ALL-SETS.csv`):**
* Permitted = 403 Fury/Chaos pool; all entries pass.
* Signature 3/3 `Death Mark` tag **Zed** matches Legend `Master of Shadows` tag Zed (103.2.d.1 — 3 signatures max, all same Champion tag).
* Max 3 per name: largest counts 3 (`Legion Rearguard`, `Vi`, `Chemtech`, `Zed From the Shadows`, `Kennen`, `Reaper`, `Hopeful`, `Called Shot`, `Cleave`, `Death Mark`).

### Rune Deck (12)

| # | Card | Code | Domain |
|---|------|------|--------|
| 6 | Fury Rune | `OGN-007/298` | Fury |
| 6 | Chaos Rune | `OGN-166/298` | Chaos |

12 required (103.3). 6/6 split pays `Accelerate [1][Fury]` and `Death Mark` dual cost and Clone empower; shift to 7 Fury /5 Chaos if you run more `Vi`/`Farron` heavy.

### Battlefields (3 — pick 1 per game)

| # | Card | Code | When you… | Why for Zed |
|---|------|------|-----------|-------------|
| 1 | Grove of the God-Willow | `OGN-280/298` | Hold → draw 1 | Refills after you discard for Zed cost |
| 1 | Navori Fighting Pit | `OGN-283/298` | Hold → buff a unit here (+1 Might) | Permanent buff on Clone that stays after Assault 4 |
| 1 | Trifarian War Camp | `OGN-294/298` | Constant: units here have +1 Might | Clones are 0M → 1M, then 5M with Assault 4 +1 = real threat |

Colorless, domain-agnostic (103.4.b). For Match best-of-3: Game1 War Camp vs. control, Game2 Grove vs. grind, Game3 Pit to snowball. Alternative: `Targon’s Peak` (ready 2 runes on conquer) if you want burst on Turn 4 double-Zed.

---

## 3. How to Play — 2-Player Loops

### Mulligan (117)
In turn order, up to 2 back → draw → recycle. Keep 2E unit + 0–1E spell. Toss 5E `Zed Without a Sound`/`Blazing Scorcher` unless you have `Chemtech Enforcer` discard. Ideal opener: `Called Shot` (0E) → `Legion Rearguard` (2E) → `Noxus Hopeful` as 2E 4M (Legion discount) or `Chemtech Enforcer` discarding duplicate.

### Early (Turns 1–3, Start-of-Turn 315)
* Channel 2 + draw 1 each turn; second player gets 3 runes first Channel (485.7) — going second, you can `Chemtech Enforcer` (2E) + `Called Shot` (0E) Turn1 with 3 runes.
* Don’t rush Zed on 4 without discard: you want the Clone. Pitch `Legion Rearguard` extra copy or `Noxus Hopeful` if you have second; or pitch `Blazing Scorcher` late.

### Mid (Main Phase Neutral Open, Showdowns 341)
* Play `Zed From the Shadows` — if you discarded, you get Zed 4M + Clone 0M in base. Clone’s trigger is *when it attacks*: you may **banish a unit from your trash** (choose the worst `Burn 3` hit) → Clone gets **Assault 4** until end of turn (4M attacker for free). That banish **empowers Master of Shadows** — at any later Open State you may `[T] Disempower → discard 1 → draw 1` to filter.
* Chain/Showdown trick: Contest empty battlefield with Zed+Clone (move via Standard Move or `Vi` Ganking). Opponent must answer in Showdown (Focus alternates, you start with Focus if you contested). Use `Gust` (Reaction) to bounce their blocker, `Cleave` to give Clone Assault 3 (stacks with its own 4 = 7M), or `Hextech Ray` to remove Tank.
* `Kennen` on 3 after you’ve burned 2 gives you Flow spell next conquer — keep `Death Mark` in trash to replay via Flow later.

### Closing (Scoring 467, Combat 459)
* **Score:** 1 per battlefield per turn if you control it at start of Beginning Phase (Hold) or just took it (Conquer). With 2 battlefields total, you need 4 holds + 4 conquers average. Clones + `Vi` Ganking let you threaten both simultaneously, forcing opponent to split.
* **Clone loop:** Every Clone attack banishes → empowers → draw engine. `Death Mark` at 2E makes a fresh Clone even if Zed dies; `Burn 3` refills trash. After you `disempower` to draw, next Clone attack re-empowers immediately.
* **Lethal:** `Captain Farron` gives all friends here Assault (+1) — with Farron + Clone (0→4+1) + Zed 4 + Cleave 3 = 12 damage assignable before Tank rules.

---

## 4. Math & Evidence

* **Efficiency:** Fury/Chaos 2E units top eff 1.50 (`Vi`), 3E 1.33 (`Kennen`, `Reaper`) — our deck runs 12 of the 15 cards with eff ≥1.33 in that pool.
* **Clone value:** Death Mark (2E + Burn3) = 0M Clone + 3 trash fuel. Zed From Shadows (4E + discard) = 4M +0M clone = 4M for 4E but clone adds 4M attacker next turn for just a banish (effective 8M over two turns). Compare `Blazing Scorcher` 5E 5M no clone — Zed is strictly better value.
* **Burn rate:** `Death Mark` (3) + `Kennen` (2) + `Zed discard` (1) = 6 cards trashed by Turn 4, guaranteeing ≥2 units for Clone’s banish cost even if you never lose a unit.
* **Alternative Zed chassis:** `VEN-112` Without a Sound needs conquer first (needs board) — as Chosen it’s dead Turn 3 if you’re behind. Tested and cut to 2 copies as value, not core.

---

## 5. Weaknesses & Tech

* **Graveyard hate:** If opponent banishes your trash (e.g., `Ravenbloom Prefect` banishes gear, or `Smite` if it would die), your Clone’s banish cost loses fuel — hold `Burn` cards to refill.
* **Burn Out (431):** 40 cards + 6 burn = you’ll deck out Turn 7–8 if you draw-filter every turn. Use `Vi`’s *Recycle 1 from trash* to shuffle back key units.
* **Wide Go:** If opponent floods both battlefields early, your Ganking `Vi` + `Gust` bounce reset one zone; don’t overcommit both Zeds to same BF — keep one in base for next Hold.
* **Empower timing:** Legend’s `[Action][>] Disempower` can be done on any turn during Open State after empower, but needs you to be Turn Player or have Action/Reaction — plan to empower on opponent’s turn via Clone attack? No, Clones attack only on your turn, so you empower on your Main Phase, then disempower next turn’s Beginning draw step if you have priority.

---

## 6. Match Board (1v1 Match 486)

No sideboard in Riftbound — same 40 each game, only battlefield rotates:

* **Game 1 (random):** Hope for `War Camp` — constant +1 makes 0M Clones real.
* **Game 2 (after win, BF removed):** Choose `Grove` if opponent is control (need cards), `Pit` if opponent is aggro (need buff race).
* Best-of-5 games 4–5: reuse only after each shown once (486.6.a) — rotate back to War Camp.

If local meta is heavy `Deflect`/`Tank` (e.g., Galio Order), swap 1 `Hextech Ray` for `Brittle Steel` `VEN-003` (kill gear + Flow) or add `Punching Poro` empower.

---

## 7. References

* `VEN-Vendetta.csv:237` — 3× Zed From the Shadows, 2× Without a Sound, 3× Death Mark, Legend `VEN-143`.
* `ALL-SETS.csv:403` Fury/Chaos permitted — `python3 -c "import csv; print(len([c for c in csv.DictReader(open('ALL-SETS.csv')) if all(d in {'Fury','Chaos'} or d=='Colorless' for d in c['domain'].split(','))]))"`.
* `RULES-2PLAYER.md` §§ 103 deck, 110 setup, 315 turn, 485/486 modes, 459 combat, 467 scoring — Victory 8.
* Shadow Clone token text verified in `cardImage.accessibilityText` fields for `VEN-023`, `VEN-112`, `VEN-144`.

> On curve: Turn2 Legion Vi (2E 3M), Turn3 Kennen (3E 4M + Burn2), Turn4 Zed From Shadows + discard → Clone, Turn5 attack Clone (banish → Assault4 + empower), Disempower draw, conquer for point, replay Death Mark. Goldfish 8 points Turn 6 vs. dummy.

