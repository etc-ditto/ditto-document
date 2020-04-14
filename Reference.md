---
layout: default
title: Reference
nav_order: 7
---

# Reference

## The reference page contains games and concepts that we had looked into and learned from for whatever better understanding of game design, multiplayer feature, or art style.

1. [LocoRoco](#locoroco)
2. [One Hour One Life](#one-hour)
3. [Concept Art](#concept-art)

## LocoRoco <a name="locoroco"></a>

LocoRoco is a platformer game developed by SCE Japan Studio. The player starts with a single LocoRoco which may be split into individual beings by pressing ○ key or through specific points on the level, while individual LocoRoco can merge back into a single being by holding down ○ key. Manipulation of the LocoRoco in this manner may be necessary to guide them to the finish; while the single large LocoRoco is easier to control, small passages can only be navigated by individual LocoRoco.

### Level design

- The level itself is not super complicated, but with challenges like collectibles and hidden paths the level has depth. In our prototype, we want to do less difficult levels too because our target audience are not all hardcore players.
- Most levels give the player chances to retry. LocoRoco is an action-based game with some sort of requirement for precise control. Always leaving room for retry can help those who fail in the first try. We think it does not necessarily mean “going back”, but just leaving appropriate difficulty level.
- Many “automatic” elements. “Automatic” means places where the player generally don’t need to do anything and the physics in the game will carry LocoRocos through. This is very fun to watch and gives players time for a short break. We can do the same for our game.

  ![LocoRoco](https://etc-ditto.github.io/media/reference/locoroco-2.PNG)

  <h5 style="text-align: center;">A waterstream that carries you in a beautiful curve.</h5>

- Linear in “automatic” parts and many easy parts, branching in places for exploration. The level itself also splits and merges back.
- Simple puzzles: one that encourages a little thinking, preferably splitting or merging.

![LocoRoco](https://etc-ditto.github.io/media/reference/locoroco-1.PNG)

  <h5 style="text-align: center;">A level where you jump between seesaws.</h5>

### System design

- Splitting and merging LocoRocos serves more like a surprise and user experience part in puzzles: yes you need to split in order to beat the level, but it is really simple. In our prototype, as each cell will be controlled by a player, we can add more puzzle elements to make everyone feel they are contributing to all. The puzzle should not be overwhelming though.
- Rewarding for requirements. In LocoRoco there are obstacles that need a certain number of LocoRocos to unlock. This is a direct ask for accumulated skills and patience.

![LocoRoco](https://etc-ditto.github.io/media/reference/locoroco-3.PNG)

  <h5 style="text-align: center;">A scale that can only be triggered with at least 18 Locorocos.</h5>
- Collectibles. Collectibles make up the most challenging part in LocoRoco as designers place them in less spottable places and it takes skills to get them. In our game, the collectibles are mainly “triggers” in the level as we don’t have to make an open-world game but to realize State Share function.
- Granting players chances to make up for something wrong. When a LocoRoco got eaten by monsters they have a short time to strike back, kill the monster and regain the lost piece.
- Highly stylish physics: low friction makes it feel really good to slide and jump.

### Very strong feedback

- Jumping and merging shakes the camera which gives strong physical feedback. To split the game creates a lightning effect in the background and is visually very impressive.
- Also, the camera zooms in and out.
- Visual hints if two LocoRocos are away from each other. This reminds players not to forget their fellows.

---

## One Hour One Life <a name="one-hour"></a>

[One Hour One Life](https://store.steampowered.com/app/595690/One_Hour_One_Life/) is a survival MMO game developed by individual developer Jason Rohrer. Each player lives for at most 60 minutes in a large, persistent world, with each minute representing a year of life. They must gather food, craft tools and build societies in order to survive. The main ideas influencing the game's design are player cooperation, sustainability and the prospect of developing a civilization.

![One-Hour](https://etc-ditto.github.io/media/reference/one-hour-1.jpg)

### System Design

- Time Limit: Everyone except the elder has the exact same expected lifetime. They will die after a certain amount of time (maybe earlier) and they become a viewer then, but they can still be called back into the game if someone invites them again. This makes sure that the game is hosted in a familiar community, not squeezed with random people that may ruin your process.
- Human Resource: The game has a hierarchy where the elder is technically immortal and have the overall control of game. The elder could invite a limited number of people as managers. Managers will die but also have some control over an area in the treehouse. The managers could also invite new players who will be workers. All people in the game have the same group goal - build a fancy tree, while their individual tasks and pursue may be different. Inviters could get referral bonus. Progress-based events would happen, setting up new challenges.
- Gathering System: Players can go deep underground to find water source and fertilizers for the tree, and they can build houses on the tree that collects sunlight automatically.
  The resources are used both for keeping the tree alive and adding new things.
- Synthesis System: In general, you combine low-level materials for high-level items. Starting with basic materials that can be gained from mining, collecting, farming, you synthesize them to make houses, infrastructures, and decorations. The result of synthesis is pre-determined just like Minecraft and Doodle God.
- PVP System: As the tree grows higher and stronger with larger capacity for people, you may find players around you who also have their own trees. You could send messages, trade, or fight them.
- Possible installations: We would love to see a physical system that simulates the weather and affects the tree. We are also thinking combining treehouse with Virus vs. Cell idea.

---

## Concept Art <a name="concept-art"></a>

[Slide of Visual Concept](https://docs.google.com/presentation/d/1_xwAPqd1bZhTzXND7o1ZQkxtBMlUvUiHlpaLceLsvUE)
