# HIDE ON BUSH — Teemo, Swift Scout (Mind/Chaos Hidden Tempo)

**Format:** 2-Player constructed. Main Deck exactly 40, sideboard 10, 12 runes, 3 battlefields.
**Legend:** Swift Scout (Teemo) — Mind / Chaos
**Chosen Champion:** Teemo, Strategist
**Archetype:** Hidden tempo. Claim a battlefield, hide a card for one Energy, and win the next combat from face down for `[0]`.

Built from the [Sydney Regional Qualifier Top 8](https://playriftbound.com/en-us/news/organizedplay/sydneys-top-decks/) (2026-05-16, 1,405 players — AshenOCE, 6th), the identical Unleashed-era copies that followed it, and the Vendetta spell suite registered at RCS Hobby Con (2026-08-08). Cross-checked against `ALL-SETS.csv` and `RULES-2PLAYER.md`. Official Origins errata for Strategist and Nocturne supersedes the CSV reminder text.

> Teemo is **not** a Tier 1 legend in the current Vendetta metagame. [riftbound.gg's August 28 ranking](https://riftbound.gg/tier-list/) has him in Tier 5; Barcelona RQ coverage never published a Teemo best-of list. This is the most competitive *Teemo* configuration the data supports, not a claim that Teemo is the best deck in the room.

---

## 1. Why This Shell — The Data, Not a Theory

Sydney is the only large-sample result Teemo has. Day 1 field: **30 Teemo** (2.4%). Day 2 conversion: **3** (10.0%), below the ~17–18% baseline a randomly-drawn legend would expect. One of those three, AshenOCE, then finished **6th overall** — legend rank #1 of 30 Teemo pilots, and the only Teemo to make the cut of a 1,000+ player RQ.

That list was copied, not reinvented. bulb's Unleashed Release Party Top 8 (61 players, 2026-05-27) is the same 40 cards. JulianoMasarelli's RCS Hobby Con 43rd (112 players, 2026-08-08) keeps every unit and the entire Sprite package, and only swaps the six flex spells for Vendetta tools.

What the later results did **not** support:

| Brew | Best result | Why it loses to the sprite shell |
|---|---|---|
| Origins "Mundo / Watcher" (Houston RQ, Gorica, 36th/1,347, Dec 2025) | Pre-Unleashed | No Sprite Fountain, no Windsinger, no Switcheroo. Closes with `[8][Mind][Mind]` Mundo. Too slow for Unleashed/Vendetta combat. |
| Hwei / Ember Monk midrange (Samossapinto, 52nd/72, Jul 2026) | Small event | Splits the Hidden plan across a 5-drop painter. No Fountain, no Sprite Call. |
| Spiderling any-count (Chinese City Challenges, Aug 2026) | 42nd/128 | Vendetta's `Spiderling` is a Hidden 1/1 that scales with copies. Density without the ready-3 Sprite clock. |
| Seal / Rhasa Chaos (FLY T1 LS, Las Vegas 63rd/1,670) | Deep Day 2 miss | Plays Kennen's cards without Kennen's legend. Teemo does not reward "played from not-hand" the way Heart of the Tempest does. |

The sprite/Hidden midrange list is the only Teemo configuration that has ever finished in the Top 8 of a Regional Qualifier. Everything below starts from that core and applies only the Vendetta substitutions later pilots independently made.

---

## 2. How The Engine Works

```
Swift Scout  (Legend, Mind/Chaos)
  "You may pay [1] to hide a card with [Hidden] instead of [rainbow].
   [1], [exhaust]: Put a Teemo unit you own into your hand from your
   Champion Zone or the board."
```

Hidden's printed cost is `[rainbow]` — recycle a rune, permanently, every time you hide (811.1.b, `RULES-2PLAYER.md` §5.2). Swift Scout replaces that Power payment with **one exhausted rune**. Hide becomes a rent, not attrition. That is the entire reason this legend exists, and it is why the deck can hide every turn without shrinking the rune base.

The second ability is the replay loop. Bounce Strategist or Scout from the battlefield (or pull the Chosen Champion out of the Champion Zone into hand), then hide him for `[1]`. Next turn he comes down as a Reaction.

### What Hidden actually does (811)

You must already control the battlefield. One facedown card per battlefield (Bandle Tree is the only extra slot; this list does not run it). Hide is not a play and does not open a chain. Beginning the **next** turn, the facedown card gains Reaction and you may play it **ignoring its base cost**. A hidden unit must enter that battlefield; a hidden spell's targets are restricted to that battlefield unless the card's own text makes that impossible (Tideturner is the exception — its swap target is defined as "another location").

If you lose the battlefield, the facedown card is removed at the next Cleanup. The hide is only as good as the hold.

### The four things this deck hides

```
Combat body     Teemo, Scout        — enters as 4 Might this turn
                Teemo, Strategist   — becomes a defender; reveals 5, pings
                                      1 per Hidden card seen, then often
                                      flips Nocturne for [rainbow]

Combat trick    Switcheroo          — swap Might of two units this turn
                Windsinger          — bounce a ≤3 Might unit
                Tideturner          — swap locations with a friendly unit
                Temporal Breach     — banish a unit, owner replays it
                                      exhausted to the same spot
                Evelynn, Entrancing — on your turn, yank an enemy unit
                                      here from another location

Clock           Sprite Call         — ready 3 Might Temporary Sprite for [0]

Card advantage  Consult the Past    — Reaction, draw 2 for [0]
```

Guerilla Warfare is the reset button: return two Hidden cards from trash, then hide ignoring costs. After a combat has spent both facedown zones, it restocks them for `[2]` and one Power.

### Why Sprites, not the old Mundo closer

```
Sprite Fountain   [2][Mind]  Temporary gear
  Play: ready 3 Might Temporary Sprite to base.
  Deathknell: do it again. (Temporary kills the Fountain at the
  start of your next Beginning Phase, before scoring.)

Sprite Call       [3]  Hidden, Action
  Play a ready 3 Might Temporary Sprite.
```

Fountain is two ready 3-Might attackers for `[2][Mind]` — one now, one when the gear dies next turn. Sprite Call from Hidden is a third ready 3-Might body for the cost of yesterday's hide. Temporary means they die before your next Hold scores, so they are conquer tools, not hold tools. That is the correct shape for a deck whose plan is "take the battlefield, hide, win the next showdown."

Dr. Mundo, Expert and Thousand-Tailed Watcher are the Origins finishers. Watcher stays in the sideboard as a closer against wide boards. Mundo does not make the 40.

---

## 3. Decklist

### Legend, Battlefields, Runes

```
LEGEND       Swift Scout                 (Mind/Chaos, tag: Teemo)
BATTLEFIELD  Grove of the God-Willow     "When you hold here, draw 1."
BATTLEFIELD  Startipped Peak             "When you hold here, you may
                                          channel 1 rune exhausted."
BATTLEFIELD  The Arena's Greatest        "At the start of each player's
                                          first Beginning Phase, that
                                          player gains 1 point."

RUNES        7 × Mind Rune
             5 × Chaos Rune
```

Grove / Startipped Peak / Arena's Greatest is unanimous across AshenOCE, bulb, and every later sprite list that reported battlefields. Arena's Greatest puts both players on 1 before anyone has conquered; the deck that wins the first two combats is then racing to 8 from 1, which is this list's whole shape. Bandle Tree ("you may hide an additional card here") is the theoretical Teemo battlefield. The field rejected it — a second hide does not win the combat that keeps the first hide alive.

The 7/5 Mind-heavy split is also unanimous. Fountain, Strategist and Temporal Breach each recycle a Mind rune; Singularity recycles two. Switcheroo is `[2][Chaos][Chaos]` from hand, but this deck never casts it from hand.

### Main Deck — exactly 40

`[E]` = runes to exhaust. `[Mind]` / `[Chaos]` = a rune recycled out of your base.

**Units — 18** *(including the Chosen Champion)*

| # | Card | Cost | Pwr | Might | Role |
|---|---|---|---|---|---|
| 1 | **Teemo, Strategist** | `[2][Mind]` | 1 | 2 | *Chosen Champion.* Hidden. When he defends, reveal 5, deal 1 per Hidden card to one enemy here. |
| 2 | **Teemo, Strategist** | `[2][Mind]` | 1 | 2 | Same. Hide from hand, or bounce with the legend and hide again. |
| 3 | **Teemo, Scout** | `[2]` | **0** | 1 | Hidden. Enters as **4 Might** this turn — the combat-trick body. |
| 3 | **Tideturner** | `[2]` | **0** | 2 | Hidden. Swap locations with a friendly unit at another place. |
| 3 | **Windsinger** | `[2]` | **0** | 1 | Hidden. Bounce another unit at a battlefield with ≤3 Might. |
| 2 | **Sneaky Deckhand** | `[3]` | **0** | 2 | Not Hidden. **Play to an open battlefield** — the card that starts the hide chain. |
| 3 | **Nocturne, Horrifying** | `[4][Chaos]` | 1 | 4 | Ganking. As you look at or reveal him off the top, banish and play for `[rainbow]`. |
| 1 | **Evelynn, Entrancing** | `[2]` | **0** | 2 | Hidden, Backline. Played from facedown on *your* turn: pull an enemy unit here from elsewhere. |

**Gear — 3**

| # | Card | Cost | Pwr | Role |
|---|---|---|---|---|
| 3 | **Sprite Fountain** | `[2][Mind]` | 1 | Temporary. Ready 3 Might Sprite now; Deathknell makes a second when it dies next Beginning Phase. |

**Spells — 19**

| # | Card | Cost | Pwr | Role |
|---|---|---|---|---|
| 3 | **Sprite Call** *(Hidden)* | `[3]` | **0** | Action. Ready 3 Might Temporary Sprite. From Hidden this is `[0]`. |
| 3 | **Switcheroo** *(Hidden)* | `[2][Chaos][Chaos]` | 2 | Action. Swap the Might of two units here this turn. Hide it; never hardcast it. |
| 3 | **Stacked Deck** | `[1]` | **0** | Action. Look at 3, take 1. The on-demand Nocturne flip. |
| 2 | **Consult the Past** *(Hidden)* | `[4]` | **0** | Reaction. Draw 2. Hide for `[1]`, fire for `[0]`. |
| 2 | **Guerilla Warfare** *(Signature)* | `[2][P]` | 1 | Return two Hidden cards from trash. Hide ignoring costs this turn. |
| 2 | **Existential Dread** | `[1][Chaos]` | 1 | Action. Stun an attacker; if already stunned, bounce it. Repeat for `[2]`. |
| 2 | **Temporal Breach** *(Hidden)* | `[2][Mind]` | 1 | Banish a unit; owner replays it to the same location, ignoring cost. Resets ready/Accelerate. |
| 1 | **Star-Crossed** | `[3][Chaos]` | 1 | Reaction. Bounce one friendly *and* one enemy. |
| 1 | **Singularity** | `[6][Mind][Mind]` | 2 | Deal 6 to each of up to two units. The hard reset. |

**Totals: 18 units, 3 gear, 19 spells. 23 Hidden cards (58%). 20 cards at zero Power (50%). 28 of 40 cost `[2]` Energy or less.**

Guerilla Warfare is the only Teemo Signature. Two copies is the field number — the third is often dead before any Hidden card has hit the trash. Three is legal if a local meta is grinding long enough to empty both facedown zones twice.

### Sideboard — 10

Barcelona-era constructed registers 10. Juliano's Hobby Con board is the Vendetta template; Gust replaces his Ocean Drake (`[8][Chaos][Chaos]`, too slow for the actual field).

| # | Card | Cost | Pwr | Bring in for |
|---|---|---|---|---|
| 2 | **Rebuke** | `[2][Chaos][Chaos]` | 2 | Rhasa, Watcher, Alpha Wildclaw, Elder Dragon — Gust and Windsinger cannot touch these. |
| 2 | **Turn to Dust** | `[2]` | **0** | Ornn, Azir, any Seal. Gives a gear Temporary; it dies at their next Beginning Phase. |
| 1 | **Star-Crossed** (2nd) | `[3][Chaos]` | 1 | Midrange mirrors. Saves a Fountain-Sprite pile and breaks a hold. |
| 1 | **Gust** | `[1]` | **0** | Master Yi and Irelia. Reaction bounce of any ≤3 Might unit at a battlefield. |
| 1 | **Decree of Insight** | `[1]` | **0** | Rengar and other Body. Reaction, ignores Deflect, −5 Might. |
| 1 | **Vex, Apathetic** | `[4]` | **0** | Aggro. Deflect. Stuns enemy units played to her battlefield and stops them moving. |
| 1 | **Thousand-Tailed Watcher** | `[7][Mind]` | 1 | Wide boards. Enemy units get −3 Might (min 1); Accelerate to attack immediately. |
| 1 | **Downwell** | `[8][Chaos][Chaos]` | 2 | The panic button. Bounce all units and gear. |

Copy-limit check: Star-Crossed is 1 main + 1 side = 2. No other name appears in both.

---

## 4. The Cost Model — Why Hiding Is Cheap Here and Expensive Everywhere Else

Energy exhausts runes (they ready next Awaken). Power recycles them (they leave the base). Net rune growth per turn = **+2 channelled − Power symbols spent**.

This deck's printed Power count is 24 symbols, 0.60 per card — similar to Kennen on paper, and a lie in practice.

**Half the deck costs zero Power**, and the half that does not is almost all Hidden. Switcheroo's `[Chaos][Chaos]` is 2 recycled runes from hand and **zero** from facedown. Consult the Past is `[4]` from hand and `[0]` from facedown. Sprite Call is `[3]` or `[0]`. Temporal Breach is `[2][Mind]` or `[0]`. The legend converts the hide itself from a Power payment into an Energy payment, so the only Power you actually spend in a normal game is Fountain (`[Mind]`), Strategist (`[Mind]`), the occasional Guerilla / Dread / Star-Crossed, and a Nocturne flipped for `[rainbow]`.

**That is why this list does not run Seal of Insight.** Kennen and Ornn need Seals because they hardcast Power-heavy cards every turn. Teemo's expensive cards are paid for yesterday, with one Energy, and resolved today for nothing. A Seal would recycle a Mind rune to print Mind Power you are trying not to spend.

**Sneaky Deckhand is the only 3-drop that is allowed to be inefficient**, because it is the only card in the 40 that can be played onto an uncontrolled battlefield. Everything else in the curve needs a hold already in place before it can hide. Two copies is the number that finds it early without flooding.

**Singularity is the only honestly expensive card**, and it is a 1-of specifically so it does not show up in the opening hand.

---

## 5. How to Pilot It

### Opening sequence

```
T1   2 runes     Play Tideturner, Windsinger, or Scout to base (all [2],
                 0 Power). Do not hide — you do not control a battlefield.
                 Going second (3 runes): Sneaky Deckhand onto the open
                 battlefield, CONQUER, hide Sprite Call or Switcheroo for [1].

T2   4 runes     Move the 2-drop out → CONQUER (+1). Hide for [1]:
                 Switcheroo if they have a bigger body, Sprite Call if
                 they don't, Strategist if you expect to be attacked.

T3   6 runes     Beginning: Hold (+1). Sprite Fountain [2][Mind] → ready
                 3 Might Sprite in base. Hide the next trick. If they
                 contested, fire yesterday's Hidden during the showdown.

T4   7+ Fountain Beginning: Fountain dies (Temporary, before scoring).
                 Deathknell Sprite #2. Hold (+1). Move a Sprite, fire
                 Sprite Call from Hidden, attack with 6–9 ready Might
                 and a Switcheroo still sitting facedown.
```

The legend bounce is not a turn-one play. Use it after Strategist has defended (or Scout has crashed in as 4 Might) to put him back in hand and hide him again. You *can* hide the Chosen Champion directly from the Champion Zone — Hidden's reminder text allows it (811.1.b) — but bouncing him first lets you play him as a normal 2-drop *and then* hide a different card the same turn, which is often better than spending the Champion Zone hide immediately.

### The three habits that separate good pilots from bad ones

**Hide the card that answers the next combat, not the card that looks most expensive.** Switcheroo and Sprite Call are the default hides. Consult the Past is the hide when the battlefield is already safe. Strategist is the hide when you know they have to attack you. Scout is the hide when you need a 4-Might blocker and do not have Fountain mana. Hiding Consult into a battlefield you are about to lose is a recycled-for-nothing.

**Always check the top for Nocturne before you spend the rest of the turn.** Stacked Deck is `[1]` and looks at 3. Strategist's defend trigger reveals 5. Official Origins errata: *as you look at or reveal Nocturne from the top, you may banish him and play him for `[rainbow]`.* A 4-Might Ganking body for one rune, in the middle of a combat they already calculated, is the highest-value sequence in the deck. Recycle the other revealed cards after the ping; Nocturne is already gone.

**Temporary Sprites conquer. They do not hold.** They die at the start of your next Beginning Phase, *before* Hold scores. If a Sprite is your only unit on a battlefield at that moment, you lose the battlefield and any facedown card on it. Always leave a real unit (Deckhand, Tideturner, a Teemo, Nocturne) as the hold piece, and use Sprites to take the other side or to win the showdown.

### Mulligan

Set aside up to 2, redraw, recycle the rest. You want **a 2-drop that can move, plus a Hidden card worth hiding on turn 2**.

| Keep | Set aside |
|---|---|
| Tideturner, Windsinger, Teemo Scout, Sneaky Deckhand | Singularity, always |
| Sprite Fountain with a 2-drop | Second Fountain, no 2-drop |
| Switcheroo, Sprite Call, Strategist | Guerilla Warfare (nothing in trash yet) |
| Stacked Deck plus any 2-drop | Star-Crossed, Temporal Breach as your only interaction |
| Evelynn only if you already have a claimer | Hands with three Power symbols before turn 3 |

Strategist is sitting in the Champion Zone, so you are not mulliganing to find a Teemo. A hand of Deckhand + Switcheroo + Sprite Call is a snap keep.

### Playing on their turn

Most of the deck is built to be spent while it is not your turn.

- **Switcheroo from Hidden** is the combat you are supposed to lose. A 3-Might Sprite and their 6-Might Rhasa trade Might for the turn; they assign 3, you assign 6.
- **Windsinger from Hidden** is Gust with a body attached, restricted to ≤3 Might. It is your best card against Master Yi and Irelia even before you board Gust.
- **Teemo, Scout from Hidden** is a 4-Might Reaction unit. He eats most 2-drops and contests most 3-drops.
- **Teemo, Strategist from Hidden** becomes a defender the moment he enters combat, which is the errata'd trigger. Choose their best unit, reveal 5, deal ~3 (the deck is 58% Hidden; expected Hidden cards in 5 is about 2.9), recycle. If Nocturne is in the 5, banish and play him for `[rainbow]` *during* that reveal.
- **Existential Dread** stuns an attacker for `[1][Chaos]`. Repeat for `[2]` stuns the second. A second Dread on an already-stunned unit bounces it.
- **Consult the Past from Hidden** is two cards at Reaction speed for `[0]`. Fire it after they pass, not before you know the combat is over.
- **Star-Crossed** returns one of yours and one of theirs. Returning your own Tideturner or Scout so you can hide them again is often the point.
- **Temporal Breach from Hidden** must target a unit *at that battlefield* (811.1.d). It is a replay, not a kill: the unit comes back exhausted, loses Accelerate/ready, and retriggers its play ability. Use it on a ready attacker they just deployed, or on your own Strategist if you need the defend trigger again in the same combat (he left and re-entered).

### Winning the game

You score the ordinary way — conquer and hold, one point per battlefield per turn. Arena's Greatest gives both players a free point on turn 1, so the race is to 8 from 1. Two battlefields held for three of your turns is 6, plus the free point and one conquer, is 8.

You do not have Baron Nashor's third battlefield and you do not have Ahri's extra hold trigger. You win combats they have already committed to, because the facedown card was not in the math. That is enough when the facedown card is Switcheroo, a 4-Might Scout, or a free Nocturne.

Guerilla Warfare on a turn you already control both battlefields restocks both facedown zones for free and usually ends the game the following combat.

---

## 6. Official Text That The CSV Gets Wrong

`ALL-SETS.csv` still has pre-errata reminder text. Play the official Origins errata.

**Teemo, Strategist.** The clause "or I'm played from Hidden" was deleted because attack/defend triggers now fire whenever a unit *becomes* an attacker or defender, including when it is played into combat. He triggers **once**, when he defends, and he has **one** target, chosen as the trigger goes on the chain. He counts cards that *have* the Hidden keyword. Ember Monk, Guerilla Warfare, and Sneaky Deckhand do not.

**Nocturne, Horrifying.** Revised to: *As you look at or reveal me from the top of your deck, you may banish me. If you do, you may play me for `[rainbow]`.* Reveal (Strategist) and look (Stacked Deck) both count. Banishment is the holding zone so he does not have to return to the deck if the play is illegal. Multiple Nocturnes in one look can all come down.

**Tideturner.** Revised to choose a unit you control *at another location* (which is why Hidden targeting restrictions do not lock the swap to the same battlefield).

---

## 7. Matchups

**Kennen (Tier 1, the room).** They play cards from trash, from the top, and from Hidden, and they deploy Rhasa as a 6-Might body for `[2]` by turn four. Windsinger and Gust bounce their Traveling Merchant / Treasure Hunter / Tentacles. Switcheroo is the Rhasa answer. Decree of Unity is Order and illegal in this identity — you cannot board it. Rebuke is your actual Rhasa card. Do not try to out-mill them.

**Master Yi, Wuju Bladesman and Irelia (Tier 1 / 2).** Small, fast, wide, almost everything ≤3 Might. Windsinger, Gust, and Existential Dread are the matchup. Keep early bodies; do not spend turns 1–2 stacking Consult. Vex, Apathetic comes in to stun anything they play onto her battlefield.

**Rengar (Tier 1).** Fury/Body, Punch First, Rampage. Decree of Insight is −5 Might at Reaction, ignores Deflect, and costs `[1]` and zero Power. It is the reason that card is in the 10. Switcheroo still wins the combat they calculated without it.

**Azir and Ornn (Tier 2).** Gear decks. Turn to Dust is the whole plan — Temporary on Sterak's Gage, B.F. Sword, Seal of Focus, or Hidden Blade. Fountain's Deathknell still gives you the second Sprite if they dust *your* Fountain, so losing the gear is not losing the card.

**The Teemo mirror.** Both players hide. The player who claims Bandle Tree (if it shows up) or who fires Guerilla Warfare first usually wins the information war. Hide Switcheroo, not Consult. Do not give them a free look at your facedown card by blinking first.

**Control and other grind.** Consult the Past and Guerilla Warfare are why you win long games. Thousand-Tailed Watcher and Downwell come in; Sneaky Deckhand and a Sprite Call come out. Singularity kills the two things they were using to hold.

---

## 8. Deviations From The Published Lists

The unit column, the Sprite package, the 7/5 rune split, and the three battlefields are AshenOCE's Sydney list untouched. The spell column is JulianoMasarelli's Hobby Con list untouched, except as noted.

| Change vs Sydney (AshenOCE, 6th/1,405) | Reason |
|---|---|
| **−1 Baron Nashor, −2 Bone Skewer, −1 Abandon, −1 Ride the Wind, −1 Consult the Past** | The six cards Juliano cut. Baron is a `[10][Chaos][Chaos][Chaos]` brick in a deck that does not mill. Bone Skewer puts *their* unit onto the battlefield (stunned). Abandon returns the countered spell to hand. Ride the Wind overlaps Tideturner. |
| **+3 Stacked Deck, +2 Temporal Breach, +1 Star-Crossed** | The six cards Juliano added. Stacked Deck is the on-demand Nocturne look — Strategist only reveals when he defends, which is not when you are the one conquering. Temporal Breach is Vendetta's best new Hidden spell in identity. Star-Crossed is the format's best bounce. |

| Change vs Hobby Con (Juliano, 43rd/112) | Reason |
|---|---|
| **−1 Ocean Drake from the sideboard, +1 Gust** | Ocean Drake is `[8][Chaos][Chaos]`, 7 Might, play-to-open, bounce a non-Dragon. It is a worse Baron. Gust is the `[1]` zero-Power Reaction that the rest of the format is built around, and this identity is allowed to play it. |

**On sideboard size:** Sydney registered 8; every Barcelona Top 8 list registered 10. Confirm the event addenda. If the event is still on 8, cut Gust and Decree of Insight and keep Juliano's other eight.

### Flex options the field has actually registered

| Card | Cost | Pwr | Consider over | Who ran it |
|---|---|---|---|---|
| **LeBlanc, Everywhere at Once** | `[4]` | **0** | Evelynn or the 1 Star-Crossed | Crabby Nabs (CCS IQ #4, 31st/160). Backline. Temporary effects at her battlefield do not trigger — Fountain Sprites stay. |
| **Ride the Wind** (main) | `[2][Chaos]` | 1 | Star-Crossed | AshenOCE / bulb. Move and ready; a Sprite can conquer and still block. |
| **Guerilla Warfare** (3rd) | `[2][P]` | 1 | Stacked Deck #3 | Legal. Only if games routinely empty both facedown zones. |
| **Bandle Tree** | — | — | Arena's Greatest | Origins Teemo default. Extra hide slot. The Sydney field preferred the free point. |
| **Edge of Night** | `[3]` | **0** | Turn to Dust | AshenOCE board. Hidden equipment; attach on flip. Worse against Ornn than just killing the gear. |
| **Unchecked Power** | `[7][Mind][Mind]` | 2 | Downwell | AshenOCE board. Exhaust your board, deal 12 to everything at battlefields. A worse Downwell that also eats your Sprites. |

Cards deliberately **not** in this 40: Ember Monk (Hidden payoff without Hidden himself — Strategist does not count him), Blastcone Fae / Fight or Flight / Smoke Screen / Stupefy (the Origins interaction suite the sprite package replaced), Dr. Mundo, Expert (the old closer), Seal of Insight (see §4), Spiderling (a different deck), Ava Achiever (hides from hand as an attack trigger — redundant with the legend).

---

## 9. Legality Check

- ✅ Main Deck is **exactly 40** including the Chosen Champion (402.1, 601.1.b)
- ✅ Sideboard is 10, matching Barcelona-era constructed — verify against the event
- ✅ 1 Legend, exactly 12 runes, exactly 3 battlefields with unique names (402.1)
- ✅ Chosen Champion is Teemo, Strategist — Champion unit, tag **Teemo**, matches the legend
- ✅ 2 Signature cards (Guerilla Warfare ×2), tagged **Teemo**, under the 3-copy Signature cap
- ✅ Every card is Mind, Chaos, Mind/Chaos, or Colorless — inside the Domain Identity
- ✅ No name exceeds 3 copies across Main Deck plus sideboard (403.3, 601.1.c.3)
- ✅ All cards from OGN, SFD, UNL and VEN
- ⚠️ You may not change your Legend, Rune Deck or Battlefields after registration (403.4.b). Only Main Deck cards and the Chosen Champion can be boarded.
- ⚠️ `ALL-SETS.csv` Strategist / Nocturne / Tideturner rows are pre-errata. Use the Origins errata in §6.

---

## 10. One-Paragraph Summary

Swift Scout is the only legend that turns Hidden from a rune you never get back into one Energy you ready next turn, and the sprite/Hidden midrange list is the only Teemo configuration that has ever put a pilot in the Top 8 of a Regional Qualifier — AshenOCE, 6th of 1,405 in Sydney, on a 40 that later Unleashed and Vendetta lists copied rather than rebuilt. You claim a battlefield with Sneaky Deckhand or a 2-drop, hide Switcheroo or Sprite Call for `[1]`, and win the combat they already committed to because the facedown card was not in the math. Sprite Fountain prints two ready 3-Might attackers across two turns; Sprite Call from Hidden prints a third for free; Teemo Scout is a 4-Might Reaction unit; Strategist reveals five on defend, pings about 3, and flips Nocturne for one rune. Half the deck costs no Power, and the half that does is almost all Hidden, so the expensive cards resolve for `[0]`. You score the ordinary two points a turn. Teemo is a Tier 5 legend in the current Vendetta room — this is the version that loses the fewest games, not a version that wins the tournament.
