---
#Title and Zone:
title: Quick Rules
zone: Kalamala

#Path and Metadata
folder: /kalamala
permalink: /rules/quick/
layout: subpage
description: The quick rules page for Kalamala on prawnsgame.org.uk, where you can learn how to play the abstract strategy board game Kalamala. These rules are great for reference and lookup.
published: true

#Links
link1name: Home
link1path: /
link2name: Rules
link2path: /rules/
link3name: Play
link3path: /play/

#SubLinks
sublinktopname: Rules
sublinktoppath: /rules/
sublink1name: Teaching Rules
sublink1path: /rules/teaching/
sublink2name: Quick Rules
sublink2path: /rules/quick/
sublink3name: Short Rules
sublink3path: /rules/short/
sublink4name: Complete Manual
sublink4path: /rules/manual/
---

These are the Quick rules for Kalamala which act primarily as a reference guide.

Please note that the terms used in this ruleset are by no means fixed.

Equipment
=========

 - 1 8x8 square gameboard
 - 16 stones (8 of each colour, with each colour representing a player)

Setup
=====

![starting position for kalamala]({{ site.baseurl }}/images{{ page.folder }}/start.png)

Each player starts with 4 stones on the board (as shown above), and keeps 4 more stones off the board.

These are called unplaced stones.

Objective
=========

To take the last turn of the game (i.e. to put your opponent in a position where it is their turn, but they are unable to do anything).

Turns
=====

Players must decide before the game who takes the first turn.

 - Play alternates, with each player making one movement or one placement in each turn.

Placement
=========

 - In a placement, the player takes one of his unplaced pieces and puts it in any empty square on the board.

Movement
========

A group is a series of one or more same-coloured stones adjacent to one another in a (diagonal, horizontal, or vertical) line.

A stone may belong to many groups, and a group is legal even if it is also part of a larger group.

The line that defines the group is the one on which all the stones in that group lie (for a group of  one, this can be any diagonal, horizontal, or vertical line that passes through it).

 - In a movement, the player selects a group of their stones called the A-group. This group does not move.
 - The player then picks a second group of either player’s stones called the P-group following two rules:
    + It must share its defining line with the A-group
    + There must be no occupied spaces directly between the two groups.
 - The player may then push the P-group (move it away from the A-group), or pull the P-group (move it towards the A-group) following four rules:
    + The movement must be along the shared line that defines the groups.
    + The number of spaces each stone in the P-group is moved by is calculated by the formula: 
      ([number of spaces] = [number of stones in the A-group] ÷ [number of stones in the P-group]), which is rounded down if it is not whole.
    + Stones in the P-group must not pass through, or land on an occupied space, but can land off of the board.
    + Any stones in the P-group that are pushed off the board are removed from play.

Progression Enforcement
=======================

The state of the game includes the position and number of stones on the board, and the number of unplaced stones each player has.

A turn is illegal if:

 - It makes no change to the state of the game.
 - It causes the state of the game to be identical to any one earlier in the game.

End of the Game
===============

The game ends when one player is in a position where it is their turn, but they are unable to do anything.

The other player is then declared the winner.

There are no draws.
