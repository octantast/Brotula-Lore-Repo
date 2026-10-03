# Creatures

A **creature** in Brotula is an enemy that blocks the explorer's way during a dive. Each species is built on a real deep-sea organism, and the species that can appear depend on the depth. A creature enters the fight with its brain cells already filled with the skills it will use.

Related files: [README](../README.md), [battle mechanics](../mechanics/battle.md), [skills](../skills/skills.md), [companions](../companions/companions.md).

## How creatures appear

- The dive is split into depth bands. At the start of each band the game picks one creature species from that band's list.
- Species names below are the internal names from the game files.
- Common species have a few percent each, and rare species have 1% each. In the first band the species Kridei, Batiz, Cirrat, Plog and Pharn have 6% each, Typhlon, Bent, Aliss, Abbet and Phobel have 5% each, and the rarest species of the list have 1% each.
- The deeper the dive, the shorter the list: shallow bands offer up to 44 species, the deepest band only 14.

## Species by depth

| Depth band (m) | Species that can appear |
|---|---|
| 5100 to 5300 | Abbet, Aliss, Babil, Batiz, Bent, Cellisee, Cirrat, Demos, Echin, Ekhir, Galan, Golor, Gren, Heeth, Hio, Khirond, Kridei, Lat, Lihet, Marius, Mikt, Nerrelid, Nophor, Pareed, Paster, Phanos, Pharn, Phiu, Phobel, Plog, Prokt, Sactin, Sciph, Sothet, Thanaid, Tkhar, Topel, Typhlon, Zem |
| 5300 to 5600 | the same species as above, plus Nemin, Popmp, Rago and Theus |
| 5600 to 6650 | the same species as in the previous band, plus Asce |
| 6650 to 8470 | Asce, Babil, Cellisee, Demos, Echin, Ekhir, Galan, Golor, Gren, Heeth, Hio, Khirond, Lat, Marius, Mikt, Nemin, Nerrelid, Nophor, Pareed, Paster, Phanos, Phiu, Prokt, Rago, Sactin, Sciph, Sothet, Thanaid, Theus, Tkhar, Topel, Zem |
| 8470 to 10500 | Asce, Cellisee, Demos, Ekhir, Galan, Golor, Hio, Khirond, Lat, Marius, Nemin, Nerrelid, Nophor, Pareed, Paster, Phiu, Prokt, Rago, Sactin, Sciph, Thanaid, Theus, Tkhar, Zem |
| 10500 to 12500 | Demos, Ekhir, Galan, Golor, Khirond, Marius, Nemin, Nerrelid, Paster, Sactin, Sciph, Thanaid, Tkhar, Zem |

In the deepest band Khirond, Golor, Marius and Demos are among the most frequent.

## Species with special behaviour

- **Theus** mimics the player. Its cells copy the skills of the player's last formation.
- **Marius** puts a skill into its first cell and, according to the game scripts, leaves the other cells empty.
- **Pareed** can draw its skills from the whole range at any depth.
- All other species draw from a skill range that widens and shifts with depth.

## Fish

In the band between 10500 and 11150 metres a dive can place a fish instead of a creature. According to the game scripts, a fish cannot be escaped from.

## Species in the game files without regular spawns

The names Hadee, Koryph, Roid and Themum exist in the game files, but the depth bands above do not spawn them.
