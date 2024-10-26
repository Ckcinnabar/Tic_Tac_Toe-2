# Object-Oriented Tic-tac-toe Game

A Python implementation of Tic-tac-toe using object-oriented programming principles. This version improves on the original by using classes to organize the code and manage game state.

## Description

This program implements a two-player Tic-tac-toe game using an object-oriented approach. The game is split into three main classes: `Board`, `Game`, and a main controller. Players take turns placing their marks (X or O) on a 3x3 grid, with full input validation and win/draw detection.

## Class Structure

### Board Class
- Manages the game board state and display
- Methods:
  - `__init__()`: Initializes the game board
  - `printBoard()`: Displays the current board state
  - `updateBoard()`: Updates a cell with a player's symbol
  - `getCell()`: Returns the content of a specific cell

### Game Class
- Handles game logic and player interactions
- Methods:
  - `__init__()`: Initializes game state
  - `switchPlayer()`: Alternates between players
  - `validateEntry()`: Validates player moves
  - `checkFull()`: Checks for a draw condition
  - `checkWin()`: Detects winning conditions
  - `checkEnd()`: Determines if the game is over
  - `playGame()`: Main game loop

## Features

- Object-oriented design with clear separation of concerns
- Interactive command-line interface
- 3x3 game board with coordinate system
- Input validation for:
  - Valid coordinate ranges (0-2)
  - Already occupied cells
  - Proper input format (row,column)
- Win detection for:
  - Horizontal rows
  - Vertical columns
  - Diagonals
- Draw detection
- Exception handling for invalid inputs
- Option to play multiple games

## How to Play

1. Run the program
2. The game starts with player X's turn
3. Enter coordinates as "row,column" (e.g., "1,1" for center)
4. Valid input ranges from 0 to 2 for both row and column
5. Players alternate turns until someone wins or the game is a draw
6. Choose to play again or exit after each game

## Input Format
```
row,column
```
- Both values should be between 0 and 2
- Values should be separated by a comma
- Example: "1,1" for the center position

## Board Layout
```
R\C |  0  |  1  |  2  | 
-----------------------
 0  |     |     |     | 
-----------------------
 1  |     |     |     | 
-----------------------
 2  |     |     |     | 
-----------------------
```

## Error Handling
The game includes robust error handling for:
- Non-numeric inputs
- Out-of-range values
- Invalid input formats
- Attempts to play in occupied cells

## Technical Improvements Over Previous Version
- Encapsulated board state and operations
- Separated game logic from display logic
- More maintainable and extensible code structure
- Improved error handling with try-except blocks
- Cleaner input processing

## Author
Kuan Chen Chen

## Date
October 25, 2024

## Version
2.0
