---
layout: default
title: Game Design - Virus vs. Cell
nav_order: 4
---

# Game Design - Virus vs. Cell

## This page covers Virus vs. Cell, our very first digital prototype's game design.

1. [Overview](#overview)
2. [System Design](#system)
3. [Level Design](#level)
4. [Post Mortem](#pm)

---

## Overview <a name="overview"></a>

Virus vs. Cell is a streaming-based platformer game where streamers and audience play in the same world (inside human body) using State Share feature to synchronize all the game data.

Split. Play together and separately. Merge. <br> In Virus vs. Cell everyone controls either a cell or virus to perform tasks in order to defeat the other side and protect/infect the human body. State Share feature will be used to transfer the control of split cells and also to regain the control when merging.

---

## System Design <a name="system"></a>

- Setup & Goals

There are two camps in the game: viruses and white blood cells. Ideally the lead of each camp will be played by a YouTube streamer who has access to the Stadia's platform exclusive features. The streamers, who are also the game host that run the game in the first place, controls a mother virus/cell that can split into smaller viruses/cells and send invitation links. The audience who click on the link will be able to jump into the current game phase and play as daughter viruses/cells.

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

---

## Level Design <a name="level"></a>

Every separate cell travels in a big map and collects nutrients for the human body. At some point where the tunnel is too narrow, they will have to splint and invite another player to play a daughter cell for them. The big map is composed of several small task maps and there are meeting places for cells to hand in collectibles and merge other cells back into a bigger one.<br> The map, with a theme of inside human body, has many platforms and fields that adds fun to the travelling.

- The level is built with State Share in mind. The cells need to split at the beginning of each separate level and merge back again.
- Jumping is an essential action for most of the levels.
- Occasional force fields simulates the blood circulation, and is a map mechanic that allows the cell to travel between distant places.
- Many platforms that cell can jump onto encourage players to explore the world. There are always more collectible in each map than the level requirement, and the system will award players that make a bigger contribution.

---

## Post Mortem <a name="pm"></a>

- More cell and enemy subclasses: red cells, T-cells, bacteria, parasite, etc.
- More exciting elements: the cells and virus can fight each other.
