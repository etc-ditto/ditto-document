---
layout: default
title: Design Process
nav_order: 3
---

# Design Process

## Design Process covers the whole iterative stages from researching to production.

1. [Research](#research)
2. [Ideation](#ideation)
3. [Paper Prototype](#paper-prototype)
4. [Digital Prototype](#digital-prototype)
5. [Final Prototype](#final-prototype)

---

## Research <a name="research"></a>

The main purpose of researching is to get the knowledge of Stadia and State Share and figure out several possible usage situations.<br>
As Stadia just came out a few months ago and the team are still working to realize State Share feature, we started off mainly by searching the internet for the documentation and demo videos of State Share. There are a few resources we found very useful: the first is [[Stadia development blog](https://stadia.dev/intl/en_us/blog/) and [State Share explanation](https://stadia.dev/blog/the-magic-of-state-share-explained/) where we can have a broad view of what Stadia is, how State Share works and several possible usage of the function.

---

## Ideation <a name="ideation"></a>

During ideation phase we specified the genre that could potentially fit the situations mentioned in our research. Our approach was to think of ideas at a higher level that use State Share as a main mechanism. There were 10 scenes that we think could be possible for implementing State Share. <br>
We went through each scene on its feasibility, novelty and how close is State Share related to the theme. And we choose five categories to move on to the theming stage where we wanted to come up with more specific gameplay that uses the feature. By the end of Week 2 we got the following: geographic/location-based, community-based coop, asymmetric multiplayer, time travel/version control, transition between devices.<br> As part of our plan and client's suggestion, We planned to create a one-page design document for each and try making paper prototypes.
![Ideation](https://etc-ditto.github.io/media/process/idea-1.jpg)

---

## Paper Prototype <a name="paper-prototype"></a>

After narrowing down ideas, we begin making paper prototypes and do playtest both internally and with naive guests. This iteration phase is helpful to solidify our ideas.<br>
We make one page design document for each idea to better illustrate the conception to the audience, especially for those who are not familiar with Stadia. We eventually built 4 paper prototypes as following:

- **Sharing Information (Photo Leap, Haunted House)**: like most multiplayer games, the game synchronizes data and passes the end of last state to the next player.<br>
- **Geographic/location-based Multiplayer (Animal Inn)**: We think of ways to connect players around the world to play together using State Share. Animal Inn is an idea where people raise pets and "send" them to others for a short time.<br>
- **State Tagging (Bomb Express)**: To let players pass a game back and forth by delivering the state to the next player after a time period. Our idea was to make a game where player pass ticking bombs like a hot potato.<br>

The shortcomings of some of our ideas is that they are not fully using the feature of State Share: recording complete progress and carry a bunch of information. And we need also to think about the replayability and theme and privacy problems.

---

## Learnings

We got a lot of valuable information from our client, faculty advisors and playtesters. Here is the three criteria that we think as the key to a (potentially) successful State Share game:

1. Asymmetrical gameplay is suitable for streamer and audience and well conveys State Share’s idea.
2. Having a persistent world (like MMO) is state sharable and could let players feel more immersed.
3. To make multiplicative distribution rather than transferring a single branch to new players.
   UGC game requires more system design to control the game, and platformers really need decent levels.

---

## Prototypes before Halves <a name="digital-prototype"></a>

After we narrow down ideas into two big categories, we begin to make the demo prototype for the incoming halves in Week 8. We all agree to make a digital prototype for the Virus vs. Cell idea for the following reasons: <br>

1.  Some ideas are hard to paper prototype, even for those paper prototype-able ones it does not wholly match the feeling we want. <br>
2.  Digital prototypes offer insights into controlling and feedback which paper prototype cannot give. <br>
3.  As the project progresses, we need to settle down on art style and hardware as our final deliverable will be a digital game, so it is good to start early exploring possible approaches for the ideas. <br>

### Game: Virus vs Cell

In this prototype we are testing out much stuff, but more specifically:

1. For designers, to confirm that the level and gameplay works well together and implements State Share as one of the core mechanism.
2. For engineers, to test technical solutions for State Share (at least faking it) such as separate control for individual player, split screen, and the fundamental splint and merge function.
3. For artists, to try different ways of simulating responsive, interesting graphics to make the world feel real.

![Cells](https://etc-ditto.github.io/media/process/cells-1.png)

<h5 style="text-align: center;">Map that we prepare for the playtest before halves.</h5>
In this early version we are building the first part of the idea: the virus camp collect power-ups and prepare for the fight with cells. The player can explore different levels and try getting collectibles many as possible by jumping in this 1-minute experience.

### Game: Treehouse

On the other side, we would like to make a paper prototype for the second idea for the following reasons:

1. We actually only have less than 2 weeks before halves for the two prototypes, and we want the project to be on a good balance without leaving any of two prototypes behind.
2. The Treehouse idea is feasible for paper prototyping as its core gameplay is pretty clear and understandable even on paper.
3. We don't need to test every details. Instead we focus on the "share" part and everything we do for paper prototype can be transferred easily to Unity.

We would like to theme this idea as growing a tree: there is one immortal elder in charge of the whole ecosystem, and they invite elves (basically workers) to play the game for a limited time. They work together to collect resource underground, branch the tree, and build houses and facilities. When an elf dies, they can pass their data to another player but also keep their work remaining in the world.<br>
The game also has a weather system which adds factors that affect the resources and have random events.

![Treehouse](https://etc-ditto.github.io/media/process/treehouse-1.jpg)

<h5 style="text-align: center;">The paper prototype of our Treehouse idea.</h5>

## Final Prototype <a name="final-prototype"></a>

Everything's changed a lot as we finished our half presentation and enjoyed the mid-semester break during which we realized we had to work remotely for the safety reasons. Our client, Erin, in the virtual meeting confirmed our work so far and suggested that we continue to polish our game and make a short clip about it demonstrating the core features and mechanics.

With her advice, we partly pivoted our focus of the final prototype to instead of making multiple maps, using a relatively short but essential level to showcase our design ideas, art style, and user interaction.
