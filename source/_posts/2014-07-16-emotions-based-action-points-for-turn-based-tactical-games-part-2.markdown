---
layout: post
title: "Emotions-based Action Points for Turn-based Tactical Games. Part 2"
date: 2014-07-16 16:28:33 +0300
comments: false
categories:
- Tactical Games
- Mechanics
- Emotional Marbles
---

In a [previous post](/blog/2014/07/13/emotions-based-action-points-for-turn-based-tactical-games/) I started talking about a mechanic for using character emotions to determine which actions out of their pool they can use at any given time. 

In the next post I will try and plan a simplest possible prototypes for various implementations.

Now, read further for specifics. I will elaborate more on some aspects of that mechanic I want to try and test. There will also be some lists of implementation variants. 

[more]

## Color-coded marbles (or the part I like best)
So, in the start of each turn, all characters get a specific number of colored marbles representing their emotional state. Each character also has a pool of possible moves that "cost" a different number of differently colored marbles. Both moveset and marble-drop percentage depend on character build.

*complications and risks*:

- A lot of variety in movesets required. Each color needs some means of performing basic actions (movements, attacks) as well as excelling in it's own field.

- The whole marble system will not have a feel of being based on emotions, the player will handle it simply as multi-colored "action points" or "mana" (makes sense since the resemblance of MtG is significant)

- It will be hard to track a number of marbles each character has in a squad, so the player won't try to do that.

*variants*: 

- The marbles are drawn at the moment it's time to make a move for that specific character, not simultaneously for all.

- The number may either vary from character to character, based on attributes, or be predefined.

- The number of marbles of each color for each character is limited, meaning the Shuffle Bag is used to drawing them (may be nicely prototyped on the table), as a less random Random. When the marble is used it gets back in the bag. This variant kinda also makes the whole mechanic look even more like MtG ripoff.

- Basic actions require **any**(colorless) marble to be paid for it (also a good way to let characters get rid of marbles of unneeded color). 

- There is an additional "action point" colorless marble that shows how fast you can move. Each maneuver require you to pay some amount of both colorless(time) and colored(feelings) marbles, but basic actions need only colorless and instant actions only colored. 

### Colors and emotions

1. Red ( Anger ) - the emotion letting the character act aggressively.  

2. White ( Compassion ) - the ability to keep an eye on squadmates during combat. Using healing on, guarding someone else.

3. Blue ( Focus ) - the ability to perform complex tasks and trick maneuvers. Setting and disarming traps, fencing, trick shots.

4. Black ( Resolve ) - the emotion making the character do whatever needs to be done, whatever the cost. May be needed for both following the rules of a strict code and fighting dirty, finishing downed enemies.

5. Yellow ( Vanity ) - the need to act in a flashy manner, drawing everybody's attention. Needed for giving orders, singing hymns, using exotic combat styles.

6. Green ( Caution ) - ability to take care of oneself, act defensively.

*risks here*:

- The Red emotion seems out of place, having a lot less possible applications than other ones.

*variants*: 

- Use seven "Heavenly Virtue - Deadly Sin" pairs as foundation for these.

- An abundance of any given color at one time is actually a weakness: a lot of red provokes berserker rage, a lot of green makes character act cowardly.

### Building connections between squadmates

Between the battles, characters can interact to build relationships. If, for example, two of them are friends, than hurting one will give a second a number of *Anger* marbles to use in his next turn.

### In-combat dialogue options

Another possible related mechanic I was thinking about: the in-combat character dialogue. Defying [Talking is a Free Action trope](http://tvtropes.org/pmwiki/pmwiki.php/Main/TalkingIsAFreeAction), characters interact during combat using their marbles to choose dialogue options. For example, if the squad members are the officers of the law, one of them can shout a short "Stop, in the name of the king!" by playing a *Focus* marble, making some enemies really give up. If none of them have a *Focus marble*, the fight will ensue. 