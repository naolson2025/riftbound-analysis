# TEMPEST — Kennen, Heart of the Tempest (Order/Chaos Recursion Tempo)

**Format:** 2-Player constructed. Main Deck exactly 40, sideboard 10, 12 runes, 3 battlefields.
**Legend:** Heart of the Tempest (Kennen) — Order / Chaos
**Chosen Champion:** Kennen, Storm of Shuriken
**Archetype:** Self-mill recursion tempo. Fill your own trash, then play the game out of it for a fraction of the printed cost.

Built from the [Barcelona Regional Qualifier results](https://playriftbound.com/en-us/news/organizedplay/barcelonas-top-decks/) (2026-08-26, 2,130 players), cross-referenced against `ALL-SETS.csv` and `RULES-2PLAYER.md`.

> This deck replaces `DECK-AHRI-SCOREKEEPER.md`, which was built from first principles and was wrong. Section 6 explains what the tournament data falsified.

---

## 1. Why This Legend — The Data, Not a Theory

Barcelona ran 2,130 players on Day 1 and 379 on Day 2, so the baseline chance of any given deck converting to Day 2 was **17.8%**. Measuring each legend against that baseline separates real performance from mere popularity:

| Legend | Day 1 | Day 2 | Conversion | vs. baseline |
|---|---:|---:|---:|---:|
| **Kennen** | **270** | **81** | **30.0%** | **1.69×** |
| Azir | 79 | 22 | 27.8% | 1.57× |
| Ezreal | 59 | 16 | 27.1% | 1.52× |
| Rengar | 96 | 26 | 27.1% | 1.52× |
| Master Yi, WB | 199 | 47 | 23.6% | 1.33× |
| Irelia | 164 | 36 | 22.0% | 1.23× |
| Rek'Sai | 109 | 21 | 19.3% | 1.08× |
| Nasus | 103 | 14 | 13.6% | 0.76× |
| Ornn | 42 | 5 | 11.9% | 0.67× |

Kennen is the only legend that was simultaneously **the most played deck in the room and the best converting deck in the room**. That combination is hard to fake. Popular decks normally regress toward the baseline because they attract inexperienced pilots and because everyone sideboards against them; Kennen went the other way, growing from 12.7% of Day 1 to 21.4% of Day 2. It then took **three of the Top 8 slots** and the finals. The article calls it "perhaps the deck of the event."

**Ornn won the tournament and is still not the right choice.** Ornn converted 5 of 42 pilots, 0.67× baseline — the third-worst rate among decks with meaningful representation. One trophy from a 42-person sample is variance; 81 Day 2 slots from 270 entries is a signal. Building toward the winner's list here would be reading the noise instead of the data.

**Azir, Rengar and Ezreal are the honest runners-up.** All three converted above 1.5×. Rengar's Fury/Body aggro list is the simplest to pilot if you want a lower-variance option, and Section 7 covers when to prefer it.

---

## 2. How The Engine Works

```
Heart of the Tempest  (Legend, Order/Chaos)
  "When you play a card from anywhere other than your hand, empower me.
   [Action] Disempower me, [exhaust]: Give a unit [Assault 2] this turn."
```

Read that trigger condition carefully, because the whole deck is built to abuse it: **anywhere other than your hand.** Cards played from your trash, from face-down Hidden zones, and from the top of your Main Deck all turn the legend on. Assault 2 is +2 Might while attacking, which is the difference between losing and winning most contested battlefields in this format.

So the deck does not try to out-value you from hand. It deliberately dumps its own library into the trash and then plays Riftbound out of the graveyard, collecting a free combat pump every time it does.

### The four ways this deck plays cards from somewhere other than hand

```
Flow            Lightning Rush   [Flow] [2][rainbow]   — recast from trash, then banish
                Up from the Deep [Flow] [3]

Off the top     Nocturne, Horrifying — "When you look at cards from the top of your deck
                (and don't draw them) and see me, you may play me for [rainbow]."

Hidden          Tideturner, Switcheroo — hide for [rainbow], play later from face down for [0]

From trash      Fizz, Trickster  — play a spell from trash with Energy cost ≤ [3], free
                The Harrowing    — play a unit from trash, ignoring its Energy cost
                Kennen conquers  — give a spell in your trash [Flow] equal to its cost
```

### The self-mill is a discount, not a cost

```
Rhasa the Sunderer   [10][Chaos]  6 Might  —  "I cost [1] less for each card in your trash."
```

Rhasa is the payoff that makes the mill plan profitable rather than merely cute. Every card you burn makes your best body cheaper. By turn four a normal draw has eight or more cards in the trash, at which point Rhasa is a **6-Might unit for `[2][Chaos]`** — better rate than anything an aggro deck can deploy on the same turn. Three copies means you find one early.

Filling the trash is nearly free because the cards that do it are cards you wanted anyway:

- **Kennen, Storm of Shuriken** burns 2 when played, and he starts in your Champion Zone.
- **Lightning Rush** `[1]`, your Signature card, digs 3 and puts the two you don't take in the trash.
- **Stacked Deck** `[1]` digs 3 and recycles the rest — and both diggers can flip **Nocturne** into play for one rune.
- **Minefield** burns 2 every time you conquer there.

### Why the digging is doubly good

Stacked Deck and Lightning Rush both say *look at the top 3*. Nocturne, Horrifying is a 4-Might Ganking unit that you may play for `[rainbow]` — **no Energy at all** — whenever you see it while looking. So a one-Energy cantrip routinely turns into a one-Energy cantrip *plus* a 4-Might body *plus* an empowered legend. That is the single highest-value sequence in the deck, and it is why all three Top 8 Kennen pilots ran 3 Stacked Deck, 3 Lightning Rush and 3 Nocturne without exception.

---

## 3. Decklist

### Legend, Battlefields, Runes

```
LEGEND       Heart of the Tempest        (Order/Chaos, tag: Kennen)
BATTLEFIELD  Minefield        "When you conquer here, put the top 2 cards of your Main Deck into your trash."
BATTLEFIELD  Zaun Warrens     "When you conquer here, discard 1, then draw 1."
BATTLEFIELD  Sandswept Tomb   "Each spell that chooses one or more units here that are friendly to it
                               costs [rainbow] less."

RUNES        9 × Chaos Rune
             3 × Order Rune
```

All three Top 8 Kennen pilots registered Minefield, Zaun Warrens and a 9/3 Chaos-Order rune split. Minefield turns your scoring into fuel for Rhasa; Zaun Warrens loots. Sandswept Tomb is the third slot from the finalist's list and it is the strongest of the options — it makes **Ride the Wind and Star-Crossed cost zero Power** when they target your own units there, which directly attacks this deck's one real constraint (see Section 4).

### Main Deck — exactly 40

`[E]` = runes to exhaust. `[Chaos]` = a Chaos rune to **recycle** (permanently gone from your base).

**Units — 18** *(including the Chosen Champion)*

| # | Card | Cost | Pwr | Might | Role |
|---|---|---|---|---|---|
| 1 | **Kennen, Storm of Shuriken** | `[3][Chaos]` | 1 | 4 | *Chosen Champion.* Burns 2 on play. On conquer, gives a trashed spell Flow. |
| 3 | **Nocturne, Horrifying** | `[4][Chaos]` | 1 | 4 | Ganking. Play for `[rainbow]` off any dig — 4 Might for one rune. |
| 3 | **Rhasa the Sunderer** | `[10][Chaos]` | 1 | 6 | Costs `[1]` less per card in trash. Your best body, usually for `[2]`. |
| 3 | **Traveling Merchant** | `[2]` | **0** | 2 | On move: discard 1, draw 1. Loots every time you attack. |
| 3 | **Treasure Hunter** | `[2]` | **0** | 1 | On move: play a Gold token. Ramps while it conquers. |
| 2 | **Fizz, Trickster** | `[3][Chaos]` | 1 | 3 | Replay a `≤[3]` spell from trash free. Empowers the legend. |
| 2 | **Tideturner** | `[2]` | **0** | 2 | Hidden. Teleports a friendly unit to where it's needed. |
| 1 | **Baron Nashor** | `[10][Chaos][Chaos][Chaos]` | 3 | 12 | Adds a **third battlefield**. Untargetable. All friendlies +2 Might. |

**Spells & Gear — 22**

| # | Card | Cost | Pwr | Role |
|---|---|---|---|---|
| 3 | **Lightning Rush** *(Signature)* | `[1]` | **0** | Dig 3, mill 2. Flow `[2][rainbow]` to do it again from the trash. |
| 3 | **Stacked Deck** | `[1]` | **0** | Dig 3. The cheapest way to flip Nocturne into play. |
| 3 | **Ride the Wind** | `[2][Chaos]` | 1 | Action. Move a friendly unit **and ready it** — conquer without tapping out. |
| 3 | **Seal of Discord** | `[0][Chaos]` | 1 | Gear. **TAP: Add `[Chaos]`.** One rune, once, then free Chaos forever. |
| 2 | **Up from the Deep** | `[3]` | **0** | Two 1-Might Tentacles. Flow `[3]` from the trash for two more. |
| 2 | **Star-Crossed** | `[3][Chaos]` | 1 | Reaction. Bounce one friendly *and* one enemy — saves a unit and breaks a hold. |
| 2 | **Switcheroo** | `[2][Chaos][Chaos]` | 2 | Hidden. Swap the Might of two units. Hide it for `[rainbow]`, fire it for `[0]`. |
| 2 | **Gust** | `[1]` | **0** | Reaction. Bounce any unit at a battlefield with 3 Might or less. |
| 1 | **Hard Bargain** | `[2]` | **0** | Reaction. Counter a spell unless they pay `[2]`. Repeatable for `[2]` more. |
| 1 | **The Harrowing** | `[6][Chaos][Chaos]` | 2 | Play a unit from your trash free. Usually Rhasa or Baron Nashor. |

**Totals: 18 units, 22 spells/gear. 26 power symbols (0.65/card). 19 cards at zero Power (48%). 25 of 40 cards cost `[2]` Energy or less.**

### Sideboard — 10

Barcelona sideboards were **10 cards**, not the 8 in the January rules document — every Top 8 list registered exactly 10. See the note in Section 8.

| # | Card | Cost | Pwr | Bring in for |
|---|---|---|---|---|
| 2 | **Decree of Unity** | `[2][Order]` | 1 | **The mirror.** Kills an enemy Chaos unit or gear. Kennen is 21% of Day 2 — this is your most likely matchup and every card in it is Chaos. All three Top 8 Kennen lists ran 2. |
| 2 | **Salvage** | `[2][Order]` | 1 | Ornn, Azir, Vi — gear decks. Kill a gear, draw 1. Also answers enemy Seal of Discord. |
| 1 | **Angler Beast** | `[5][Chaos]` | 1 | Master Yi and Irelia. Returns **all** units with ≤2 Might to hand, which is most of their board. |
| 1 | **Downwell** | `[8][Chaos][Chaos]` | 2 | When you are behind on board and need a full reset — returns all units *and* gear to hand. |
| 1 | **Invert Timelines** | `[3][Chaos]` | 1 | Grindy games. Both players discard and draw 4 — and your discards feed Rhasa. |
| 1 | **Ravenbloom Prefect** | `[3]` | **0** | Ornn specifically. Banish it to banish a gear as they play it. |
| 1 | **Vi, Peacekeeper** | `[5][Order]` | 1 | Aggro. Ambush lets you flash in a 5-Might body as a Reaction and stun an attacker. |
| 1 | **Rebuke** | `[2][Chaos][Chaos]` | 2 | Big single threats that Gust can't touch — Rhasa, Alpha Wildclaw, Elder Dragon. |

Copy-limit check: no name exceeds 3 across Main Deck plus sideboard. Gust and Star-Crossed are at 2 in the main and 0 in the board.

---

## 4. The Cost Model — Why This Shell Is Cheap

The one piece of analysis worth carrying over from the previous deck is the rune economy, because it turns out to explain why the Kennen shell is good:

- **Energy** (`[3]`) means exhaust 3 ready runes. They untap next Awaken Phase. Renewable rent.
- **Power** (`[Chaos]`) means recycle a Chaos rune back into your Rune Deck. It is gone from your base. Permanent attrition.
- Net rune growth per turn = **+2 channelled − power symbols spent**.

By that measure this deck is unusually efficient, and not by accident:

**Nearly half the deck costs zero Power.** Lightning Rush, Stacked Deck, Traveling Merchant, Treasure Hunter, Tideturner, Up from the Deep, Gust and Hard Bargain — 19 of 40 cards — never shrink your rune base at all.

**Seal of Discord is the same engine card as Seal of Focus, in a better deck.** `[0]` Energy, recycle one Chaos rune, and from then on it taps every turn to Add `[Chaos]` without exhausting or recycling anything. It breaks even on turn two and prints resources thereafter. Three copies is unanimous across the Top 8 lists, and it is your best turn-one play by a wide margin.

**The expensive cards are fake-expensive.** Rhasa reads `[10]` and costs `[2]` in practice. Nocturne reads `[4][Chaos]` and costs one rune when flipped off a dig. Up from the Deep and Lightning Rush recast from the trash for Flow rather than being drawn twice. The Harrowing pays full price once to put a `[10]` unit into play for free. The only genuinely expensive card is Baron Nashor.

**Sandswept Tomb is Power reduction.** Ride the Wind and Star-Crossed both choose friendly units. Played at Sandswept Tomb, they cost `[rainbow]` less — which zeroes their Power symbol. Over a long game that is several runes you keep.

The result is a deck that runs 0.65 power symbols per card while casting a 6-Might unit on turn four and never actually going backwards on mana.

---

## 5. How to Pilot It

### Opening sequence

```
T1   2 runes    Seal of Discord [0][Chaos].  Recycle 1 → 1 rune in base, but the Seal
                now adds [Chaos] every turn. Tap it, cast Stacked Deck [1].
                If Stacked Deck reveals Nocturne, play it for [rainbow].

T2   3 + Seal   Treasure Hunter [2] and Traveling Merchant [2] to your base.
                Both zero Power. Both want to move next turn.

T3   5 + Seal   Move Treasure Hunter out → CONQUER (+1 point), and its move trigger
                plays a Gold token. Move Traveling Merchant → loot 1.
                Cast Lightning Rush [1]: dig 3, two cards to the trash.
                Trash is now 4-6 cards deep.

T4   7 + Seal   Beginning Phase: Hold both = +2.  Rhasa the Sunderer now costs about
                [2][Chaos] for a 6-Might body. Deploy it onto a battlefield you hold.
                Hold up Gust [1] on their turn.

T5+             Ride the Wind to move-and-ready, conquer the contested battlefield,
                and use the legend's Assault 2 to win the combat you're supposed to lose.
```

### The three habits that separate good pilots from bad ones

**Always check whether the legend is empowered before you attack.** Every Flow cast, every Hidden card, every Nocturne off the top empowers Heart of the Tempest. Disempowering it to hand out Assault 2 costs you nothing but the exhaust. Forgetting this is the single most common way to lose a combat you had won.

**Burning your own cards is not a cost — but Burn Out is real.** Filling the trash makes Rhasa cheap, Fizz live, and The Harrowing enormous. But rule 431 says that if your Main Deck is empty at your Draw Phase you recycle your trash into your deck, shuffle, and **your opponent gains a point**. This deck can genuinely deck itself in a long game. Once you are past about 12 cards remaining, stop milling for value and start closing.

**Sequence your digs before your deployments.** Stacked Deck and Lightning Rush can flip Nocturne into play for one rune. If you cast your dig first, you may find a free 4-Might body and change what you were going to spend the rest of your Energy on. Casting the body first and then digging wastes that option.

### Mulligan

You may set aside up to 2 cards and redraw. You want **a Seal of Discord or a one-mana dig, plus a two-drop that moves**.

| Keep | Set aside |
|---|---|
| Seal of Discord | Rhasa in an opening hand with no way to fill the trash |
| Stacked Deck, Lightning Rush | Baron Nashor, always |
| Treasure Hunter, Traveling Merchant | The Harrowing before turn five |
| Any hand with a turn-2 and a turn-3 play | Hands with three or more Power symbols in the first three turns |

Kennen is in your Champion Zone, so you are never mulliganing to find him. A hand of two cheap movers and a dig is a perfect keep even with no expensive cards in it.

### Playing on their turn

A third of this deck is Reaction speed and most of it costs no Power.

- **Gust `[1]`** is the best card in the deck against the actual Barcelona field. Master Yi, Irelia, Rengar and Master Yi's Lonely Poro / Scuttle Crab / Pit Rookie shells are full of units with 3 Might or less. Bouncing a unit mid-showdown at Reaction speed for one Energy and no attrition swings the combat and costs them the whole card.
- **Star-Crossed** bounces one of theirs *and* one of yours. Returning your own unit is often the point: it saves a Traveling Merchant from dying and lets you replay it for another move trigger.
- **Hard Bargain** is a tax, not a hard counter. Use it when they are tapped out, not as a Plan A.
- **Hide Switcheroo when you have a spare rune.** Swapping the Might of a 1-Might Tentacle and their 6-Might attacker, played from face down for `[0]`, ends games.

### Winning the game

You score the ordinary way — conquer and hold, capped at one point per battlefield per turn — and that cap is fine. The previous deck tried to break the ceiling and lost sight of the fact that **nobody in this format is actually hitting the ceiling every turn**. Winning combats reliably is worth more than raising the maximum.

Two things do let you exceed two points a turn when the game goes long:

- **Baron Nashor** adds the Baron Pit battlefield token, which any unit can move to from anywhere. That is a genuine third scoring location, plus a 12-Might untargetable body, plus +2 Might for everything else you control.
- **Ride the Wind** readies the unit it moves, so a single unit can conquer and still be available to defend.

---

## 6. What The Ahri Deck Got Wrong

Worth writing down, because the failure was analytical rather than arithmetic.

**The claim was:** scoring is capped at 2 points per turn, so the deck that raises its own ceiling to 4 and lowers the opponent's to 0 must win the long game.

**What was wrong:** the ceiling was never the binding constraint. Getting Ahri (`[5][Calm]`) and Blue Sentinel (`[4][Mind]`) onto the same battlefield and keeping them alive through two Beginning Phases is a turn-six plan. Kennen, Master Yi and Irelia are decks that have already conquered twice by turn four with units that cost `[2]`. The relevant question was never "how many points can I score per turn" but "can I win the combat on turn three," and I never modelled that.

**What held up:** the rune economy analysis. Zero-Power cards really are undercosted, the Seal cycle really is the best engine effect in the game, and 8/4-style skewed rune splits really are correct. The winning Ornn list ran 3 Seal of Focus and an 8 Calm / 4 Mind rune pool — exactly the package and split I had derived. I applied a correct economic model to a legend that could not use it.

**The falsification was total.** Zero of 2,130 players brought Ahri. All eight legends with no representation are from the original core set, while every legend from Spiritforged, Unleashed and Vendetta had at least one pilot. Nine-Tailed Fox is not banned; it is simply outclassed.

---

## 7. Matchups

**Kennen mirror (21.4% of Day 2 — expect it twice).** The most important matchup in the room. Both decks are Chaos, which makes Decree of Unity a clean two-for-one that they cannot answer. Whoever resolves Rhasa first usually wins the board, so prioritise milling over value early. Do not over-mill: mirror games go long and Burn Out decides more of them than combat does.

**Master Yi, Wuju Bladesman (12.4%) and Irelia (9.5%).** Small, fast, wide. Gust and Angler Beast are your two best cards — most of their board is 3 Might or less. Bring in Vi, Peacekeeper for an Ambush blocker. Keep hands with early bodies over hands with card selection; you cannot afford to spend turns one and two digging.

**Rengar (6.9%) and other Fury/Body aggro.** They present 3-Might bodies with Punch First and Rampage pumps. Your legend's Assault 2 lets your Nocturne beat their Kinkou Initiate in combat, and Rhasa outsizes everything they have. Star-Crossed to save a blocker is better than Star-Crossed to break a hold here.

**Azir (5.8%).** Gear-heavy — B.F. Sword, Soul Sword, Hidden Blade, Brutalizer. Salvage is excellent and Ravenbloom Prefect can eat a key piece as it lands. Their units are small without equipment, so answering the gear is answering the deck.

**Ornn.** Slow, gear-based, and the reason Salvage and Ravenbloom Prefect are in the board. You are far faster. Do not let the game reach the turn where Sterak's Gage and Guardian Angel make their board unkillable.

**Control and other grindy decks.** Invert Timelines and the Flow package mean you have more total cards than they do. Hold Hard Bargain for their key sweeper, and remember The Harrowing rebuys anything they kill.

---

## 8. Deviations From the Barcelona Lists

I started from the three Top 8 Kennen lists and kept everything they agreed on. The unanimous core — 3 Lightning Rush, 3 Nocturne, 3 Rhasa, 3 Ride the Wind, 3 Seal of Discord, 3 Stacked Deck, 3 Traveling Merchant, 2 Fizz — is untouched, as is the 9/3 rune split and the Minefield/Zaun Warrens battlefield base.

Relative to the finalist's list (CTCG Koko Lopez, 2nd place), I made four changes that net to zero:

| Change | Reason |
|---|---|
| **+2 Gust** | Both other Top 8 Kennen pilots ran 2 and the finalist ran 0. Against a Day 2 field that is a quarter Master Yi and Irelia, a `[1]` zero-Power Reaction that bounces any unit with ≤3 Might is too well-positioned to leave out. |
| **−1 Flash, −1 Shadow Order Disciple** | Both singletons, both replaceable. Flash overlaps with Star-Crossed; Shadow Order Disciple is the weakest body in the shell. Singleton reactive cards you cannot reliably draw are worse than a second copy of something good. |
| **+1 Star-Crossed, +1 Tideturner** | Moves both to 2, matching the other two Top 8 lists. |
| **−2 Last Rites** | **Flagged, not confident.** Five copies appeared across the three Top 8 lists, so the field clearly rates it. But the `ALL-SETS.csv` row for Last Rites contains only its Equip cost with no granted ability, so I could not evaluate what it actually does and would not write a pilot guide around it. Check the physical card — if it is as good as the field's usage implies, the first two Gust are the slot to take back. |

**On sideboard size:** the January tournament rules document says 8 or fewer (601.1.c.1), but every Barcelona Top 8 list registered exactly 10. The rule has evidently been updated since January. Confirm the current number in your event's addenda before you register — this also means the 8-card board in `DECK-AHRI-SCOREKEEPER.md` is built to a stale rule.

### Other flex options, all field-supported

| Card | Cost | Pwr | Consider over |
|---|---|---|---|
| **Tail-Cloaked Matriarch** | `[4]` | **0** | Tideturner. Empower to reanimate a cheap unit from the trash — another play from not-hand. |
| **Rebuke** (maindeck) | `[2][Chaos][Chaos]` | 2 | Hard Bargain, if the field is big units rather than spells. |
| **Gust Monk** | `[2]` | **0** | Treasure Hunter, for a more aggressive draw. |
| **Shadows of the Past** | `[3][Chaos]` | 1 | The Harrowing, as a cheaper way to rebuy two units to hand. |
| **Forbidding Waste** | — | — | Sandswept Tomb, if you expect opponents to hold with a single unit. Cuts both ways. |
| **Veiled Temple** | — | — | Sandswept Tomb, only if you add the Last Rites equipment package back. |

---

## 9. Legality Check

- ✅ Main Deck is **exactly 40** including the Chosen Champion (402.1, 601.1.b)
- ✅ Sideboard is 10, matching every Barcelona Top 8 list — verify against current rules
- ✅ 1 Legend, exactly 12 runes, exactly 3 battlefields with unique names (402.1)
- ✅ Chosen Champion is Kennen, Storm of Shuriken — Champion unit, tag **Kennen**, matches the legend
- ✅ 3 Signature cards (Lightning Rush ×3), tagged **Kennen**
- ✅ Every card is Order, Chaos, Order/Chaos or Colorless — inside the Domain Identity
- ✅ No name exceeds 3 copies across Main Deck plus sideboard (403.3, 601.1.c.3)
- ✅ All cards from OGN, SFD, UNL and VEN — the sets played at Barcelona in August 2026
- ⚠️ You may not change your Legend, Rune Deck or Battlefields after registration (403.4.b). Only Main Deck cards and the Chosen Champion can be boarded.

---

## 10. One-Paragraph Summary

Kennen was both the most-played and the best-converting deck at a 2,130-player Regional Qualifier, taking three Top 8 slots and the finals at 1.69× the field's baseline conversion rate — the strongest combined signal any legend produced. The deck works because Heart of the Tempest rewards playing cards from anywhere other than your hand, and Chaos gives it four separate ways to do that: Flow spells recast from the trash, Nocturne flipped off the top for a single rune, Hidden cards fired from face down for zero, and Fizz and The Harrowing reanimating out of the graveyard. Self-milling is pure profit rather than a cost, because Rhasa the Sunderer gets a discount for every card in the trash and lands as a 6-Might body for two Energy by turn four. Nearly half the deck costs no Power at all and three Seal of Discord print a Chaos rune every turn, so the rune base grows while you deploy. You score the ordinary way, two points a turn, and that is enough — because the constraint in this format was never the scoring ceiling, it was whether you win the combat on turn three.
