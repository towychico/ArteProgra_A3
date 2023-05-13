# ArteProgra_A3
- `import random` and `from random import choice`: Import the `random` library and specifically the `choice` function, which will be used later to randomly select a direction for the ghosts to move.

- `from turtle import *`: Import everything from the `turtle` library, which will be used to create the game graphics.

- `from freegames import floor, vector`: Import two functions from the custom `freegames` library. `floor` is used to round down floating-point numbers to integers, while `vector` creates a 2D vector with x and y components.

- `state = {'score': 0}`: Define an initial state for the game, which contains a single key-value pair for the score.

- `path = Turtle(visible=False)`: Create a new `Turtle` object called `path`, which will be used to draw the grid of tiles.

- `writer = Turtle(visible=False)`: Create a new `Turtle` object called `writer`, which will be used to display the player's score.

- `aim = vector(5, 0)`: Define an initial direction for Pac-Man to move in. This vector represents a movement of 5 units to the right and 0 units up or down.

- `pacman = vector(-40, -80)`: Define an initial position for Pac-Man on the grid. This vector represents a position of 40 units to the left and 80 units down from the top-left corner of the grid.

- `ghosts = [...]`: Define the initial positions and directions of the four ghosts on the grid.

- `tiles_list = [...]`: Define a 2D list that represents the grid of tiles. Each tile is either a 0 (for an empty tile) or a 1 (for a tile with a pellet that Pac-Man can eat).


- `square(x, y)`: Draws a single square on the grid at the specified x and y coordinates.

- `food(x, y)`: Draws a small white dot (representing a pellet) on the grid at the specified x and y coordinates.

- `move():` Moves Pac-Man and the ghosts according to their current directions, and handles collisions between Pac-Man and the pellets or the ghosts.

- `change(x, y)`: Changes Pac-Man's direction based on the arrow keys pressed by the player.

- `inside(point)`: Returns `True` if the specified point (represented as a vector) is inside the grid.

- `down():`, `left():`, `right():`, `up():`: These functions change Pac-Man's direction to move in the corresponding direction.

- `next_tile(point, direction)`: Returns the position of the next tile in the specified direction from the given point.

- `opposite(direction)`: Returns the opposite direction from the given direction (e.g. if the given direction is "right", this function returns "left").

- `distance(p, q)`: Computes the Euclidean distance between two points (represented as vectors).

- `main():` The main function that sets up the game window, draws the grid of tiles and pellets, and starts the game loop.
