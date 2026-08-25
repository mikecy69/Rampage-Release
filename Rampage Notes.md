# Rampage Notes

## Welcome to Rampage

Rampage is a creature-centered card game in which players summon creatures, wield Items, establish Enchantments, and use Spells and Incantations to defeat the opposing hero. Reduce the opposing hero's Life to zero to win the duel.

This guide is a practical introduction for beta testers. The in-game Glossary provides definitions for keywords and rules terminology found on individual cards.

## Basic controls

### Inspecting cards

- Hover over a card to see its larger preview.
- Left-click a previewed card to freeze the large image in place, allowing you to inspect its text and hover explanations.
- Cards and highlighted terms may provide contextual explanations when hovered.

### Casting cards and using abilities

To cast cards, use Items, activate abilities, or choose targets for effects, you can generally use either method:

- **Double-click** the card or target.
- **Left-click and hold** until the timing meter fills. The action is performed when the meter is full. Release early to cancel.

The green meter is used when casting a card. The blue meter is used for targeting, replacing cards, attaching Items, and activating abilities. The meter duration can be adjusted in Game Options.

During the Replace phase, the blue haze over your hand indicates that card interactions replace cards rather than cast them.

### Priority and phases

- **Pass Priority** yields the current opportunity to respond without necessarily ending the phase.
- A red **End [Phase Name]** button permanently ends that phase and gives up any remaining opportunities available in it.
- Combat buttons confirm attackers, defenders, and damage decisions.
- The phase wheel and phase labels show where the duel currently stands.

## Game modes

Rampage offers three main play modes:

### Constructed

Build and bring your own deck. Choose cards that satisfy the deck-building rules for your selected Biomes, save the deck, and refine it between matches.

### Draft

Build a 30-card deck by choosing cards from a sequence of random offerings. Your Biome choices determine which cards may appear. Draft decks keep a win-loss record and retire after reaching seven wins or three losses.

### Randomly Generated

Play with a 30-card deck generated from two random Biomes. This mode exposes players to a particularly wide variety of cards and interactions. Generated decks also keep a win-loss record and retire after seven wins or three losses.

## The five Biomes

Each Biome has its own personality. Dual-Biome cards combine themes from two different regions, while Universal cards can be used more broadly.

### Forest

Forest represents growth, endurance, natural adaptation, and interconnected life. Its creatures tend to build lasting battlefield value through healing, Boons, regeneration, tribal cooperation, and efficient creature development.

### Mountain

Mountain embodies aggression, fire, physical strength, destruction, and explosive momentum. It favors hard-hitting creatures, direct damage, combat pressure, destructive abilities, and fast attacks.

### Ocean

Ocean rewards knowledge, flexibility, manipulation, and carefully timed responses. Its cards often draw, Discover, Filter, return objects to hand, alter control, or use Flying and reactive effects to outmaneuver the opponent.

### Savannah

Savannah emphasizes courage, discipline, healing, formation fighting, and communal strength. Its armies excel at coordinated combat, protection, Life gain, Boons, and creatures that become stronger when fighting beside allies.

### Swamp

Swamp turns death, sacrifice, decay, fear, and graveyards into resources. It uses Wounds, discard, resurrection, death triggers, draining effects, and creatures that remain dangerous even when they die.

### Universal

Universal cards are not tied to one Biome. They include broadly useful creatures, Items, Enchantments, and utility effects that can support many different strategies. Universal does not function as a sixth Biome when satisfying deck-building requirements.

## Game Options

During a duel, open **Game Options** using the settings icon in the upper-left corner of the match screen. The menu contains navigation controls, display and audio settings, gameplay preferences, the Glossary, and the option to resign.

### Card Size

Changes the size of cards shown on the battlefield.

### Cast-Meter Duration

Controls how long you must hold the mouse button before a hold-to-cast or hold-to-target action completes.

### Music Volume

Controls landing-screen and duel background music.

### Sound Effects

Controls casting, targeting, movement, combat, draw, replace, and other gameplay sounds.

### Make beneficial effects optional

When checked, normally beneficial effects may ask for confirmation instead of resolving automatically. Leave it unchecked for automatic resolution of untargeted beneficial effects whenever the rules permit.

### Auto-Pass Priority with no Legal Moves

When checked, the game automatically passes priority when you have no legal response. When unchecked, the game stops at priority opportunities even when no legal move is available, allowing closer observation and manual testing.

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

- Read the phase and combat subphase labels before acting.
- Use the Glossary when an unfamiliar keyword appears.
- Take a screenshot when something looks wrong.
- Note the exact cards, targets, and sequence that produced the issue.
