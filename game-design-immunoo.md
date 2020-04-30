---
layout: default
title: Game Design - Immunoo
nav_order: 6
---

# Game Design - Immunoo

## This page introduces every bit of Immunoo, our final prototype's game design!

1. [Overview](#overview)
2. [Player Number](#number)
3. [System Design](#system)
4. [Level Design](#level)
5. [Update Plan](#plan)
6. [Post Mortem](#pm)

## Overview <a name="overview"></a>

Immunoo is a multiplayer casual action game with some RPG elements where players team up as white blood cells who must clear the map of biological contaminants (typically viruses) in order to keep the body safe. Players team up to go through levels in a heart-shaped map and try to eat viruses and beat the final boss.

---

## Expected Number of Players <a name="number"></a>

The question on the numbers of our game was an important one we need to answer: due to the nature of State Share's feature that can drag people into the game, it would be great if some game mechanism is more multiplayer-friendly. However, we don't want the number too large which may make the map too crowded and impact everyone's experience.

We figured out that six players would be an ideal number, with a minium of four and a maximum of eight. The game will be still playable with less than four or more than eight, but in some area the game may not feel as smooth.

Having this interval in mind we are also trying to dynamically adjust the difficulty in the final boss battle, like increasing or decreasing the child viruses' number.

---

## System Design <a name="system"></a>

- **State Share Replication**: The players have the chance of splitting the cells and inviting others to join in the game with State Share feature. The players need to find lymph nodes in the game and attach to the lymph nodes in order to split and send the invitation link outside the game. Each new player is put into a separate game state, meaning they will not see each other and enjoy the level to its full.
- **Inheritance**: The cell can learn different skills either by collecting power-ups in the game, or when someone shares the link to the player, they will inherit one skill from the parent cell. The skill is saved with player's profile so it will not disappear after leaving the game. The more games you join, the more skills you will obtain.
- **More Cells, More Power!**: Players will eliminate viruses from the map the same way white blood cells do in real life: by eating them. The gameplay is oriented around absorbing viruses and their chemical trails to both eliminate contaminants and recruit more players into the game state. Some mechanics require multiple players to collectively complete and will offer better rewards.
- **Environmental Effects**: Since the game take place inside human body, we are creating each map with its own unique qualities and hazards. For instance, in the heart, players are subject to the rhythms of the blood stream. Bloodstream is a unique game element that acts both a boon and an obstacle to players, dependent on the timing. But in the stomach, players must avoid stores of acid found around the map.

---

## Level Design <a name="Level"></a>

The game by concept has a heart map with four integrated chambers.

![In-engine prototype](https://etc-ditto.github.io/media/process/level-all.png)

<h5 style="text-align: center;">The level design of heart.</h5>

Inspired by our client's suggestion, we use Nintendo's IPM model (Introduce, Practice, Master) as a principle in designing the levels. All chambers are designed for multiplayer experience, with increasing demands for skill mastery from players. The increasing difficulty mainly means more enemies and more complex mechanics in the later chambers.

The last chamber is designed to be the boss fight room, with a preparation room in front of it which technically serves as a place for players to invite their friends/audience and team up before entering the boss room.

The boss fight's mechanics are partly different from previous experience because we want to make it more intense and make players feel the connection between each other and the necessity of sharing and helping others. The powerful mother virus is in invulnerable at the beginning, players will have to eat all the surrounding child viruses in order to make it vulnerable and surround it again to disintegrate and "kill" it.

![Chamber 1](https://etc-ditto.github.io/media/process/chamber1.png)
Chamber 1 is the "Introduce" level. The players get carried by the bloodstream to board the level, and follow along the chemical signals left by the viruses to track down them. The nymph node is placed at a obvious location so players would be attracted and try to use it. This level is relatively simple and straight forward, but there's also a skill collectible for curious players to try to find.

![Chamber 2](https://etc-ditto.github.io/media/process/chamber2.png)
Chamber 2 is the "Practice" level. We continue to introduce some more complex mechanics there such as the magnetism power. As players are more familiar with the virus's movement pattern (they escape when cells are near), we put more viruses in the second chamber to practice players' skills.

![Chamber 3](https://etc-ditto.github.io/media/process/chamber3.png)
Chamber 3 is the "Master" level. More viruses are there and as we introduce the camouflage mechanic, we are asking players to be more aware of the surrounding environment to find collectibles that allows them to get the "supervision" skill to find the disguised virus. The environmental effect is also more challenging there.

![Chamber 4](https://etc-ditto.github.io/media/process/chamber4.png)
Chamber 4 in our plan is the to-be boss fight level where we introduce mass battle mechanics and ask players to invite people to team up for the final battle. The mother virus has new skills child viruses don't have, but in general their skill pattern will be understandable if player have successfully gone through the previous levels because it's still asking for cell's movement control skills.

---

## Update Plan <a name="plan"></a>

We also have made the schedule for future DLC (downloadable content) releases.

---

## Post Mortem <a name="overview"></a>
