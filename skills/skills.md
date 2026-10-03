# Skills

A **skill** in Brotula is an action that the player places on a brain cell before a battle. It is one of the moves that real deep-sea animals use to hunt, defend themselves or hide. A skill lasts for one dive.

Related files: [README](../README.md), [battle mechanics](../mechanics/battle.md), genes (planned).

## How skills are obtained

- Skills are learned during the dive for caviar. Caviar is food: it gives energy, and energy is spent on training a skill.
- New skills cannot be learned once the player has met a creature and the battle is being prepared.
- Skills 1 to 9 need no genes.
- Every other skill unlocks only when the listed gene reaches level 3 (the maximum). Skills 30 to 43 need two genes at level 3.

## Effect types

| Icon | Effect |
|---|---|
| attack | lowers enemy brain cell activity (-1) |
| heal | raises brain cell activity (+1) |
| block | permanent block: clouds the mind while the cell is not extinguished |
| antiblock | permanent antiblock: keeps mental clarity while the cell is not extinguished |
| long-lasting | long-lasting impulse (effect x3): the poison skills |
| trap | the cell is activated and damaged when excited (-1) |
| multi-target | impulse reaches multiple targets: every skill with more than one target |

## All skills

| ID | Skill | Caviar | Effects | Genes needed (level 3) |
|---|---|---|---|---|
| 1 | Silent threat | 1 | attack | none |
| 2 | Aiming to hit | 1 | attack | none |
| 3 | Flick | 1 | attack | none |
| 4 | Distraction bait | 1 | block | none |
| 5 | Vigilance | 2 | antiblock | none |
| 6 | A breath of calm | 2 | heal | none |
| 8 | Dream of life | 2 | heal | none |
| 9 | Hypnotic dance | 1 | block | none |
| 10 | Competence in anatomy | 2 | heal, multi-target | Red pigmentation |
| 11 | Comprehensive recovery | 2 | heal, multi-target | Red pigmentation |
| 12 | Invisibility | 2 | antiblock | Transparency |
| 13 | A weak point detection | 1 | attack | Black pigmentation |
| 14 | Merging with darkness | 1 | attack | Black pigmentation |
| 15 | Blinding camouflage | 1 | block | Bioluminescence |
| 16 | Puncture | 4 | attack, multi-target | Cirri, needles |
| 17 | Pinch | 4 | attack, multi-target | Pedicellariae |
| 18 | Bacteria cleansing | 3 | heal, multi-target | Pedicellariae |
| 19 | Tentacle tenacity | 3 | block | Tentacles, suckers |
| 20 | Autotomy | 3 | trap | Regeneration |
| 21 | Bite | 5 | attack, multi-target | Teeth |
| 22 | Thanatosis | 3 | attack, block | Evisceration |
| 23 | Ink cloud | 4 | attack, multi-target | Ink bag |
| 24 | Ink jet | 4 | block, multi-target | Ink bag |
| 25 | Improvised bandage | 4 | heal | Cuvier tubules |
| 26 | Improvised bandage | 4 | heal | Cuvier tubules |
| 27 | Sticky touch | 4 | block, multi-target | Colloblasts |
| 28 | Poison touch | 5 | attack, long-lasting | Toxins |
| 29 | Silt coating | 3 | antiblock, multi-target | Fins |
| 30 | Jaw ejection | 4 | attack, multi-target | Teeth + Evisceration |
| 31 | Poison bite | 5 | attack, long-lasting | Teeth + Toxins |
| 32 | Eerie shouting | 4 | attack, multi-target | Mechanoreception + Evisceration |
| 33 | Body bloat | 5 | attack, multi-target | Gigantism + Fins |
| 34 | Improvised lasso | 5 | attack, multi-target | Colloblasts + Cuvier tubules |
| 35 | Wound healing | 5 | heal, multi-target | Colloblasts + High immunity |
| 36 | The secret of longevity | 5 | heal, multi-target | Red pigmentation + High immunity |
| 37 | Distracting dance | 4 | block, multi-target | Pheromones + Bioluminescence |
| 38 | Fast flashing | 4 | block | Gelatinity, mucus + Bioluminescence |
| 39 | Counter-illumination | 4 | antiblock, multi-target | Transparency + Bioluminescence |
| 40 | Disorientation | 5 | attack, multi-target | Black pigmentation + Ink bag |
| 41 | Blind needle attacks | 4 | trap | Cirri, needles + Regeneration |
| 42 | Scary camouflage | 5 | heal, block | Tentacles, suckers + Mimicry |
| 43 | Pulling pincers out | 5 | attack, block | Pedicellariae + Intensive development |

## Notes

- A skill that combines effects carries several icons, for example Thanatosis is both an attack and a block.
- The ID is the skill's internal number in the game. The numbering has no skill 7.
- Skills 25 and 26 share the name Improvised bandage.
