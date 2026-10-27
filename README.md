# Asteroids

A classic Asteroids-style arcade game built with Python and Pygame. Fly your ship, shoot asteroids, and avoid getting hit.

## Features

- Rotate and move a triangular ship
- Shoot bullets with a cooldown (one shot every 0.3 seconds)
- Asteroids spawn from the screen edges and drift across the playfield
- Large asteroids split into two smaller, faster ones when shot
- Circle-based collision detection
- Game over when the ship hits an asteroid

## Controls

| Key | Action |
| --- | --- |
| `A` | Rotate left |
| `D` | Rotate right |
| `W` | Move forward |
| `S` | Move backward |
| `Space` | Shoot |

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/DCaputi001/boot-asteroids.git
   cd boot-asteroids
   ```

2. Create and activate a virtual environment (optional but recommended):

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Install Pygame:

   ```bash
   pip install pygame
   ```

4. Run the game:

   ```bash
   python main.py
   ```

## Project Structure

| File | Purpose |
| --- | --- |
| `main.py` | Game loop, sprite groups, and collision checks |
| `circleshape.py` | Base class for all circular game objects |
| `player.py` | The player's ship: movement, rotation, shooting |
| `asteroid.py` | Asteroid behavior, including splitting |
| `asteroidfield.py` | Spawns new asteroids at random screen edges |
| `shot.py` | Bullets fired by the player |
| `constants.py` | Game settings (sizes, speeds, cooldowns) |
| `logger.py` | Logs game state and events |

## Extending the Project

You've done all the required steps, but if you'd like to make the game your own, here are some ideas:

* Add a scoring system
* Implement multiple lives and respawning
* Add an explosion effect for the asteroids
* Add acceleration to the player movement
* Make the objects wrap around the screen instead of disappearing
* Add a background image
* Create different weapon types
* Make the asteroids lumpy instead of perfectly round
* Make the ship have a triangular hitbox instead of a circular one
* Add a shield power-up
* Add a speed power-up
* Add bombs that can be dropped
