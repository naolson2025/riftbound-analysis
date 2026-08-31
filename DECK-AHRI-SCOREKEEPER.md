# FOXHOLE — Nine-Tailed Fox Calm/Mind Scorekeeper Control

**Format:** 2-Player Duel / Match (Victory Score 8, 2 battlefields)
**Legend:** Nine-Tailed Fox (Ahri) — Calm / Mind
**Chosen Champion:** Ahri, Alluring
**Archetype:** Defensive board-control that scores *more points per battlefield than is normally possible* while denying the opponent the ability to score at all.

Built only from `ALL-SETS.csv` and `RULES-2PLAYER.md`.

---

## 0. The Cost Model This Deck Is Built On

This matters more than anything else in deckbuilding, so it goes first.

A cost written `[5][Calm]` means:

- **Energy (`[5]`) — exhaust 5 ready runes.** Any domain. They untap in your next Awaken Phase, so this is a renewable, per-turn resource.
- **Power (`[Calm]`) — recycle 1 Calm rune.** That rune leaves your base and is shuffled back into your Rune Deck. An already-exhausted rune can be recycled, so the recycled rune may be one of the five you just exhausted.

Both must be paid. So the number of runes you need to *have* is `max(energy, power)`, which is the energy number for essentially every card — but **power symbols permanently shrink your board**.

That gives one governing equation for the whole deck:

```
net rune growth per turn  =  +2 (Channel Phase)  −  (power symbols you spent)
```

Spend three power symbols in a turn and you go *backwards* on mana. This is why the entire pool tops out at 12 energy: 12 is the size of a Rune Deck, and the only way to have 12 runes in your base is to have never paid a power cost in your life.

Two consequences drive every card choice below:

1. **A zero-power card is dramatically better than its energy cost suggests.** `Falling Comet [5]` costs five *rentals*. `Charm [1][Calm]` costs one rental plus one rune you never get back — in real terms Charm is the more expensive card.
2. **Double-power cards are big commitments,** and you can only afford a couple of them across a game. This deck plays exactly two names with `[C][C]` costs, and both of them win the game on their own.

The build below runs **0.60 power symbols per card, half the deck at zero power, and two Seal of Focus that generate Calm Power for free every turn.** Against +2 channelled per turn, that keeps net rune growth comfortably positive while still casting a 7-drop.

---

## 1. The Thesis — Why This Is the Best Deck

### The format is a race to 8, and there are only three ways to move the number

Per the rules (§10), you score exactly one way: **Conquer** (take an uncontrolled battlefield) or **Hold** (start your Beginning Phase controlling one). Both are hard-capped at **once per battlefield per turn per player** (470). With only **2 battlefields** in a 2-player game, the rules-legal ceiling for a normal deck is **2 points per turn**. From zero, that is a minimum four-turn scoring window, and realistically six-plus because you have to fight for both battlefields at once and then keep them.

So there are exactly three levers that beat a "normal" deck:

1. **Break the 2-point ceiling** — score points from card text, which is not subject to the once-per-battlefield limit.
2. **Set the opponent's ceiling to zero** — stop them scoring entirely.
3. **Never lose the board** — because both of the above require units standing on battlefields at your Beginning Phase.

Calm + Mind is the only domain identity in the pool that does all three, and it is exactly the identity of the Ahri legend, whose own text is a free permanent tax on every attack made against you.

### Lever 1 — Break the ceiling

```
Ahri, Alluring    [5][Calm]  4 Might  —  "When I hold, you score 1 point."
Blue Sentinel     [4][Mind]  4 Might  Shield 2
                              "Your hold effects for holding here trigger an additional time."
```

Ahri's point is a **triggered ability**, not the rules-based Hold score, so rule 470's cap does not apply to it. A battlefield with Ahri on it produces **2 points per turn instead of 1**.

Add Blue Sentinel to the same battlefield and Ahri's trigger fires twice:

| Source | Points |
|---|---|
| Rules-based Hold (capped) | 1 |
| Ahri trigger | 1 |
| Ahri trigger, duplicated by Blue Sentinel | 1 |
| **Total, one battlefield, one turn** | **3** |

Hold the second battlefield with anything at all and you are at **4 points per turn** — double the theoretical maximum of every other deck in the format. Two clean upkeeps wins.

Critically, **this engine costs almost nothing to run.** Ahri and Blue Sentinel are one power symbol each, paid once, and then they generate points every turn for free. Compare the alternatives I checked: Renata Glasc, Mastermind wants `[4][Mind][Mind][Mind][Mind]` — four recycled runes — for *every single point*, which under the real cost model is close to unplayable. Nasus, Ascended needs 8 energy and then an 8-energy Empower. Bottled Constellation eats three of your own permanents per point. Ahri asks for nothing except that she stands where she already wants to stand.

### Lever 2 — Set their ceiling to zero

```
Tianna Crownguard  [7][Calm][Calm]  4 Might  Deflect
                   "While I'm at a battlefield, opponents can't score points."
```

In a format whose only win condition is accumulating 8 points, a resident unit reading "opponents can't score points" is a **lock**, not a tempo play. It ignores board state, combat maths, and how far ahead they are.

Her **Deflect** is much stronger than it looks under the real cost model: every removal spell aimed at her costs an extra rainbow Power, which means **they permanently lose a rune to target her**. Killing Tianna is not just a card, it is a lasting hit to their mana base.

She is the most expensive card here — 7 exhausted plus 2 recycled — so she is the *long-game* card, not the opener. Ahri is the plan; Tianna is what closes out a game that goes past turn six.

### Lever 3 — Never lose the board

- **Nine-Tailed Fox (the legend):** *"When an enemy unit attacks a battlefield you control, give it -1 Might this turn."* Free, permanent, no exhaust, no cost. Every attacker they send is a worse attacker, forever.
- **Alpha Wildclaw** `[6][C][C]` 7 Might Tank — *"Your units here with less Might than me can't be chosen by enemy spells and abilities."* Ahri is 4. Blue Sentinel is 4. Tianna is 4. **All three become completely immune to targeted removal**, and Tank forces all combat damage into the 7-Might body first.
- A wall of Shield/Tank bodies that defend well above their printed Might, all at **zero power cost**, so holding the board never taxes your rune base.

### Why not the alternatives

| Considered | Why it loses |
|---|---|
| Fury/Chaos or Fury/Body aggro | Capped at 2 points/turn. Must break Tank + Shield + the legend's -1 Might tax, and a perfect curve is still a turn behind the Ahri engine. |
| Body/Order Sett or Garen buff-swarm | Also capped at 2/turn, and folds to Fox-Fire, which kills any number of units totalling 4 Might for `[3]` and **zero power**. |
| Mind/Order Viktor or Order Recruit tokens | Makes 1-Might bodies, the exact thing Fox-Fire erases. |
| Calm/Order Leona stun | Solid defensively, no way to break the 2-point ceiling. Loses the long game to a deck scoring double. |
| Shurima/Fury "fewer runes" package | Genuinely rewarded by the recycling economy, but still capped at 2 points/turn. Faster, not higher. |

Every other deck in this pool plays for tempo. This one plays directly on the scoreboard.

---

## 2. Decklist

### Legend & Battlefields

```
LEGEND       Nine-Tailed Fox            (Calm/Mind, tag: Ahri)
BATTLEFIELD  Grove of the God-Willow    "When you hold here, draw 1."
BATTLEFIELD  Startipped Peak            "When you hold here, you may channel 1 rune exhausted."
BATTLEFIELD  Hallowed Tomb              "When you hold here, you may return your Chosen Champion
                                          from your trash to your Champion Zone."
```

Blue Sentinel doubles all three: **Grove draws 2, Startipped Peak channels 2.** Startipped Peak is specifically here to fight rune attrition — two extra runes per turn on top of your Channel Phase is what pays for Tianna and Alpha Wildclaw.

### Main Deck — 42 cards

`[E]` = runes to exhaust. `[C]`/`[M]` = Calm/Mind runes to **recycle** (gone from your base).

**Units — 22**

| # | Card | Cost | Pwr | Might | Role |
|---|---|---|---|---|---|
| 3 | **Ahri, Alluring** | `[5][C]` | 1 | 4 | The engine. +1 point per hold. *One copy is the Chosen Champion.* |
| 3 | **Blue Sentinel** | `[4][M]` | 1 | 4 | Doubles Ahri and both battlefields. Shield 2 = 6-Might defender. |
| 3 | **Mutated Mouser** | `[2]` | **0** | 1 | Shield 2 + Tank. Defends as 3 and must be killed first. |
| 3 | **Sunlit Guardian** | `[3]` | **0** | 3 | Shield + Tank. Defends as 4. Your standard battlefield claim. |
| 2 | **Lecturing Yordle** | `[3]` | **0** | 2 | Tank that replaces itself — draw 1 on play. |
| 2 | **Taric, Protector** | `[4][C]` | 1 | 4 | Shield + Tank, and grants Shield to everything else there. |
| 2 | **Sona, Harmonious** | `[4][C]` | 1 | 4 | **Readies 4 runes at end of your turn.** Your mana engine. |
| 2 | **Alpha Wildclaw** | `[6][C][C]` | 2 | 7 | Tank. Makes Ahri, Tianna and Blue Sentinel untargetable. |
| 2 | **Tianna Crownguard** | `[7][C][C]` | 2 | 4 | Deflect. **Opponents can't score points.** |

**Spells & Gear — 20**

| # | Card | Cost | Pwr | Role |
|---|---|---|---|---|
| 3 | **Fox-Fire** *(Signature)* | `[3]` | **0** | Hidden, Action. Kill any number of units at a battlefield totalling ≤4 Might. |
| 3 | **Consult the Past** | `[4]` | **0** | Hidden, Reaction. Draw 2. |
| 3 | **Thwonk!** | `[2]` | **0** | Action, Repeat `[2]`. Stun an attacking unit — or two, for `[4]` total. |
| 3 | **Not So Fast** | `[2][C]` | 1 | Reaction. Counter any spell or ability that chooses your unit or gear. |
| 2 | **Seal of Focus** *(Gear)* | `[0][C]` | 1 | **TAP: Add `[Calm]`.** One rune buys a permanent Calm Power engine. See below. |
| 2 | **Falling Comet** | `[5]` | **0** | Action. 6 damage — kills essentially any single threat, for no runes. |
| 2 | **Crescent Strike** | `[3][M]` | 1 | Action. 4 damage to one enemy, 1 to every other enemy there. |
| 2 | **Block** | `[2]` | **0** | Hidden, Action. Give a unit Shield 3 **and** Tank this turn. |

**Totals: 25 power symbols across 42 cards (0.60/card). 21 cards at zero power (50%).**

Note the raw symbol count went *up* by 2 when the Seals came in, because a Seal costs a Calm Power to deploy. That is the correct trade and the raw number is misleading: those 2 symbols are one-time payments that then refund themselves every turn for the rest of the game. Judge the deck on **net rune flow**, not on the printed total.

> **Why Seal of Focus is the best card the corrected rules unlocked.** It costs `[0]` Energy plus one recycled Calm rune — so you pay exactly one rune, once. From then on it taps every turn to **Add `[Calm]` directly to your Rune Pool without exhausting or recycling anything.** It breaks even on its second turn in play and is pure profit forever after. This deck spends 18 Calm Power symbols across a full playset; two Seals cover roughly one to two of them *every turn*, which takes net rune growth from about +0.5/turn to roughly +1.7/turn. That is the difference between casting Tianna Crownguard on turn 5 and never casting her. It also means the Power half of Not So Fast is free on the opponent's turn, so you can hold up interaction without tapping low.

**Rune Deck — 12**

```
8 × Calm Rune
4 × Mind Rune
```

The deck spends 18 Calm symbols to 5 Mind across a full playset, so the split is deliberately Calm-heavy. Mind is only ever needed one symbol at a time (Blue Sentinel, Crescent Strike), and with 4 Mind in 12 you have a ~97% chance of having channelled at least one by your third turn. Calm needs *doubles* for Alpha Wildclaw and Tianna, which is why it gets 8. Recycled runes return to the Rune Deck and get re-channelled, so neither colour ever runs dry.

### Legality check

- ✅ 42 cards ≥ 40 minimum
- ✅ Chosen Champion is Ahri, Alluring — Champion unit, tag **Ahri**, matches the legend, not a Signature card
- ✅ 3 Signature cards total (Fox-Fire ×3), all tagged **Ahri**
- ✅ Every card is mono-Calm, mono-Mind, or Calm/Mind — inside the Domain Identity
- ✅ Max 3 copies of any name
- ✅ 12 runes, all matching the Domain Identity
- ✅ 3 distinct battlefields, no duplicates

---

## 3. How to Pilot It

### The core sequence, with rune accounting

`R` = runes in your base at the start of that turn's Main Phase. Watch how it moves.

```
T1   R=2    Play Mutated Mouser [2].  (0 power)                         R stays 2
T2   R=4    Move Mouser out → CONQUER open battlefield.        +1  →  1
            Play Sunlit Guardian [3] to base.  (0 power)                R stays 4
T3   R=6    Beginning: Hold = +1                               +1  →  2
            Play Ahri [5][C] DIRECTLY onto the battlefield you hold.
                                            exhaust 5, recycle 1   →   R drops to 5
            Move Sunlit Guardian out → CONQUER the second.     +1  →  3
T4   R=7    Beginning: BF1 = 1 + Ahri 1 = 2.  BF2 = 1.         +3  →  6
            Play Blue Sentinel [4][M] onto BF1.
                                            exhaust 4, recycle 1   →   R drops to 6
            2 energy spare — hold up Thwonk! (0 power).
T5   R=8    Beginning: BF1 = 1 + Ahri 1 + Ahri-again 1 = 3.  BF2 = 1.
                                                               +4  →  10   WIN
```

Note the rune line: 2 → 4 → 5 → 6 → 8. It grows even while casting the engine, because Ahri and Blue Sentinel are one power symbol each and the walls are free. **That is the entire reason this build works and a power-heavy version would not.**

Against real resistance this is a turn 6–7 kill, and from the moment Tianna lands the opponent is scoring nothing while you get there.

**The most important sequencing rule:** you may play units directly onto a battlefield **you already control**, but you must *move* a unit from your base to take an uncontrolled one, and units enter **exhausted** (they cannot move the turn they arrive). So deploy walls to your base one turn before you need them to march, and once a battlefield is yours, drop everything else straight onto it.

### Managing the rune economy

This is the skill the deck actually rewards.

- **Budget power symbols, not energy.** Before your turn, count the power symbols in what you plan to cast. Two is a normal turn. Three means you end the turn poorer than you started. Four means you have set yourself back two full turns of channelling.
- **Sona, Harmonious is a mana engine, not a body.** Readying 4 runes at end of turn means those 4 are available again during the opponent's turn for Not So Fast, Meditation and Hidden cards, and then they ready *again* in your Awaken Phase. She effectively adds four energy per turn cycle. She does not replace recycled runes, so she fixes energy, not attrition — but energy is what you run out of first.
- **Startipped Peak, doubled by Blue Sentinel, is +2 runes per turn.** That is the only card in the deck that actually reverses attrition. If you get to choose battlefields (a Match), and the game looks like it will go long, take it.
- **Hidden is a rune conversion, not free value.** Hiding costs `[rainbow]` — one recycled rune — and then the card plays for `[0]`. So hiding Consult the Past turns one rune into "draw 2 at Reaction speed on their turn." That is a fine trade, but it *is* a trade. You control up to 2 facedown zones (one per battlefield you hold), so cap yourself at the ones that matter: Fox-Fire and Block are the best hides because they win combats outright.
- **Their Deflect and Hidden costs hurt them the same way.** Making an opponent pay `[rainbow]` to target Tianna costs them a rune permanently. Deflect in this economy is a mana attack, not just a tax.

### Mulligan

You may set aside up to 2 cards and redraw. You want **a cheap zero-power body plus a way to reach turn 3**.

| Keep | Set aside |
|---|---|
| Mutated Mouser, Sunlit Guardian, Lecturing Yordle | Hands with zero units |
| Blue Sentinel | Second and third copies of Ahri, Alluring |
| One cheap interaction card (Thwonk!, Not So Fast) | Alpha Wildclaw + Tianna together — far too slow to keep both |
| Ahri is in your Champion Zone — never mulligan for her | Any hand needing 3+ power symbols before turn 4 |

Two cheap walls and one interaction spell is a perfect keep. Two 6-drops is a mulligan even though they are your best cards.

### Playing on their turn

Roughly half this deck is meant to be spent while it is not your turn.

- **Thwonk! is your primary anti-aggro card** and it costs no runes. Base `[2]` stuns one attacker; pay the `[2]` Repeat and it stuns two. A stunned unit deals no combat damage, so two attackers are simply deleted from the combat for four energy and zero attrition.
- **Block is a hidden blowout.** Shield 3 *and* Tank on one unit, played from face down for `[0]`, turns a 3-Might wall into a 6-Might defender that must be killed first. It wins combats the opponent has already calculated.
- **Not So Fast only stops things that *choose* your unit or gear** — targeted removal, bounce, steal. It does **not** stop a sweeper like The Ruination, because those don't choose. Accept this: under the real cost model a sweeper like `[9][Order][Order][Order]` requires nine ready runes *and* three recycled, which almost no deck assembles. Paying two extra recycled runes for a catch-all counter is a worse deal than just having more board.
- **Lead with Seal of Focus whenever you have a spare rune early.** It is the only card in the deck that gets better the longer the game runs, and a turn-1 or turn-2 Seal is worth more than a turn-5 one. Never hold it.

### Assembling the lock

The board you are building toward, all on one battlefield:

```
    Alpha Wildclaw (7 Might, Tank)   ← eats all combat damage, makes everything else untargetable
    Ahri, Alluring (4)               ← +1 point per turn
    Blue Sentinel (4, Shield 2)      ← makes it +2
    Tianna Crownguard (4, Deflect)   ← their score is frozen
```

With Alpha Wildclaw down, the other three cannot be chosen by enemy spells or abilities at all, and Tank forces every point of combat damage into the 7-Might body first. To break it they need 7+ damage in one combat *through* Tank, while your legend gives each attacker -1 Might and Taric hands out Shield.

**Priority if you only get one:** Ahri first (she wins the game), Alpha Wildclaw second (she keeps Ahri alive), Tianna third (she buys the turns). Never lead with Tianna into an open board — she is 4 Might and dies immediately without the umbrella, and you will have burned two runes for nothing.

### The second battlefield

You do not need to win it, only to **deny** it. Every turn they hold it is 1 point for them; every turn nobody holds it is 0 for both. A single Mutated Mouser parked there contests it for two rentals and no attrition. Once Tianna is down the second battlefield stops mattering entirely — they can hold it all they like and score nothing.

### Common mistakes

- **Spending three or more power symbols in a turn.** You will notice the hole two turns later when you cannot cast Tianna.
- **Over-extending to conquer both battlefields early.** One battlefield with Ahri and Blue Sentinel out-scores two ordinary ones.
- **Playing Ahri to your base.** She does nothing there. If you cannot protect her on a battlefield this turn, wait.
- **Hiding cards you won't use.** Every hide is a rune. Hide Fox-Fire and Block; hard-cast Consult the Past when you have spare energy instead.
- **Forgetting the once-per-battlefield cap.** Conquering and then holding the same battlefield in one turn does not double-dip. Ahri's trigger is what breaks the cap, not clever movement.
- **Letting Hallowed Tomb go to waste.** If Ahri dies and Hallowed Tomb is in play, holding it returns her to the Champion Zone to be redeployed — which makes killing her nearly pointless.

---

## 4. Matchup Notes

**Vs. aggro (Fury/Chaos, Fury/Body, Noxus Legion):** You are favoured but turns 1–3 are real. Prioritise zero-power Tank bodies over card draw. The legend's -1 Might plus Shield means their 2- and 3-Might attackers frequently deal nothing. Thwonk! doing double duty for `[4]` and no attrition is your best card here. Fox-Fire is at its best against Legion boards, which routinely present four bodies totalling under 4 Might.

**Vs. token swarm (Order Recruits, Sand Soldiers, Sprites):** Fox-Fire is close to a one-card win. Hide it and fire it mid-showdown after they commit. Crescent Strike's 1 damage to every other enemy also wipes 1-Might boards.

**Vs. big-unit ramp (Dragons, Volibear, Void):** Their threats have heavy energy *and* power costs, so the recycling economy is already fighting them — a `[10][C][C]` finisher sets them back two turns of channelling. Falling Comet answers one for zero attrition on your side. Tianna is at her very best here: their single enormous body scores nothing.

**Vs. other control:** The Hidden package is your edge — cards played from face down cost `[0]` energy, so you win every efficiency exchange on their turn. Be patient; you have the only inevitability, because you are the only deck scoring 3+ a turn.

**Vs. removal-heavy decks:** Do not deploy Ahri into an opponent with ready runes unless you have Not So Fast up. Alpha Wildclaw *before* Ahri is often correct against known removal, even though it delays the clock a turn.

---

## 5. Flex Slots

| Card | Cost | Pwr | Bring in for |
|---|---|---|---|
| **Meditation** | `[2]` | **0** | Extra card draw at zero attrition — Reaction, draw 1, or exhaust a friendly unit to draw 2. |
| **Seal of Focus (3rd copy)** | `[0][C]` | 1 | If you keep getting stranded on Power. Three is greedy in a board game, but it is defensible. |
| **Charm** | `[1][C]` | 1 | Breaking a hold on the second battlefield. Cheap in energy, but remember it costs a rune outright. |
| **Rune Prison** | `[2][C]` | 1 | If you need to stun on *your* turn (Thwonk! only hits attackers). |
| **Zhonya's Hourglass** | `[2]` | **0** | Targeted-removal fields. Zero power, Hidden, redirects a kill onto itself. |
| **Find Your Center** | `[3]` | **0** | Costs `[1]` when they're at 5+ points. Draw 1 *and* channel a rune — pure economy repair. |
| **Navori Scout** | `[4]` | **0** | A 4-Might Deflect body for zero attrition when you want more raw board. |
| **Mageseeker Warden** | `[6][C]` | 1 | Ambush and Reaction-unit decks. Opponents can only play units to their base. |
| **Wind Wall** | `[3][C][C]` | 2 | Only if you're actually losing to sweepers. Two recycled runes for one counter is a steep price. |

Cards I deliberately **cut** on cost-model grounds: **Premonition** `[2][M][M][M]` (three recycled runes for three cards is a losing trade), **Janna, Savior** (great effect, but a third `[C]` card in a Calm-saturated curve), and **Wind Wall** as a maindeck slot.

**Battlefield swaps for a Match (Bo3),** where you choose rather than randomise:

- **Fortified Position** — "when you defend here, a unit gains Shield 2 this combat." Bring in against the fastest aggro starts.
- **Aspirant's Climb** — Victory Score becomes 9. Bring in against decks racing you; an extra point costs them a full turn and costs you about a third of one.
- **Forgotten Monument** — nobody scores here until their third turn. Pure anti-aggro.

---

## 6. One-Paragraph Summary

Riftbound is decided by a scoreboard with a hard ceiling of 2 points per turn, and this is the only configuration in the pool that raises its own ceiling to 4 while lowering the opponent's to 0. Ahri, Alluring turns every hold into a double score and starts in the Champion Zone so she is never a draw-step gamble; Blue Sentinel triples it and doubles both battlefield abilities; Tianna Crownguard freezes their counter outright; Alpha Wildclaw makes all three immune to targeted removal while soaking every point of combat damage as a 7-Might Tank. Just as importantly, it is built for the actual resource system: 55% of the deck costs zero power, so the board never eats your rune base, and the two point-scoring engine pieces cost one recycled rune each and then produce points forever. The opponent has to break a Tank-protected, spell-proof board with a shrinking army and a shrinking mana base, and if they fail even once, they lose by four points a turn.
