# Snake Game

Welcome to the Snake Game, a classic arcade-style game implemented in Python using the Turtle graphics library. In this game, you control a snake, guiding it to consume food and grow longer while avoiding collisions with the game boundaries and itself.

## Classes

### Scoreboard Class
The `Scoreboard` class manages the display of the player's score, updates it as the snake consumes food, and handles the end of the game.

```python
from turtle import Turtle

ALIGNMENT = "center"
FONT = ("Courier", 24, "normal")

class Scoreboard(Turtle):
    # ... (see Scoreboard class section)
```


### Food Class

The `Food` class represents the food items that the snake consumes. It initializes a blue circular shape and places itself randomly on the screen.
```python
from turtle import Turtle
import random

class Food(Turtle):
    # ... (see Food class section)
```

### Snake Class

The `Snake` class defines the behavior of the snake. It includes methods for moving, changing direction, extending length, and creating initial segments.
```python
from turtle import Turtle

STARTING_POSITIONS = [(0, 0), (-20, 0), (-40, 0)]
MOVE_DISTANCE = 20
UP = 90
DOWN = 270
RIGHT = 0
LEFT = 180

class Snake:
    # ... (see Snake class section)
```

### main.py
The `main.py` file orchestrates the game by setting up the window, creating instances of the Snake, Food, and Scoreboard classes, and running the game loop.

```python
from turtle import Screen
import time
from snake import Snake
from food import Food
from scoreboard import Scoreboard
```

### ... (see main.py section)

## Getting Started
1. Ensure you have Python installed on your machine.
2. Clone the repository to your local machine.

`git clone https://github.com/your-username/snake-game.git`

`cd snake-game`

## Running
Run the game using the following command:

`python main.py`

## Play
Use the arrow keys to navigate the snake, and try to eat as much food as possible without colliding with the boundaries or yourself.

## Gameplay
1. The snake starts with three segments and grows longer each time it consumes food.
2. The score is displayed at the top of the screen, updating as the snake eats.
3. The game ends if the snake collides with the boundaries or itself.

#### Enjoy playing the Snake Game!


