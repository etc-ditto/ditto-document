---
layout: default
title: Game Design
nav_order: 4
---

# Game Design

## This page covers detailed discussions on our games' mechanics.

1. [Prototype Phase 1](#phase1)
2. [Prototype 1: Virus vs. Cells](#virus)
3. [Prototype 2: Treehouse](#treehouse)
4. [Immunoo](#immunoo)

---

## Prototype Phase 1 <a name="phase1"></a>

We had in total five ideas in the first ideation phase and as suggested by the client, we created one-page design document for each to depict the overall mechanics and game flow. In this stage we mainly focused on finding interesting mechanics to implement the State Share feature.

During quarter walkaround, we showed and explained these five documents to our guests and faculty and students who also gave positive feedback and thoughtful opinions.
Check the hyperlink to see each. <br>

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

Immunoo is a multiplayer casual action game with some RPG elements where players acts as white blood cells who must clear the map of biological contaminants (typically viruses) in order to keep the body safe.

### Core Gameplay

Players are granted the freedom of wandering through different levels where they need to find and eat viruses.

### System Design

- Splitting: The players have the chance of splitting the cells and inviting others to join in the game with State Share feature. The players need to find lymph nodes in the game and attach to the lymph nodes in order to split and send the invitation link outside the game. Each new player is put into a separate game state, meaning they will not see each other and enjoy the level to its full.
- Inheritance: The cell can learn different skills either by collecting power-ups in the game, or when someone shares the link to the player, they will inherit one skill from the parent cell. The skill is saved with player's profile so it will not disappear after leaving the game. The more games you join, the more skills you will obtain.
- Bloodstream: Bloodstream is a unique game element that acts both a boon and an obstacle to players. Additionally, the bloodstream is rhythmed due to the nature of heartbeat, thus at the right timing the players could use the bloodstream as a help.

### Level Design

The game by concept has a heart map with four integrated chambers. All but the last chamber is designed for single-player experience, with increasing difficulty for players. The last chamber is designated to be the boss fight, with a preparation room which technically serves as a place for players to invite their friends/audience and team up before entering the boss room.
