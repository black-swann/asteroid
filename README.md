# Asteroids

A classic Asteroids arcade game clone built with Python and Pygame.

## Features

- Player ship with rotation and thrust controls
- Shooting mechanics with cooldown
- Asteroids that spawn from screen edges
- Asteroids split into smaller pieces when shot
- Collision detection between player, shots, and asteroids

## Requirements

- Python 3.10+
- Pygame 2.6+

## Installation

```bash
# Clone the repository
git clone https://github.com/black-swann/asteroid.git
cd asteroid

# Create virtual environment and install dependencies
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install pygame
```

Or using [uv](https://github.com/astral-sh/uv):

```bash
uv sync
```

## Running the Game

```bash
python main.py
```

Or with uv:

```bash
uv run main.py
```

## Controls

| Key | Action |
|-----|--------|
| W | Move forward |
| S | Move backward |
| A | Rotate left |
| D | Rotate right |
| Space | Shoot |

## How to Play

- Avoid colliding with asteroids
- Shoot asteroids to destroy them
- Large asteroids split into two smaller, faster asteroids
- The smallest asteroids are destroyed completely when shot
- The game ends when your ship collides with an asteroid

## Project Structure

```
asteroid/
├── main.py           # Game entry point and main loop
├── player.py         # Player ship class
├── asteroid.py       # Asteroid class
├── asteroidfield.py  # Asteroid spawning logic
├── shot.py           # Bullet/shot class
├── circleshape.py    # Base class for circular game objects
├── constants.py      # Game configuration constants
└── logger.py         # State logging utilities
```

## License

MIT
