---
layout: default
title: Game Design
nav_order: 4
---

# Game Design

## This page covers the detailed discussion on our game mechanics.

1. [One-Page Design Document](#one-page)
2. [Prototype 1: Virus vs. Cells](#virus)
3. [Prototype 2: Treehouse](#treehouse)

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

### Core Gameplay

Everyone except the game holder has limited playtime during which they can explore the map and collect and build things. Upon their death they need to introduce others into the game and continue for the long-term goal.

### System Design

- One player acts as the "tree" (also the game host) who never dies and is ever-growing. The game host invites other players into the game and play as the elves who roam underground and collect resources to help the tree.
- The map consists of two parts: the ground part where the tree grows its part and elves build things; the underground part covered by blocks where different types of resources (water and fertilizer) are distributed and ready to collect.
- Each turn (one day in game) elves travel up to three blocks and uncover the blocks. If there are fertilizers they obtain them, but for discovered water resources the tree needs to grow its root to touch the water in order to get the resource.
- The weather changes every day. In sunny days the leaves on tree will produce sunlight while in cloudy or rainy days they are unable to do that.
- The tree uses one of each type of resources to grow up to three parts of itself.
- The elves uses two resources of any kind to build facilities on or off the tree.
