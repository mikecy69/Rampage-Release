# Rampage Notes
Rampage is a creature-centered card game in which players summon creatures, wield Items, establish Enchantments, and use Spells and Incantations to defeat the opposing hero. Reduce the opposing hero's Life to zero to win the duel.
This guide is a practical introduction for beta testers. The in-game Glossary provides definitions for keywords and rules terminology found on individual cards.

## Inspecting cards and card elements
- Hover over a card to see a larger preview
- Left-click a currently hovered over card to freeze the larger hover image in place, allowing you to inspect its text and hover explanations
- Right-click a card to bring up a "Huge" version of the card for closer inspection
- At the top left of each card is its name; casting cost (energy) is at the top right. Under that is a rarity symbol (Common, Uncommon, Rare, Epic) and the card type (Creature, Item, Enchantment, Spell, Incantation).
- The bottom of the card has card text explaining what the card does
- For creature cards, at the bottom you'll find gold keywords for creature abilities, and the Strength / Health of a creature in the lower right

## Casting cards and using abilities
To cast cards, use Items, activate abilities, or choose targets for effects, you can use several methods:
- **Double-click** the card or target
- **Left-click and hold** until the timing meter fills - the desired action is performed when the meter is full. Release early to cancel. The green meter is used when casting a card. The blue meter is used for targeting, replacing cards, attaching Items, and activating abilities. The meter duration can be adjusted in Game Options.
- To the right of your cards in hand is the **Action Button** area. You can "commit" your actions by clicking the buttons shown here, whose labels change depending on the current game actions

## Card Types
- **Creatures**: the beasts used to maul your opponent. Read their keywords carefully to get a sense of how to play them properly.
> NOTE: For each player, there are only 8 available battlefield spaces for creatures. If a 9th non-token creature is cast, the caster will have to choose which creature to replace, or choose not to resolve the newly casted creature at all. Any spell/effect that produces tokens will not produce any with a full board. If some board spots are open, but not enough for all tokens produced, then a partial number of tokens will fill the empty slots.
- **Items**: similar to MtG artifacts, they can be "Attached" to creatures or perform functions on their own
- **Enchantments**: can also be cast directly onto creatures to provide modifications, or directly onto the battlefield for static global effects
- **Incantations**: the MtG "Sorcery"; a slow-speed spell
- **Spells**: the MtG "Instant" that can be cast during all of your turn phases and the opponent's turn

## Priority and Phases
Each Round has 2 Turns: one for each player. Each Turn has 7 phases:
- **Refresh**: Max energy increased by 1 and energy restored to full; creatures lose "Exhausted"
- **Draw**: a card is drawn
- **Replace**: one card from your hand can be chosen to be shuffled back in your deck; at the same time, a random card from your deck (other than the replaced card) will be drawn;
  during the Replace phase, the blue hazy rectangle over your hand is a visual indication that clicked cards will be replace in this phase, not cast
- **Preparation**: Pre-combat phase where all cards types can be cast
- **Combat**: The active player declares attackers, then the other player declares defenders; combat damage is assigned and then damage resolves and the battlefield is cleaned up
- **Triage**: Post-combat phase where all cards types can be cast
- **End**: End-of-turn actions resolve and the turn is passed to the other player

### Turn/Phase Notes:
- Only Spells and item/creature abilities that aren't specified "As an Incantation" can be used outside of the Preparation and Triage phases on your Turn, and on your opponent's Turn
- **Pass Priority** yields the current opportunity to respond without necessarily ending the phase.
- A red "End [Phase Name]" button permanently ends that phase and gives up any remaining opportunities available in it
- Combat buttons confirm selected attackers, defender positioning, and damage decisions
- The phase wheel above the player portrait and phase labels to the right of the player's hand show the current phase
- The player going first on Turn 1 will not draw a card for that Turn.

## Combat
- Creatures that are declared as attackers become "Exhausted" (unless they have Stamina) and are unavailable to defend during the subsequent turn
- The attacking player only selects which creatures they want to attack with. The defending player then chooses what defenders to assign to each attacker, with multiple defenders per attacker being legal
- In Rampage, damage to creatures is not cleared at the End phase. A 3/3 will kill a 2/2 in combat, but will be left as a 3/1 afterwards. This changes combat math dramatically as compared to MtG! You've been warned...

## Game modes
Rampage offers three play modes:

- **Constructed**
Choose your Biomes (limit of 2), build your own deck. If a deck has a single biome, ALL dual-biome cards involving that biome are eligible for admission. If the deck is dual-biome, only dual-biome cards of that specific combination are eligible. Choose cards that satisfy the deck construction rules, save the deck, and refine it between matches. Rules: a deck must have at least 30 cards, but not more than 180. In a 30-card deck, a maximum of 2 Epics are allowed (both must be unique), 6 rares (at most 2 copies of each rare), and 3 copies of any common/uncommon. Once you reach 60 cards, you may have 4 epics (still single copies) and 12 rares (3 copies of each). For 90, 120, 150 and 180 card decks, the numbers scale, but never more than 3 copies of any non-epic, and 1 copy of any unique Epic is allowed. The exception is Creatures with the Keyword "Tribal." For those cards, you may have 5 of the exact same card in a 30 card deck, 10 in a 60 card deck, etc.
- **Draft**
Build a 30-card deck by choosing cards from a sequence of random offerings: 30 sets of 4 cards. Your initial Biome choices determine what cards appear. Each drafter will be offered exactly 2 epics and 8 rares in the 120 cards; the rest will be commons and uncommons. There are 2 "Two Pick" tokens the drafter can spend to draft 2 cards, rather than 1, out of the set of 4 that are offered. Draft decks keep a win-loss record and retire after reaching seven wins or three losses.
- **Randomly-Generated**
Play with a 30-card deck generated from two random Biomes. This mode exposes players to a wider variety of cards and interactions. Generated decks also keep a win-loss record and retire after seven wins or three losses.
> NOTE: When a player's library is gone, they will lose 1 Life at the start of their next turn, then 2 Life at the start of their next turn, then 3 Life at the start of their next turn, etc., until some player wins the game.

## The five Biomes
Each Biome has its own personality. Dual-Biome cards combine themes from two different regions, while Universal cards can be used more broadly.

### Forests
Represent growth, endurance, natural adaptation, and interconnected life. Forest creatures tend to build lasting battlefield value through healing, Boons, regeneration, tribal cooperation, and efficient creature development.
### Mountains
Embody aggression, fire, physical strength, destruction, and explosive momentum. This biome favors hard-hitting creatures, direct damage, combat pressure, destructive abilities, and fast attacks.
### Oceans
Reward knowledge, flexibility, manipulation, and carefully timed responses. Ocean cards often draw, Discover, Filter, return objects to hand, alter control, or use Flying and reactive effects to outmaneuver the opponent.
### Savannahs
Emphasize courage, discipline, healing, formation fighting, and communal strength. Savannah armies excel at coordinated combat, protection, Life gain, Boons, and creatures that become stronger when fighting beside allies.
### Swamps
Turn death, sacrifice, decay, fear, and graveyards into resources. Swamp tactics use Wounds, discard, resurrection, death triggers, draining effects, and creatures that remain dangerous even when they die.
### Universal
Universal cards are not tied to one Biome. They include broadly useful creatures, Items, Enchantments, and utility effects that can support many different strategies. Universal does not function as a Biome when satisfying deck-building requirements.

## Game Options
During a duel, the Settings icon in the upper-left corner of the match screen opens the **Game Options** modal. The modal contains navigation controls, display and audio settings, gameplay preferences, the Glossary, and the option to Resign.

### Card Size
Changes the size of cards shown on the battlefield
### Cast-Meter Duration
Controls how long you must hold the mouse button before a hold-to-cast or hold-to-target action completes
### Music Volume
Controls landing-screen and duel background music
### Sound Effects
Controls casting, targeting, movement, combat, draw, replace, and other gameplay sounds
### Make beneficial effects optional
When checked, normally beneficial effects (healing, card drawing, etc) may ask for confirmation instead of resolving automatically. Leave it unchecked for automatic resolution of untargeted beneficial effects whenever the rules permit.
### Auto-Pass Priority with no Legal Moves
When checked, the game automatically passes priority when you have no legal response. When unchecked, the game stops at priority opportunities even when no legal move is available, allowing closer observation and manual testing.

## Other UI Elements
- Your character portrait can by changed by right-clicking and choosing a different one.
- Your life total is shown below your portrait. Both players start with 20 Life.
- A silver timer to the right of your life total counts down how long you have to make decisions before priority is passed to your opponent.
- The **Phase Wheel** rotates to show you the Turn phase. The apex of that wheel is green during your turn and gray during the opponent's turn.
- The **Energy Wheel** shows you how many maximum and available energy "pips" you currently have. Available pips are filled blue, unavailable are empty circles. In Rampage, maximum energy starts at 1 on Turn 1 and increases by 1 each turn. It rises no higher than 10.
- Your library and graveyard at shown at the lower left. You can click your graveyard to open it and view the cards there.
- The "stack" is shown in the left-middle of the screen during a duel. That's where actions go before they are resolved. Players get an opportunity to react to most stack actions with Spells or Spell-speed abilities.

## CPU difficulty
The CPU has four difficulty levels:
- **Casual** — Uses a small search budget, examines fewer actions and combat arrangements, and includes substantial variation in its choices. Intended for relaxed or introductory play.
- **Normal** — Searches more alternatives with less randomness and provides a moderate challenge.
- **Challenging** — Examines substantially more plays and combat configurations and forecasts important consequences into the opponent's next turn.
- **Expert** — Uses the broadest search, deepest rollouts, strongest combat exploration, no deliberate scoring noise, and next-turn forecasting. Intended to find the highest-value line available within its thinking budget.
The current approximate thinking budgets are 0.5 seconds for Casual, 1 second for Normal, 3 seconds for Challenging, and 6 seconds for Expert. Complex positions may still be constrained by the number of legal actions and target combinations.

### How the CPU thinks
The CPU does not follow a fixed script for every card. It generates legal actions and target combinations, simulates their results, and compares the resulting board states using an expected-value model. That evaluation considers factors such as:
- Creature Strength, Health, keywords, and persistent damage
- Cards in hand and diminishing value near the hand limit
- Current and maximum Energy
- Hero Life, with increasingly severe penalties at dangerously low Life
- Removal, card advantage, control effects, and battlefield presence
- Tough, Disciplined, Masterful, Unstoppable, and other combat mechanics
- Attack and defense configurations
- The value of passing, preserving reactive Spells, or waiting for a better timing window
- Replacement decisions during the early, middle, and late game
- Likely opponent responses and, at higher levels, defensive needs on the following turn
Expert play is still an approximation rather than a perfect solution to every possible position, but its simulation-based approach allows it to recognize many interactions without relying on a separate hard-coded instruction for every card.

## Helpful beta-testing habits
- Read the phase and sub-phase labels before acting
- Use the Glossary when an unfamiliar keyword appears
- Take a screenshot when something looks wrong
- Note the exact cards, targets, and sequence that produced the issue
