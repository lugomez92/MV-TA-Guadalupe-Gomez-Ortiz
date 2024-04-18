# The Floor Is Lava!

The Floor Is Lava! is a simple text-based game implemented in Node.js. It simulates the challenge of navigating through a room filled with lava puddles. Below is an explanation of how the game works:

## Collaborators
- Mei Huang

## Initialization

The game starts by importing the `prompt-sync` library to enable interaction with the player through the console. It also initializes various variables such as `board`, `gamePlay`, `playerName`, `playerLives`, `playerPosition`, `collisionPointsArray`, `playerMove`, and `exitPosition`.

## Welcome Message

Upon starting, the game welcomes the player and asks for their name. It then informs them about the game's premise and rules.

## Game Start

Depending on the player's response, the game either starts or exits. If the player chooses to play ("yes"), the game generates random collision points on the board, sets the player's initial position, and informs them that they are in a life or death situation.

## Player Moves

The player is prompted to choose a direction to move ("forward", "back", "left", or "right"). The game checks if the move is valid and updates the player's position accordingly. If the move results in a collision with a lava puddle, the player loses a life.

## Game Over/Continuation

If the player loses all lives, the game ends with a "Game Over" message. If the player reaches the exit position, they win the game. Otherwise, they continue playing until they win or lose.

## Functions

- `generateCollisionPoints(board, numPoints)`: Randomly generates collision points on the board, excluding the player's initial and exit positions.
- `movePlayer(board, playerPos, direction)`: Handles player movement, checks for collisions, updates player position, and manages game state.
- `checkCollision(x, y)`: Checks if the specified position collides with a lava puddle.
- `collisionPointExists(point)`: Checks if a collision point already exists at the specified coordinates.

The game continues until the player either successfully reaches the exit or loses all lives.
