---
layout: post
title: Battleships game
subtitle: Adaptation of the Battleships game as an Android app
tags: [Java, Android]
cover-img: /assets/img/custom_grid.jpg
thumbnail-img: /assets/img/custom_grid.png
share-img: /assets/img/custom_grid.jpg
comments: true
---

This is a university project in which the classic board game "Battleships" is adapted into a basic android mobile application using Java.

## Home screen

![image](/assets/img/home-screen.PNG){: .mx-auto.d-block :}

This is the screen the user sees when they launch the game.

## Ship placement screen

![image](/assets/img/place-fleet.PNG){: .mx-auto.d-block :}

The user can select a specific ship to place onto the grid (selection on the left side of the screen) and whether it will be placed horizontally or vertically (selected orientation is highlighted on the right side of the screen)  
* If the user does not place all the ships onto the grid, the game does not start.
* If a ship is placed out of the grid bounds, its placement is removed and it has to be placed again.


## Gameplay/Fight screen

![image](/assets/img/fight-screen.PNG){: .mx-auto.d-block :}

The game alternates turns between the user and their enemy. The enemy guesses can be displayed at the top left on the screen.  
The tiles in the grid turn to different colours based on the guess:
* Grey: Miss
* Red: Hit
* Blue: Ship destroyed

The game ends when either the friendly or enemy ships are destroyed and the user is transferred to the Home Screen.
