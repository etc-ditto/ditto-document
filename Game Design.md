---
layout: default
title: Game Design
nav_order: 4
---

# Game Design

## This page covers detailed discussions on our prototypes' game design.

1. [Prototyping Phase 1](#phase1)
2. [Prototype 1: Virus vs. Cells](#virus)
3. [Prototype 2: Treehouse](#treehouse)
4. [Immunoo](#immunoo)

---

## Prototyping Phase 1 <a name="phase1"></a>

We had in total five ideas in the first prototyping phase. In this stage we mainly focused on finding interesting mechanics where the State Share feature is suitable to be implemented. Also per our client's suggestion, we created one-page design documentation for each to depict the overall mechanics and game flow.

During quarter walkaround, we showed and explained these five documents to our guests who also gave positive feedback and thoughtful opinions.
Click on the hyperlink to find out. <br>

- <a href="https://etc-ditto.github.io/media/process/virus-cell.png" target="_blank">Virus vs Cell</a>
- <a href="https://etc-ditto.github.io/media/process/animal-inn.png" target="_blank">Animal Inn</a>
- <a href="https://etc-ditto.github.io/media/process/bomb.png" target="_blank">Bomb Express</a>
- <a href="https://etc-ditto.github.io/media/process/photo-leap.png" target="_blank">Photo Leap</a>
- <a href="https://etc-ditto.github.io/media/process/manor.png" target="_blank">Escape from Timelock Manor</a>

---

## Virus vs. Cell <a name="virus"></a>

Virus vs. Cell is a streaming-based platformer game where streamers and audience play in the same world (inside human body) using State Share feature to synchronize all the game data.

### Core Gameplay

Split. Play together and separately. Merge. <br> In Virus vs. Cell everyone controls either a cell or virus to perform tasks in order to defeat the other side and protect/infect the human body. State Share feature will be used to transfer the control of split cells and also to regain the control when merging.

### Camps

There are two camps in the game: virus and white blood cells. Ideally the lead of each camp will be played by a YouTube streamer who has access to the Stadia's platform exclusive features. The streamers, who are also the game host that run the game in the first place, controls a mother virus/cell that can split into smaller viruses/cells and send invitation links. The audience who click on the link will be able to jump into the current game phase and play as daughter viruses/cells.

### Setup & Goals

The game simulates the battle between viruses and cells inside human's body. The viruses and cells starts off somewhere inside human body, with only one streamer playing each side.

The game is overall like a race between virus and cells. The win condition for the white blood cells is to kill enough viruses so that they cannot infect the heart. The win condition for the viruses is to get to the heart and infect enough cells there.

### System Design

- Splitting

  - Cells/viruses may only split at certain locations.
  - "Infecting" a cell: cells have a certain receptor on their body that when viruses touch it, they got converted into a virus. This is how viruses split.
  - Everytime when viruses split, they leave a "trail" or signal, which the white blood cells can find.
  - Cells may split in more places where they need to.

- Merging

  - "Clone Machine": it is a mechanism that allows people to share a portion of their bio mass with others, instead of simply getting merged into another player and losing all control.
  - Cells may merge viruses into themselves in order.

- Permanent Infrastructure
  - After cells reach a particular destination, they can start to build defense facilities to hinder viruses from moving forwards freely.

### Level Design

Every separate cell travels in a big map and collects nutrients for the human body. At some point where the tunnel is too narrow, they will have to splint and invite another player to play a daughter cell for them. The big map is composed of several small task maps and there are meeting places for cells to hand in collectibles and merge other cells back into a bigger one.<br> The map, with a theme of inside human body, has many platforms and fields that adds fun to the travelling.

- The level is built with State Share in mind. The cells need to split at the beginning of each separate level and merge back again.
- Jumping is an essential action for most of the levels.
- Occasional force fields simulates the blood circulation, and is a map mechanic that allows the cell to travel between distant places.
- Many platforms that cell can jump onto encourage players to explore the world. There are always more collectible in each map than the level requirement, and the system will award players that make a bigger contribution.

### Possible Improvements

- More cell and enemy subclasses: red cells, T-cells, bacteria, parasite, etc.
- More exciting elements: the cells and virus can fight each other.

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

---

## Immunoo <a name="immunoo"></a>

Immunoo is a multiplayer casual action game with some RPG elements where players team up as white blood cells who must clear the map of biological contaminants (typically viruses) in order to keep the body safe.

### Core Gameplay

Players team up to go through levels in a heart-shaped map and try to eat viruses and beat the final boss.

### Expected Number of Players

The question on the numbers of our game was an important one we need to answer: due to the nature of State Share's feature that can drag people into the game, it would be great if some game mechanism is more multiplayer-friendly. However, we don't want the number too large which may make the map too crowded and impact everyone's experience. We especially

We figured out that six players would be an ideal number, with a minium of four and a maximum of eight. The game will be still playable with less than four or more than eight, but in some area the game may not feel as smooth.

Having this interval in mind we are also trying to dynamically adjust the difficulty in the final boss battle, like increasing or decreasing the child viruses' number.

### System Design

- **State Share Replication**: The players have the chance of splitting the cells and inviting others to join in the game with State Share feature. The players need to find lymph nodes in the game and attach to the lymph nodes in order to split and send the invitation link outside the game. Each new player is put into a separate game state, meaning they will not see each other and enjoy the level to its full.
- **Inheritance**: The cell can learn different skills either by collecting power-ups in the game, or when someone shares the link to the player, they will inherit one skill from the parent cell. The skill is saved with player's profile so it will not disappear after leaving the game. The more games you join, the more skills you will obtain.
- **More Cells, More Power!**: Players will eliminate viruses from the map the same way white blood cells do in real life: by eating them. The gameplay is oriented around absorbing viruses and their chemical trails to both eliminate contaminants and recruit more players into the game state. Some mechanics require multiple players to collectively complete and will offer better rewards.
- **Environmental Effects**: Since the game take place inside human body, we are creating each map with its own unique qualities and hazards. For instance, in the heart, players are subject to the rhythms of the blood stream. Bloodstream is a unique game element that acts both a boon and an obstacle to players, dependent on the timing. But in the stomach, players must avoid stores of acid found around the map.

### Level Design

The game by concept has a heart map with four integrated chambers.

![In-engine prototype](https://etc-ditto.github.io/media/process/level-3.png)

<h5 style="text-align: center;">The level design of heart.</h5>

Inspired by our client's suggestion, we use Nintendo's IPM model (Introduce, Practice, Master) as a principle in designing the levels. All chambers are designed for multiplayer experience, with increasing demands for skill mastery from players. The increasing difficulty mainly means more enemies and more complex mechanics in the later chambers.

The last chamber is designed to be the boss fight room, with a preparation room in front of it which technically serves as a place for players to invite their friends/audience and team up before entering the boss room.

The boss fight's mechanics are partly different from previous experience because we want to make it more intense and make players feel the connection between each other and the necessity of sharing and helping others. The powerful mother virus is in invulnerable at the beginning, players will have to eat all the surrounding child viruses in order to make it vulnerable and surround it again to disintegrate and "kill" it.
