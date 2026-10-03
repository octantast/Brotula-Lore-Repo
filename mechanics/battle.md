# Battle

A **battle** in Brotula is a turn-based duel between two sets of brain cells. The player and the creature each fill a 3x3 grid with skills, the two sides take steps in turn, and the side that extinguishes more enemy cells by the end wins.

Related files: [README](../README.md), skills (planned), genes (planned), creatures (planned).

## Brain-cell grids

- Each side has a grid of nine brain cells.
- A cell that holds a skill is a unit with 1 HP. An empty cell holds no skill, takes no damage and counts as a skipped step.
- A cell that is damaged is extinguished and stays extinguished until the end of the battle.
- Every extinguished enemy cell adds 1 to the player's total damage, and every extinguished cell of the player adds 1 to the enemy's.
- The goal is to extinguish more enemy cells while losing as few of your own as possible. Whoever extinguished more enemy cells by the end of the battle wins.
- In battle both creatures shift to the left of the screen. The player's grid opens on top, the enemy's grid opens below it.

## Before the fight

1. The player swims down until a creature blocks the way.
2. The creature's cells are already filled with the skills it will use.
3. The player may inspect them: a tap on an enemy skill shows its targets.
4. The player sets up a formation in response, by tapping their own skills or through the brain button at the top of the screen, which opens the player's skills.
5. New skills cannot be learned at this stage. Preparation had to happen earlier in the dive.
6. Tapping the enemy starts the fight. Tapping your own creature tries to escape (see Escape).

The formation has to be set before the fight starts.

## Turn order

The two sides take steps in turn. A round has 18 steps: 9 for the player's cells and 9 for the enemy's.

**The player moves first.** Player steps run from the bottom-right cell of the player's grid to the left, then up row by row. Enemy steps run from the top-right cell of the enemy's grid to the left, then down row by row.

Player's grid (top):

| 17 | 15 | 13 |
|----|----|----|
| 11 | 9  | 7  |
| 5  | 3  | 1  |

Enemy's grid (bottom):

| 6  | 4  | 2  |
|----|----|----|
| 12 | 10 | 8  |
| 18 | 16 | 14 |

**The enemy moves first.** The order is mirrored: the enemy takes steps 1, 3, 5 and so on, the player takes steps 2, 4, 6 and so on.

Player's grid (top):

| 18 | 16 | 14 |
|----|----|----|
| 12 | 10 | 8  |
| 6  | 4  | 2  |

Enemy's grid (bottom):

| 5  | 3  | 1  |
|----|----|----|
| 11 | 9  | 7  |
| 17 | 15 | 13 |

## Skill effects

Every skill carries one or more icons. The in-game hint (opened by tapping the red starfish at the top right of the skills screen) explains each one.

| Icon | In-game description |
|---|---|
| fish with a mouth | Lowers enemy brain cell activity (attack -1) |
| heart in a tentacle | Increases brain cell activity (heal +1) |
| closed mollusc | Clouds the mind while not extinguished (permanent block) |
| open mollusc with a stone between the valves | Maintains mental clarity while not extinguished (permanent antiblock) |
| sea cucumber (holothurian), stylized | The cell generates a long-lasting impulse (effect x3). These are the poison skills |
| cave with a lurking creature | The cell is activated and damaged when excited (trap -1) |
| neural connections | Impulse reaches multiple targets. Put on every skill with more than one target |

A skill with several effects shows several icons, for example an attack with many targets shows the fish and the neural connections.

## Targets and markers

- A **red crosshair** on the enemy's grid shows where the selected skill hits.
- A **white crosshair** on the player's own grid shows the target of a skill aimed at the player's own cells, for example A breath of calm.
- A **white outline** on the player's own grid shows the cells where the selected skill can be placed.

## High pressure

With depth, pressure closes the cells of both grids. A closed cell is blackened: it is invisible on the enemy's grid and cannot be occupied on the player's grid. Cells 1, 2 and 3 never close. Cells 4 to 9 close at the depths below (metres, as shown in the game). Enemy cells close at the same depths.

| Cell | Closes at | Closes at, with partial protection | Gene that protects it |
|---|---|---|---|
| 9 | 5600 | 6300 | Lipids |
| 8 | 6000 | 8000 | Gigantism |
| 7 | 6300 | 8470 | Hydropores |
| 6 | 6650 | 9000 | Hard body covering |
| 5 | 6800 | 9500 | Statoliths |
| 4 | 7000 | 10000 | Gelatinity |

A gene at level 3 keeps its cell open for the whole dive. A gene at level 2 gives a chance to delay the closing to the deeper depth. Level 1 has no effect on pressure. In the Subduction zone (below 12030) the closed cells of enemies are reopened.

## Escape

Tapping your own creature before the fight tries to escape. Escape is a chance, not a guarantee. The Mimicry gene at levels 2 and 3 improves the chance. According to the game scripts, creatures of the fish type cannot be escaped from, and escape is also disabled in the deepest part of the Subduction zone.

## Reward

After a victory the player chooses one reward: caviar, a companion (mermaid) or a water memory.

- **Caviar** is food. It gives energy, and energy is spent on training new skills during the dive.
- **A mermaid** takes one of the companion slots. There are 2 slots at the start and up to 6. See [companions](../companions/companions.md).
- **A water memory** shows a picture and text and unlocks a story scene. Memories drop at random.

## Level-ups

Battles give experience. Every new level shows the message "Level N reached!" and the player chooses a permanent reward: +1 to the initial caviar stock (the stock starts at 9) or +1 companion slot (2 at the start, 6 at most). With all 6 slots open, only the caviar reward is offered.
