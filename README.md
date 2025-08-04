# Ghost Chase Game in C++

## Project Overview
This is a console-based grid game implemented in C++ where the player controls a character `X` navigating through a 32x32 board filled with barriers and two ghosts (`G` and `K`). The goal is to avoid the ghosts while collecting points by moving over free spaces. The game features multiple difficulty levels that affect ghost movement behavior.


## Features
- **Large 32x32 game board** with static and randomly placed barriers (`#`).
- Player represented by `X`, controlled using `WASD` keys.
- Two ghosts (`G` and `K`) that chase the player with different AI strategies depending on the difficulty level:
  - Easy: Random and simple pathfinding behavior.
  - Medium: More strategic movement towards the player.
  - Hard: Aggressive chasing using distance calculations.
- Score increases as the player moves through open spaces.
- Lose lives mechanic with 3 lives (`LoseCounter`) before game over.
- Color-coded board display using Windows console color attributes.
- Screen refresh and cursor control for smooth rendering.
- Win condition: Covering all empty spaces.
- Lose condition: Collision with either ghost.

## How to Play
- Compile the program using a C++ compiler that supports Windows-specific headers (`windows.h`).
- Run the executable in a Windows terminal.
- Choose difficulty level: 1 (Easy), 2 (Medium), or 3 (Hard).
- Use `W`, `A`, `S`, `D` keys to move the player character `X` around the board.
- Avoid ghosts `G` and `K`.
- The goal is to cover all open spots on the board (denoted by `.`).
- The game ends when you lose all lives or win by clearing the board.


## Code Structure Highlights
- **Board Initialization:** The board is a 2D char array with walls (`#`), empty spaces (`.`), player, and ghosts.
- **Barriers:** Static barriers and randomly placed obstacles populate the board.
- **Player Movement:** Controlled via keyboard input with bounds and collision checking.
- **Ghost AI:** Different ghost movement functions depending on difficulty.
- **Rendering:** Uses Windows console API for colored output and cursor positioning to redraw the board efficiently.
- **Game Logic:** Checks for win/lose conditions every cycle.

## Requirements
- Windows OS (due to usage of `<windows.h>` and console color functions).
- A C++ compiler (e.g., Visual Studio, MinGW).
- Terminal with ANSI escape code and Windows console API support.

