# Brotula

**Brotula** is a roguelike about a deep immersion to the very sources of life and water. Battles are turn-based and are fought as a duel of brain cells: each side fills a 3x3 grid with skills that real deep-sea animals use, and the side that extinguishes more enemy cells wins.

- **Developer:** Octanta Studio (Ukraine)
- **Engine:** Unity
- **Genre:** roguelike, turn-based tactics
- **Languages:** English, Ukrainian
- **Platforms:** mobile devices, and in the browser on PC
- **Release:** first released on mobile in August 2022; published on itch.io in 2026
- **Game page:** https://octantastudio.itch.io/brotula
- **Studio website:** https://www.octantastudio.com/
- **Author:** Dariia Zodcha (Octanta Studio). Everything from the art to the code was made by hand
- **Music and sound:** Shvetsb

This repository is a plain-text reference to what is inside the game: mechanics, skills, genes, companions, creatures and the world. Every file starts with a short definition and links to neighbouring files.

## Premise

The player controls a sexless deep-sea explorer who dives from the surface zone toward the sources of life and water. This is not a plain trip to the bottom, and not a decay: the deeper the dive, the closer the explorer comes to the origin of water itself. The explorer keeps dying and is replaced by a modified one, so memory is erased between dives. Water is one and remembers everything: fragments of memory ("water memories") drop at random as battle rewards and unlock story scenes in order. They tell the backstory of a man who tested Brotula, the first social network built into human consciousness, grew tired of the high-tech world, joined deep-sea expeditions and became an explorer like the one the player controls.

The goal of the game is to reach the lowest secret biome and find ringwoodite crystals, the first structures that formed water on Earth. That biome is left as a mystery: its visuals and music differ from the rest of the game, and its gameplay is slightly different.

The visual style is monochrome black and white with red. Both the player and the creatures can be any colour in that range.

## How a run works

1. **Before the dive** the player chooses genes. Genes progress globally between dives, and each gene has levels from 0 to 3. Up to 4 genes can be inserted before an expedition, or 5 with the Intensive development gene.
2. **The dive.** The player holds the bottom of the screen to swim down through biomes. Depth is shown in metres. Zone names appear on the way: Abyssal zone, Hydrothermal vents, Hadal zone, Trench, Trench bottom, Subduction zone. Each zone has its own creatures and mermaids.
3. **Skills.** Skills are learned during the dive for caviar. Caviar is food: it gives energy, and energy is spent on training a skill. Skills exist for one dive only.
4. **Encounter.** The player swims until a creature blocks the way. Its brain cells are already filled with the skills it will use. Before the fight the player can inspect them (a tap on an enemy skill shows its targets) and set up a formation in response. New skills cannot be learned at this point.
5. **Start or flee.** Tapping the enemy starts the fight. Tapping your own creature is an attempt to escape, and escape is a chance, not a guarantee.
6. **Battle.** See [mechanics/battle.md](mechanics/battle.md).
7. **Reward.** After a victory the player picks one reward: caviar, a companion (mermaid) or a water memory.
8. **Level-ups.** Battles give experience. Each new level offers a choice between two permanent rewards: +1 to the initial caviar stock (it starts at 9) or +1 companion slot (the slots start at 2 and stop at 6). Once all 6 slots are open, only the caviar reward is offered.
9. **Companions.** Between fights the player can spend time with a mermaid. After the next fight she generates genes that she can produce, the player picks among them, and the chosen genes are injected after the dive.
10. **Defeat.** The first defeat in a dive can be survived, and the player swims on. When the explorer dies, the player is thrown to the capsule screen, where genes are set up between dives, and then starts a new expedition.

## Progression

- **Carries over between dives:** genes and their levels, the player's level, the initial caviar stock (it starts at 9) and the number of companion slots (2 at the start, 6 at most).
- **Lasts for one dive only:** skills. They cost 1 to 5 caviar each.

## Battle in short

- Each side has nine brain cells in a 3x3 grid. A cell with a skill is a unit with 1 HP.
- The two sides take steps in turn, 18 steps per round. When the player moves first, the player's steps run from the bottom-right cell to the left and then up row by row, and the enemy's steps run from the top-right cell to the left and then down row by row. When the enemy moves first, the order is mirrored.
- An empty cell takes no damage, holds no skill and counts as a skipped step.
- Every extinguished enemy cell adds 1 to the player's total damage. Whoever extinguished more enemy cells by the end of the battle wins.
- Under high pressure, deeper cells are closed. A closed cell is blackened: it is invisible on the enemy's grid and cannot be occupied on the player's grid. Genes keep specific cells open.

## Skill effect icons

Every skill carries one or more icons. A skill has several icons when it combines several effects.

| Icon | Effect |
|---|---|
| fish with a mouth | attack: lowers enemy brain cell activity (-1) |
| heart in a tentacle | heal: raises brain cell activity (+1) |
| closed mollusc | permanent block: clouds the mind while the cell is not extinguished |
| open mollusc with a stone stuck between the valves | permanent antiblock: keeps mental clarity while the cell is not extinguished |
| sea cucumber (holothurian), stylized | long-lasting impulse (effect x3): the poison skills |
| cave with a lurking creature | trap (-1): the cell is activated and damaged when excited |
| neural connections | impulse reaches multiple targets: every skill with more than one target |

## Credits

- **Dariia Zodcha** made everything by hand, from the art to the code.
- **Shvetsb** wrote the music and the sounds.

## Repository map

| Path | Content |
|---|---|
| `README.md` | this overview |
| [mechanics/battle.md](mechanics/battle.md) | battle, turn order, pressure, escape, rewards |
| [skills/skills.md](skills/skills.md) | the full skill list with effects |
| [genes/genes.md](genes/genes.md) | genes, levels and the skills they unlock |
| [companions/companions.md](companions/companions.md) | mermaids and the genes they generate |
| [creatures/creatures.md](creatures/creatures.md) | enemy species by depth |
| [world/world.md](world/world.md) | zones, story, water memories |
| [glossary.md](glossary.md) | terms used across the files |
| [llms.txt](llms.txt) | short index of the pages for AI crawlers |
