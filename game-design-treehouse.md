---
layout: default
title: Game Design - Treehouse
nav_order: 5
---

# Game Design - Treehouse

## This page covers introduces Treehouse, our second prototype's game design.

1. [Overview](#overview)
2. [System Design](#system)
3. [Map Design](#map)
4. [Post Mortem](#pm)

## Overview <a name="treehouse"></a>

Treehouse is a casual collaborative game where players feed the Tree of Life and build houses on the tree. They use State Share to invite others to join in so as to collect more resources and build a large, fancy world.

Everyone except the game holder has limited playtime during which they can explore the map and collect and build things. Upon their death they need to introduce others into the game and continue for the long-term goal.

---

## System Design <a name="system"></a>

- One player acts as the "tree" (also the game host) who never dies and is ever-growing. The game host invites other players into the game and play as the elves who roam underground and collect resources to help the tree.
- The map consists of two parts: the ground part where the tree grows its part and elves build things; the underground part covered by blocks where different types of resources (water and fertilizer) are distributed and ready to collect.
- Each turn (one day in game) elves travel up to three blocks and uncover the blocks. If there are fertilizers they obtain them, but for discovered water resources the tree needs to grow its root to touch the water in order to get the resource.
- The weather changes every day. In sunny days the leaves on tree will produce sunlight while in cloudy or rainy days they are unable to do that.
- The tree uses one of each type of resources to grow up to three parts of itself.
- The elves uses two resources of any kind to build facilities on or off the tree.

---

## Map Design <a name="map"></a>

![Treehouse](https://etc-ditto.github.io/media/process/treehouse-1.jpg)

<h5 style="text-align: center;">The paper prototype of our Treehouse prototype.</h5>

---

## Post Mortem <a name="pm"></a>

Almost all playtesters agreed that the game was designed in a quite novel way to encourage people to communicate and share information with each other, and we're satisfied that most players seemed engaged throughout the whole process. For this one, when comparing to Virus vs. Cell on which one to continue to develop in the second half of the semester, we just found it more technically challenging if we wanted to fully implement the features in digital prototype. There are a lot of cool things we wanted to do in Treehouse (and there are already a lot)
