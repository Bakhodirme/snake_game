# Snake Game

A classic Snake game built with Python and the built-in `turtle` module.

## About

This project is a small desktop game where the player controls a snake inside a 600x600 window. The snake grows each time it eats food, the score updates in real time, and the game ends when the snake hits a wall or its own body.

## Features

- Smooth continuous snake movement
- Keyboard controls with arrow keys
- Random food spawning
- Score tracking at the top of the screen
- Collision detection for walls and tail
- Simple object-oriented project structure

## Gameplay

The snake starts with three segments and moves continuously across the screen. Each time it touches the food, the food respawns at a random position, the snake grows by one segment, and the score increases by one.

## Controls

| Key | Action |
| --- | --- |
| `Up Arrow` | Move up |
| `Down Arrow` | Move down |
| `Left Arrow` | Move left |
| `Right Arrow` | Move right |

## Requirements

- Python 3
- Standard library `turtle` module

No external packages are required.

## Run the Project

From the project folder:

```bash
py -3 main.py
```

If the `py` launcher is not available:

```bash
python main.py
```

## Project Structure

```text
.
|-- food.py
|-- main.py
|-- scoreboard.py
|-- snake.py
|-- README.md
`-- assets/
```

## File Overview

- `main.py` sets up the screen, starts the game loop, handles input, and checks collisions.
- `snake.py` defines the `Snake` class, movement behavior, and growth logic.
- `food.py` defines the `Food` class and handles random food repositioning.
- `scoreboard.py` defines the `Scoreboard` class for score display and game-over text.

## Game Rules

1. The snake starts with three body segments.
2. Eating food increases the score by one.
3. Eating food also adds one segment to the snake.
4. The game ends if the snake touches the window border.
5. The game ends if the snake touches its own tail.

## Media

The repository is prepared for screenshots or a demo GIF in the `assets/` folder.

Suggested file names:

- `assets/snake-demo.gif`
- `assets/snake-screenshot.png`

Once those files are added, you can embed them in this README.

## Possible Improvements

- Add a restart option after game over
- Keep a high score between runs
- Prevent food from spawning on the snake body
- Add difficulty levels by increasing speed

## Notes

This project is a good beginner example of:

- Python classes and objects
- Game loops
- Event handling
- Collision detection
- Basic GUI programming with `turtle`
