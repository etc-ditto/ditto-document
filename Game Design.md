---
layout: default
title: Game Design
nav_order: 4
---

# Game Design

## The project is updating everyday and our game design is subject to change. But before that, have fun!

1. [Learnings](#learnings)
2. [Prototype 1: Virus vs. Cells](#virus)
3. [Prototype 2: One Hour One Life](#one-hour)

---

## Learnings <a name="learnings"></a>

By looking into existing games we are able to find many patterns that make a game fun to play and watch, and most importantly, to share things.

## LocoRoco 1 & 2

- ### Level design
  - The level itself is not super complicated, but with challenges like collectibles and hidden paths the level has depth. In our prototype, we want to do less difficult levels too because our target audience are not all hardcore players.
  - Most levels give the player chances to retry. LocoRoco is an action-based game with some sort of requirement for precise control. Always leaving room for retry can help those who fail in the first try. We think it does not necessarily mean “going back”, but just leaving appropriate difficulty level.
  - Many “automatic” elements. “Automatic” means places where the player generally don’t need to do anything and the physics in the game will carry LocoRocos through. This is very fun to watch and gives players time for a short break. We can do the same for our game.
  - Linear in “automatic” parts and many easy parts, branching in places for exploration. The level itself also splits and merges back.
- ### System design
  - Splitting and merging LocoRocos serves more like a surprise and user experience part in puzzles: yes you need to split in order to beat the level, but it is really simple. In our prototype, as each cell will be controlled by a player, we can add more puzzle elements to make everyone feel they are contributing to all. The puzzle should not be overwhelming though.
  - Rewarding for requirements. In LocoRoco there are obstacles that need a certain number of LocoRocos to unlock. This is a direct ask for accumulated skills and patience.
  - Collectibles. Collectibles make up the most challenging part in LocoRoco as designers place them in less spottable places and it takes skills to get them. In our game, the collectibles are mainly “triggers” in the level as we don’t have to make an open-world game but to realize State Share function.
  - Granting players chances to make up something wrong. When a LocoRoco got eaten by monsters they have a short time to strike back, kill the monster and regain the lost piece.
  - Highly stylish physics: low friction makes it feel really good to slide and jump.
- ### Very strong feedback
  - Jumping and merging shakes the camera which gives strong physical feedback. To split the game creates a lightning effect in the background and is visually impressive.
  - Also, the camera zooms in and out.
  - Visual hints if two LocoRocos are away from each other. This reminds players not to forget their fellows.

---

## Virus vs. Cell <a name="virus"></a>

Virus vs. Cell is a steaming-based multiplayer game where streamers and audience play in the same world (human body) using State Share feature to synchronize all the game data.

### Core Gameplay

Split. Play together AND separately. Merge. <br>
In Virus vs. Cell everyone except the host starts off as a cell splinted from another player. The game host, who starts the game, controls a mother cell who needs other players' help to do the tasks. At some certain point the mother cell can split into two and the host can invite audience or friends to join in and play as the daughter cell.

### Level Design

Every separate cell travels in a big map and collects nutrients for the human body. At some point where the tunnel is too narrow, they will have to splint and invite another player to play a daughter cell for them. The big map is composed of several small task maps and there are meeting places for cells to hand in collectibles and merge other cells back into a bigger one.<br>
The map, with a theme of inside human body, has many platforms and fields that adds fun to the travelling.

- The level is built with State Share in mind. The cells need to split at the beginning of each level and merge back again.
- Jumping is an essential action for most of the levels.
- Occasional force fields simulates the blood circulation, and is a map mechanic that allows the cell to travel between distant places.
- Many platforms that cell can jump onto encourage players to explore the world. There are always more collectible in each map than the level requirement, and the system will award players that make a bigger contribution.

---

## One Hour One Life <a name="one-hour"></a>

One Hour One Life is a multiplayer casual collaborative game where players feed the Tree of Life and build houses on the tree. They invite others to join in so as to collect more resources and build a larger, fancier world. The only limitation is that everyone except the game holder only has limited playtime after which they have to switch to viewers waiting for someone else to invite them again.

### Core Gameplay

Invite. Collect. Build.<br>
