---
layout: default
title: Game Design
nav_order: 4
---

# Game Design

## This page covers how we think over the mechanics. The project is updating everyday and our game design is subject to change. But before that, have fun!

1. [Learnings](#learnings)
2. [One-Page Design Document](#one-page)
3. [Prototype 1: Virus vs. Cells](#virus)
4. [Prototype 2: Treehouse](#treehouse)

---

## Learnings <a name="learnings"></a>

By looking into existing games we are able to find many patterns that make a game fun to play and watch and most importantly, to share things.

## LocoRoco 1 & 2

### Level design

- The level itself is not super complicated, but with challenges like collectibles and hidden paths the level has depth. In our prototype, we want to do less difficult levels too because our target audience are not all hardcore players.
- Most levels give the player chances to retry. LocoRoco is an action-based game with some sort of requirement for precise control. Always leaving room for retry can help those who fail in the first try. We think it does not necessarily mean “going back”, but just leaving appropriate difficulty level.
- Many “automatic” elements. “Automatic” means places where the player generally don’t need to do anything and the physics in the game will carry LocoRocos through. This is very fun to watch and gives players time for a short break. We can do the same for our game.
  ![LocoRoco](https://etc-ditto.github.io/media/reference/locoroco-2.PNG)
  <h5 style="text-align: center;">A waterstream that carries you in a beautiful curve.</h5>
- Linear in “automatic” parts and many easy parts, branching in places for exploration. The level itself also splits and merges back.
- Simple puzzles: one that encourages a little thinking, preferably splitting or merging. ![LocoRoco](https://etc-ditto.github.io/media/reference/locoroco-1.PNG)
  <h5 style="text-align: center;">A level where you jump between seesaws.</h5>

### System design

- Splitting and merging LocoRocos serves more like a surprise and user experience part in puzzles: yes you need to split in order to beat the level, but it is really simple. In our prototype, as each cell will be controlled by a player, we can add more puzzle elements to make everyone feel they are contributing to all. The puzzle should not be overwhelming though.
- Rewarding for requirements. In LocoRoco there are obstacles that need a certain number of LocoRocos to unlock. This is a direct ask for accumulated skills and patience. ![LocoRoco](https://etc-ditto.github.io/media/reference/locoroco-3.PNG)
  <h5 style="text-align: center;">A scale that can only be triggered with at least 18 Locorocos.</h5>
- Collectibles. Collectibles make up the most challenging part in LocoRoco as designers place them in less spottable places and it takes skills to get them. In our game, the collectibles are mainly “triggers” in the level as we don’t have to make an open-world game but to realize State Share function.
- Granting players chances to make up for something wrong. When a LocoRoco got eaten by monsters they have a short time to strike back, kill the monster and regain the lost piece.
- Highly stylish physics: low friction makes it feel really good to slide and jump.

### Very strong feedback

- Jumping and merging shakes the camera which gives strong physical feedback. To split the game creates a lightning effect in the background and is visually very impressive.
- Also, the camera zooms in and out.
- Visual hints if two LocoRocos are away from each other. This reminds players not to forget their fellows.

---

## One Page Design Document <a name="one-page"></a>

As suggested by the client, we created one-page design document that describes the overall mechanics for each of 5 ideas and showed them to the guests during the quarters. One-page design document is a nice way to conclude our thoughts and present them in an relatively appealing way. Check the hyperlink to see each. <br>

- <a href="https://etc-ditto.github.io/media/process/virus-cell.png" target="_blank">Virus vs Cell</a>
- <a href="https://etc-ditto.github.io/media/process/animal-inn.png" target="_blank">Animal Inn</a>
- <a href="https://etc-ditto.github.io/media/process/bomb.png" target="_blank">Bomb Express</a>
- <a href="https://etc-ditto.github.io/media/process/photo-leap.png" target="_blank">Photo Leap</a>
- <a href="https://etc-ditto.github.io/media/process/manor.png" target="_blank">Escape from Timelock Manor</a>

---

## Virus vs. Cell <a name="virus"></a>

Virus vs. Cell is a streaming-based platformer game where streamers and audience play in the same world (inside human body) using State Share feature to synchronize all the game data.

### Core Gameplay

Split. Play together AND separately. Merge. <br> In Virus vs. Cell everyone except the host starts off as a cell splinted from another player. The game host, who starts the game, controls a mother cell who needs other players' help to do the tasks. At some certain point the mother cell can split into two and the host can invite audience or friends to join in and play as the daughter cell.

### Level Design

Every separate cell travels in a big map and collects nutrients for the human body. At some point where the tunnel is too narrow, they will have to splint and invite another player to play a daughter cell for them. The big map is composed of several small task maps and there are meeting places for cells to hand in collectibles and merge other cells back into a bigger one.<br> The map, with a theme of inside human body, has many platforms and fields that adds fun to the travelling.

- The level is built with State Share in mind. The cells need to split at the beginning of each separate level and merge back again.
- Jumping is an essential action for most of the levels.
- Occasional force fields simulates the blood circulation, and is a map mechanic that allows the cell to travel between distant places.
- Many platforms that cell can jump onto encourage players to explore the world. There are always more collectible in each map than the level requirement, and the system will award players that make a bigger contribution.

### Next Step

- More cell subdivisions. Red cells, T-cells, etc.
- More competitive elements: the cells and virus can fight each other.

---

## Treehouse <a name="treehouse"></a>

Treehouse is a casual collaborative game where players feed the Tree of Life and build houses on the tree. They use State Share to invite others to join in so as to collect more resources and build a large, fancy world.

### Inspiration

We got this idea from the game [One Hour One Life](https://store.steampowered.com/app/595690/One_Hour_One_Life/) made by Jason Rohrer. That game is a survival game where players only have one hour to experience the life from 0 to 60 and try not to get killed or starve during their time slot.

![One-Hour](https://etc-ditto.github.io/media/reference/one-hour-1.jpg)

<h5 style="text-align: center;">How you age in One Hour One Life.</h5>

### Core Gameplay

Live. Collect. Build.<br> This game introduces a hierarchy where the game holder is immortal while the people they invite have limited lifetime so they will switch to viewers and wait for someone else to invite them again. In their playtime, players obtain resources to craft tools and found buildings.

### System Design

- Time Limit: Everyone except the elder has the exact same expected lifetime. They will die after a certain amount of time (maybe earlier) and they become a viewer then, but they can still be called back into the game if someone invites them again. This makes sure that the game is hosted in a familiar community, not squeezed with random people that may ruin your process.
- Human Resource: The game has a hierarchy where the elder is technically immortal and have the overall control of game. The elder could invite a limited number of people as managers. Managers will die but also have some control over an area in the treehouse. The managers could also invite new players who will be workers. All people in the game have the same group goal - build a fancy tree, while their individual tasks and pursue may be different. Inviters could get referral bonus. Progress-based events would happen, setting up new challenges.
- Gathering System: Players can go deep underground to find water source and fertilizers for the tree, and they can build houses on the tree that collects sunlight automatically.
  The resources are used both for keeping the tree alive and adding new things.
- Synthesis System: In general, you combine low-level materials for high-level items. Starting with basic materials that can be gained from mining, collecting, farming, you synthesize them to make houses, infrastructures, and decorations. The result of synthesis is pre-determined just like Minecraft and Doodle God.
- PVP System: As the tree grows higher and stronger with larger capacity for people, you may find players around you who also have their own trees. You could send messages, trade, or fight them.
- Possible installations: We would love to see a physical system that simulates the weather and affects the tree. We are also thinking combining treehouse with Virus vs. Cell idea.
