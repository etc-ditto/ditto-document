---
layout: default
title: Game Design
nav_order: 4
---

# Game Design
## The project is running and our game design is subject to change. But before that, have fun! 

1. [Learnings](#learnings)
   
---
## Learnings <a name="learnings"></a>
By looking into existing games we are able to find many patterns that make a game fun to play and watch, and most importantly, to share things.
## LocoRoco 1 & 2
- ### Level design
  - The level itself is not super complicated, but with challenges like collectibles and hidden paths the level has depth. In our prototype, we want to do less difficult levels too because our target audience are not all hardcore players.
  - Most levels give the player chances to retry. LocoRoco is action-based with some sort of requirement for precise control. Always leaving room for retry can help those who fail in the first try. We think it does not necessarily mean “going back”, but just leaving appropriate difficulty level.
  - Many “automatic” elements. “Automatic” means places where the player generally don’t need to do anything and the physics in the game will carry LocoRocos through. This is very fun to watch and gives players time for a short break. We can do the same for our game.
  - Linear in “automatic” parts and many easy parts, branching in places for exploration. The level itself also splits and merges back.
- System design
  - Splitting and merging LocoRocos serves more like a surprise and user experience part in puzzles: yes you need to split in order to beat the level, but it is really simple. In our prototype, as each cell will be controlled by a player, we can add more puzzle elements to make everyone feel they are contributing to all. The puzzle should not be overwhelming though.
  - Rewarding for requirements. In LocoRoco there are obstacles that need a certain number of LocoRocos to unlock. This is a direct ask for accumulated skills and patience.
  - Collectibles. Collectibles make up the most challenging part in LoroRoco as designers place them in less spottable places and it takes skills to get them. In our game, the collectibles are mainly “triggers” in the level as we don’t have to make an open-world game but to realize State Share function.
  - Granting players chances to make up something wrong. When a LocoRoco got eaten by monsters they have a short time to strike back, kill the monster and regain the lost piece.
  - Highly stylish physics: low friction makes it feel really good to glide and jump.
- Very strong feedback
  - Jumping and merging shakes the camera which gives strong physical feedback. To split the game creates a lightning effect in the background and is visually impressive.
  - Also, the camera zooms in and out.
  - Visual hints if two LocoRocos are away from each other. This reminds players not to forget their fellows.
