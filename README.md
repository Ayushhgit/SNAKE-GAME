# Snake Game

A classic Snake game implemented in Java using the Swing framework. The game involves controlling a snake to eat food and grow longer while avoiding collisions with the walls and itself.

## Features

- Snake movement controlled by arrow keys
- Food placement at random positions
- Score tracking based on the length of the snake
- Game over detection when the snake collides with itself or the walls
- Ability to restart the game by pressing the spacebar

## Requirements

- Java Development Kit (JDK) 8 or higher

Controls
Arrow Keys: Control the direction of the snake
Spacebar: Restart the game after a game over
Code Overview
Classes
Tile
Represents a single tile on the game board with x and y coordinates.

SnakeGame
Extends JPanel and implements ActionListener and KeyListener to handle game logic and user input.

Constructor:
Initializes the game board, snake, food, and starts the game loop timer.

paintComponent(Graphics g):
Calls draw(Graphics g) to render the game components.

draw(Graphics g):
Draws the grid, snake, food, and score.

placeFood():
Randomly places food on the game board.

move():
Handles the movement of the snake, including eating food and game over conditions.

collision(Tile tile1, Tile tile2):
Checks if two tiles occupy the same position.

actionPerformed(ActionEvent e):
Called by the game loop timer to update the game state and repaint the board.

keyPressed(KeyEvent e):
Handles user input for controlling the snake and restarting the game.

restart():
Resets the game state for a new game.
