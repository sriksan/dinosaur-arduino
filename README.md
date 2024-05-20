# Dinosaur Arduino

This project implements a simple side-scrolling game inspired by the Chrome dinosaur game, using an Arduino and an I2C-connected Liquid Crystal Display (LCD). The player controls a dinosaur character that must jump over various obstacles to avoid collisions and keep the game going.

## Overview
- **Custom Characters**: Unique characters for the dinosaur, small cactus, big cactus, and bird obstacles, created using the LCD's custom character functionality.
- **Random Obstacle Generation**: Obstacles are generated at random positions and intervals, making each game session unique.
- **Score Display**: The player's current score is continuously displayed on the LCD screen.
- **Increasing Difficulty**: As the player’s score increases, the game speed increases, making the game progressively more challenging.
- **Game Over Screen**: When the dinosaur collides with an obstacle, the game ends and a "GAME OVER" message is displayed along with the final score.

## Game Mechanics
- **Jumping**: The player controls the dinosaur using a push button connected to the Arduino. Pressing the button makes the dinosaur jump to avoid obstacles.
- **Obstacle Movement**: Obstacles move from right to left across the screen. If an obstacle reaches the left side of the screen, it resets and reappears on the right.
- **Collision Detection**: The game checks for collisions between the dinosaur and obstacles. If a collision is detected, the game ends.
- **Score Keeping**: The player's score increases over time as long as the dinosaur avoids obstacles. The score is displayed on the LCD and updated in real-time.
- **Speed Increase**: The game speed increases at regular intervals based on the player's score, adding to the game's difficulty.

## Custom Characters
The game uses custom binary arrays to define the shapes of the dinosaur, small cactus, big cactus, and bird. These custom characters are stored in the LCD’s memory and displayed as needed during gameplay.

