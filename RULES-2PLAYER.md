# Riftbound — Core Rules (2-Player Compressed)

**Source:** https://cmsassets.rgpub.io/sanity/files/dsfx7636/news_live/e9ac8e3d33e0f78cef296f5945aba7bc1313b086.pdf  
**Original:** *Riftbound Core Rules* — Last Updated 2026-07-16 — 120 pages, RUP4 Staging  
**Cross-checked against:** [How to Play — Quick Start Guide](https://playriftbound.com/en-us/news/rules-and-releases/how-to-play-get-started/) (official, 2025-06-06)  
**This file:** Compressed summary filtered to **2-player** (`1v1 Duel` & `1v1 Match`). Ignores `FFA3`, `FFA4`, `2v2 Magma Chamber` and team rules except where noted as excluded.

> **Corrections log (from quick-start cross-check):**
> 1. **§5 rewritten** — the rune payment mechanic (exhaust → Energy, recycle → Power) was missing entirely. This is the single most important rule for deckbuilding.
> 2. **§4 Channel Phase** — channelling puts runes in your base ready; it does *not* add to the Rune Pool.
> 3. **§8 Standard Move** — previously read "to a battlefield you control", which contradicted §4 and §9 and made attacking impossible. You may move from base to *any* battlefield.
> 4. **§11 Recycle / Add / Channel** — clarified that recycling a rune returns it to the Rune Deck.
>
> Further official sources not yet folded in: *Unleashed Core Rules Patch Notes* (2026-03-30), *Unleashed Rules FAQ* (2026-04-29), *Unleashed Errata* (2026-04-03), *Spiritforged FAQ/Errata* (2026-01-14). The 2026-07-16 PDF postdates all of these, so they should already be incorporated.

> Rule numbers in parentheses reference the original PDF (e.g., 054.1).

---

## 0. Golden & Silver Rules (000–056)

* **Golden Rule (001.002):** Card text beats rules text.
* **Silver Rule (050–053):** Card text shorthands: “Card” = Main Deck card; “I/me” = that unit/legend, “this” = gear/spell, “here” = that battlefield.
* **Can't beats Can (054):** Forbids override allows; “only” means exclusively.
* **Do as much as possible (055):** Ignore impossible instructions.
* **Ownership (056):** Your cards never go to another player’s non-Board zone (Main Deck, Rune Deck, Trash, Hand, Champion Zone, Banishment) — redirected to owner.

---

## 1. Deck Construction — 2-Player (102–103)

A **deck** for 2-player = Champion Legend + Main Deck + Rune Deck + 3 Battlefields (only 1 used per game):

* **Champion Legend (103.1):** 1 card, placed in Legend Zone. Defines **Domain Identity** (symbols top-left). Cards in deck must match all domains on the card; if multi-domain, identity must contain *all* of them.
* **Main Deck (103.2):** ≥40 cards:
  * **Chosen Champion:** 1 champion unit whose tag matches Legend’s tag (e.g., *Loose Cannon* → tag Jinx → any Jinx champion unit). Placed in Champion Zone at start. Signature units (e.g., Tibbers) *cannot* be Chosen Champion.
  * Other units / gear / spells. Max 3 copies per name (different names count separately even if same character). Max **3 Signature** cards total, all must share Legend’s champion tag. Format legality applies.
* **Rune Deck (103.3):** 12 Rune cards, must match Domain Identity, shuffled separately.
* **Battlefields (103.4):** Provide **3**, include in deck. In 2-player modes only **1** of your 3 is used per game (see Setup), so **2 battlefields are in play total** — one contributed by each player. Cannot have duplicates if multiple required. *(The official quick-start says "each player brings a battlefield", which is the same end state simplified — the 3-then-select-1 step is the constructed/tournament procedure.)*

---

## 2. Setup — 2-Player (110–118, 485–486)

### Common Steps
1. Legend → Legend Zone.
2. Chosen Champion → Champion Zone.
3. Set aside Battlefields (see 2-player modes below).
4. Shuffle Main & Rune decks → respective zones.
5. Determine Turn Order (random, clockwise).
6. Draw 4 each.
7. **Mulligan in turn order:** may set aside up to 2 cards, draw that many, then recycle set-aside.
8. First Player takes first turn.

### 1v1 Duel (485) — *Best of 1*
* **Players:** 2, no teams, **Victory Score 8**, **Battlefield Count 2**
* **Battlefields:** Each provides 3, **randomly selects 1**, other 2 removed. Both selected placed simultaneously in Battlefield Zone.
* **First Turn:** Player going **second channels an extra Rune** during first Channel Phase.

### 1v1 Match (486) — *Best of 3 (or 5)*
Same as Duel except:
* **Selection is chosen, not random** (pick 1 of 3).
* Other 2 set aside. After a game where someone won, that game’s battlefields are **removed**; next game each must choose from remaining set-aside. If no winner, same battlefields may be reused.
* Best-of-5: games 4–5 may reuse a battlefield only if each has been presented once, and no battlefield >2 times.
* First Turn extra Rune same as Duel.

*Excluded for 2-player:* FFA3/FFA4 (3 battlefields, first player no draw, last player extra rune), 2v2 (Victory 11, 3 battlefields, shared points, alternating teams, teammate scoring restrictions).

---

## 3. Play Area — Zones (106–108)

**The Board (public):**
* **Bases (107.1):** 1 per player, a Location holding your permanents/runes. Gear attached to your permanent also in your base.
* **Battlefield Zone (107.2):** Holds the 2 battlefields (2-player). Each battlefield is a Location. White-border = controlled, black = uncontrolled.
* **Facedown Zones (107.3):** 1 per battlefield (max 1 hidden card, may change). You must control battlefield to hide there. If you lose control, facedown cards removed next Cleanup. Facedown cards are private even though zone is public.
* **Legend Zone (107.4):** Champion Legend, cannot leave, not a location.

**Non-Board Zones (per player, private/public as noted):**
* **Chain (108.1):** Temporary zone during card/ability resolution. Public, unordered.
* **Trash (108.2):** Public, ordered by? Public info, ordered.
* **Champion Zone (108.3):** Your Chosen Champion start zone. Public.
* **Main Deck Zone (108.4):** Face-down deck, **Secret** order.
* **Rune Deck Zone (108.5):** Face-down runes, **Secret** order.
* **Banishment (108.6):** Removed/banished cards, Public, unordered.
* **Hand (108.7):** Private, unordered; count is public.

All board objects are Public. Secret → no one may look; Private → only owner/controller; Public → anyone.

---

## 4. Turn Structure — 2-Player Cycle (301–317)

Play cycles turn by turn until win. Turn = **Start of Turn → Main Phase → Ending Phase**. Phases end when no Chain items and Turn Player passes with no discretionary actions.

### Start of Turn (315) — 4 sequential phases:
1. **Awaken Phase (315.1):** Ready all you control that can be readied.
2. **Beginning Phase (315.2):** 
   * “At start of Beginning Phase” triggers fire.
   * **Hold:** Turn Player scores **1 point per battlefield they control** (once per battlefield per turn). Hold triggers queue. *Team mode exclusion ignored for 2-player (no teammate disqualification).*
3. **Channel Phase (315.3):** Channel **2 runes** from Rune Deck (move top 2 face-up to your base, **ready**). Channelling does *not* itself add anything to your Rune Pool — you generate Energy/Power later by exhausting or recycling those runes to pay costs (see §5.1). Second player on first turn channels 3 total (2+1 extra).
4. **Draw Phase (315.4):** Draw 1. If Main Deck empty, **Burn Out** (431): recycle trash → deck (shuffled), opponent gains 1 point, then still draw 1. Repeated burn outs if still empty: each gives opponent 1 point that *cannot be replaced/prevented* and can win game.

### Main Phase (316) — The bulk of play:
* **Start of Main Phase triggers.**
* Neutral Open State — only Turn Player can play/activate (no Action/Reaction needed). No fixed steps; player may act in any order until they pass and chain empty.
* If a player moves units to an uncontrolled battlefield not they control, destination becomes **Contested** → may trigger Showdown (341). If units of two players end up on same battlefield, that battlefield stages **Combat** (459).
* Cleanups interleave to move from Neutral Open → Showdown/Combat when staged. Turn Player chooses which Showdown/Combat next.

### Ending Phase (317):
* “At end of turn” triggers.
* Turn passes to next in Turn Order. Rune Pool empties at end of turn (and start of next Main Phase).

Cleanups (318) handle state checks: winning check (≥ Victory Score and most points wins; 8 for 2-player), conquer/hold scoring limits, chain resolution, contested/combat staging, etc. Occur after moves and after chain empty.

---

## 5. Resources — Runes & Costs (160–167, 201–206, 430)

* **Runes:** Resource cards from a separate 12-card Rune Deck. 6 domains: Fury, Calm, Body, Mind, Chaos, Order + Colorless/A (any). Channelled runes sit **ready in your base**; channelling by itself does *not* put anything in your Rune Pool.
* **Rune Pool:** Conceptual pool holding Energy and Power you have generated. Empties at start of each Main Phase and end of each turn — unspent Energy/Power is lost.

### 5.1 The Two Ways to Spend a Rune ⚠️ *(the core resource rule)*

A rune in your base can be spent in **two different ways**, and this distinction drives all deckbuilding:

| Spend | Action | Produces | Cost to you |
|---|---|---|---|
| **Exhaust** | Turn the rune sideways | **1 Energy** (generic) | **Temporary** — rune stays in your base and readies in your next Awaken Phase |
| **Recycle** | Return the rune to your Rune Deck | **1 Power** of that rune's domain | **Permanent** — rune leaves your base entirely (it will be re-channelled later) |

* **A cost is written as an Energy number plus zero or more Power symbols**, e.g. `[5][Calm]` or `[6][Calm][Calm]`. **Both parts must be paid**: the Energy by exhausting runes, the Power by recycling runes of that domain.
* **An already-exhausted rune can still be recycled.** So the runes you recycle for Power may be the same ones you exhausted for Energy. Runes you need to *have* in base = **max(Energy, Power)**, which is the Energy number for virtually every card.
* **Colorless/rainbow Power `[A]`** may be paid by recycling a rune of any domain.
* **Consequence — Energy is rent, Power is attrition:**
  ```
  net rune growth per turn = +2 (Channel Phase) − (Power symbols you spent)
  ```
  Spend 3+ Power symbols in a turn and your base *shrinks*. This is why the maximum printed Energy cost in the game is **12** — the size of a Rune Deck, reachable only if you have never paid a Power cost.
* **“Add [X]” abilities** (Seals, Ancient Henge, legend abilities, Gold tokens) put Energy or Power straight into the Rune Pool **without exhausting or recycling a rune**, so they sidestep attrition entirely. Abilities that add resources can't be reacted to.
* **Readying runes** (Sona, Targon's Peak, “ready 2 runes”) lets you exhaust them again for more Energy in the same turn. It does **not** return recycled runes — readying fixes Energy, never attrition.
* **Channel N runes exhausted:** the rune enters your base already sideways, so it produces nothing until your next Awaken Phase.

### 5.2 Cost Rules

* **Costs:** Printed cost is base; paying is mandatory to get effect. Additional/Replacement costs (Accelerate, Repeat, Deflect) apply during playing. Effects checking cost use printed/copied cost, not amount paid. Some texts “you may pay [X] as you play me” are Optional Additional Costs (e.g., Accelerate = pay [1][A] to enter ready).
* **Deflect X** and **Hidden** costs are Power costs — they make the payer *recycle* runes, so they are a lasting attack on the opponent's rune base, not just a one-turn tax.

---

## 6. Playing Cards & Abilities (349–360, 376–400)

* **Playable types:**
  * **Units:** Play to your base or battlefield you control (or via Ambush/Ganking permissions) — enter **exhausted** unless Accelerate/ready effect. Have **Might** (combat strength — *not* the same thing as rune Power), a cost (Energy + Power symbols), and Domains.
  * **Gear:** Play to base only (except Hidden at that battlefield). May have Equipment tag + Equip ability.
  * **Spells:** Play during Open State on your turn (or Showdown if Action/Reaction). Resolve effect then go to Trash; if countered/ignored may be banished.
  * **Legends/Battlefields:** Not played like cards; legends static in Legend Zone, battlefields placed at setup.

* **Steps to Play (HOT FEPR):** Handle Outstanding Tasks → Finalize (choices, targets, costs, pay, check legality) → Execute (put on Chain as Pending → Finalized) → Pass priority → Resolve (top of chain).

* **Targets (355.6):** Must be legal at Finalize and at Resolve; if illegal at Resolve, that instruction mistargets/ignored.

* **Abilities:**
  * **Passive:** Continuous while source on board.
  * **Replacement:** Alters event (Deflect adds cost, etc.) — controller of affected object chooses order if multiple.
  * **Activated [cost>effect]:** Only on controlling player’s turn during Open State (unless Action/Reaction). Pay cost → chain.
  * **Triggered “When/At”:** Queued as Pending when condition met, ordered by controller in Turn Order, added to Chain after cleanup.
  * **Delayed:** Created by another effect, active only during specified window (e.g., “next spell this turn”).
  * **Linked:** Abilities on same card referencing each other share context.

---

## 7. Chain, Priority, Focus, Showdowns (311–348)

* **Priority (312):** One player at a time may take Discretionary Actions in Neutral Open. Starts with Turn Player; after they pass, next in Turn Order gets it.
* **Focus (313, 345–347):** During Showdown, who may act alternates. Player who created Contested status gains initial Focus.
* **Chain (327–330):** Stack of Pending→Finalized items. Items added by Turn Order when simultaneous.
* **Showdown (341–342, 348):** When a battlefield becomes Contested *and* turn is Neutral Open, a Showdown stages. It’s an Open State where each player with Focus may play Action/Reaction spells/abilities alternately; passing Focus to next; if all pass without acting, it closes. May stage without Combat (move to empty) or as part of Combat (Step 1).
* **Closed State:** During Chain or Combat Damage step, only Action/Reaction can be used.

---

## 8. Movement & Control (420–455, 188–190)

* **Standard Move (144, 445–452):** As discretionary action on your turn, you may move your units **from your base to any battlefield** — including one that is uncontrolled or controlled by an opponent. That is how you attack: moving into a battlefield you don't control makes it **Contested** (→ Showdown, and Combat if enemy units are there). Moving **battlefield → battlefield** requires **Ganking**.
* **Move via spells/abilities:** May target any legal destination; if moving to uncontrolled battlefield, it becomes Contested → cleanup → Showdown/Combat. After move, perform Cleanup.
* **Recall (454):** Move to base without being a Move (doesn’t trigger move effects, no contesting).
* **Control (188–190):** You control permanents you played/tokens you created; battlefields while you have units there *and* opponent has none. Uncontrolled battlefields’ abilities are controlled by Turn Player if needed.

---

## 9. Combat — 2-Player (459–466)

Staged when two opposing players have units on same battlefield *and* no other Showdown/Combat ongoing. Only between exactly 2 players in Duel.

**Steps:**
1. **Combat Showdown (464):** Focus/Priority loop as in Showdown, starting with player who staged combat. Players may play Action/Reaction.
2. **Combat Damage (465):**
   * Each player assigns total Might of their attackers/defenders as damage to opposing units. Must assign lethal to a unit before next. **Tank** must take lethal before non-Tank of same controller; **Backline** opposite (non-Backline first). **Shield** (+X while defender), **Assault** (+X while attacker) apply. Damage marks stay until cleanup where units with damage ≥ Might are killed (marked damage cleared on zone change).
3. **Resolution (466):** 
   * If one player’s units remain alone and they don’t already control battlefield → they gain control (**Conquer**) and score **1 point** (once per battlefield per turn). Conquer Hold triggers queue. If still contested, no control change.

Units exhaust when they attack/defend unless otherwise readied.

---

## 10. Scoring & Winning — 2-Player (467–472, 194, 323, 431)

* **Score 1 point** via:
  * **Conquer (467, 469.1):** Take control of uncontrolled battlefield *and* haven’t scored it this turn.
  * **Hold (467, 469.2):** Start of Beginning Phase while you still control it (once per turn per battlefield).
* **Limit:** Once per battlefield per turn per player (470).
* **Winning (194, 323.1):**
  * At any Cleanup, if a player has **≥ 8 points (2-player Victory Score) AND more than opponent**, they win immediately; if both ≥8, higher wins (ties? no win, continue). Applies to Duel best-of-1 (first to 8 wins Match) and Match best-of-3 (first to 2 game wins wins Match).
  * Also win via card effect or being last remaining (concede/lose). **Burn Out** repeated empties give opponent unpreventable points and can win.
  * When winning check occurs, game ends (196).

---

## 11. Other Core Actions (413–443 summarized)

* **Draw:** Private from Main Deck; burn out if empty.
* **Recycle:** Return a card to the bottom/shuffle of the deck it belongs to. Main Deck cards recycle from Trash → Main Deck. **A recycled *rune* goes back to your Rune Deck and leaves your base** — this is how Power costs are paid (§5.1), so “recycle” is both a cost and an effect depending on context.
* **Exhaust/Ready (414–415):** Tap/untap; units enter exhausted; awaken readies.
* **Discard (422), Discard?** Choose from hand → trash.
* **Kill (428):** Permanent to Trash (if replaced by recall, death triggers don’t fire).
* **Banish (427):** To Banishment, harder to recover.
* **Buff/Debuff (426):** Temporary Might changes via layers.
* **Stun (423):** Unit doesn’t deal combat damage this turn.
* **Counter (425):** Spell on chain → banished instead of resolving.
* **Add/Channel (429–430):** **Add** = put Energy/Power directly into your Rune Pool without exhausting or recycling a rune. **Channel** = move runes from Rune Deck to your base (ready, unless the effect says “exhausted”).
* **Predict (436):** Look at top of Main Deck, may recycle it.
* **Empower (441–442):** Legend/permanent gains Empowered status if not already; Empowered abilities become active.

---

## 12. Keyword Glossary — Essentials

| Keyword | Type | Quick Effect |
|---------|------|--------------|
| **Accelerate** | Optional Cost | Pay [1] + 1 Power **of my own domain** (verified across all 6 domains) as you play me → I enter ready. Note the Power half recycles a rune. |
| **Action** `[Action]` | Permissive | Playable during Showdowns on any turn (any player) |
| **Reaction** `[Reaction]` | Permissive | Action + playable during Closed States (chain/combat) |
| **Assault X** | Passive | +X Might while attacker |
| **Shield X** | Passive | +X Might while defender |
| **Tank** | Passive | Must assign lethal to Tank units first |
| **Backline** | Passive | Must assign lethal to non-Backline first |
| **Deflect X** | Passive | Opponent pays +X any-Power to target this |
| **Ganking** | Passive | Standard move battlefield ↔ battlefield |
| **Hidden** `[Hidden]` | Hide | Pay [A] on your turn Open State to hide facedown at battlefield you control; next turn gains Reaction, play ignoring base cost; triggers limited to that battlefield |
| **Temporary** | Triggered | Kill this at start of controller’s Beginning Phase |
| **Vision** | Triggered | When played, Predict |
| **Equip [Cost]** | Activated | Attach Equipment gear to unit you control |
| **Quick-Draw** | Gear | Reaction + when you play this, attach to unit |
| **Repeat [Cost]** | Optional Cost | Pay → execute spell/ability a second time (choices separate) |
| **Weaponmaster** | Triggered | When you play me, may choose Equipment you control, pay Equip reduced by [A] even if already attached, attach to me |
| **Legion** `[Legion>]` | Dependent | If you’ve played another card this turn, gains following text |
| **Deathknell** `[Deathknell>]` | Triggered | When I die, effect (only if sent to Trash) |
| **Hunt X** | Triggered | When I Conquer or Hold, gain X XP |
| **Level N** `[Level N>]` | Dependent | While you have ≥N XP, gains text |
| **Unique** | Deck Constraint | Only 1 copy of that name in deck |
| **Empower / Empowered** | Activated/Dependent | Pay to gain Empowered status; Empowered → gains text |
| **Flow [Cost]** | Spell | May play from trash for Flow cost, then banish |
| **Ambush** | Passive/Permissive | May be played to battlefield where you control units (grants Reaction there) |
| **Ally, Scout,** etc. | — | See full rules 800+ for full 25+ keywords |

*Full 120-page keyword list 801–828 compressed; refer to PDF for exact functional text.*

---

## 13. What Was Omitted (Non-2-Player)

Filtered out per instruction: **FFA3 Skirmish** (3p, 3 battlefields, Victory 8), **FFA4 War** (4p, 3 BFs, first player removes BFs), **2v2 Magma Chamber** (4p teams Victory 11, shared points, alternating turn order, teammate activation/scoring restrictions §489.8), and team-specific priority/Cleanup notes. All other layers, attachment (716), XP (728), and comprehensive timing (HOT FEPR) remain as in base rules.

---

## 14. Reference Notes

* **Layers (473–480):** Modifications apply repeatedly until stable, ordered by Timestamp within Layer/Sublayer.
* **Privacy/Timestamp/Inactive Text** rules apply as in PDF; ignored here for brevity.
* E.g., Oath/Allies, Runes basic vs. non-basic, Domain/Battlefield counts for sanctioned 2-player already covered above.

> For complete 800+ rule numbers, examples, and full keyword text, consult the original PDF. This compressed version prioritizes playable 2-player Duel/Match.

