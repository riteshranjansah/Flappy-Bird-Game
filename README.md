# Flappy Bird Game

This is a simple **Flappy Bird** clone created using **Pygame**, a Python library for making video games. The game follows the classic Flappy Bird mechanics, where the player must navigate a bird through pipes by pressing the space bar to make the bird "flap." The game is over when the bird hits the ground or collides with a pipe.

## Features

- **Flappy Bird Mechanics**: The bird flaps when the space bar is pressed and falls due to gravity.
- **Pipes**: Randomly generated pipes that the bird must navigate between. The pipes continuously move towards the bird.
- **Score**: The player scores points each time they successfully pass between the pipes.
- **Game Over Screen**: Displays when the bird crashes or falls to the ground.
- **High Score Tracking**: Keeps track of the highest score achieved during gameplay.

## Technologies Used

- **Python**: The main programming language used for implementing the game logic.
- **Pygame**: A library used for developing the game, handling graphics, sounds, and user input.
- **Random**: Used for generating random pipe heights to vary the difficulty.

## Installation

### Prerequisites

- **Python**: Make sure you have Python 3.x installed. You can download it from [python.org](https://www.python.org/downloads/).
- **Pygame**: Install the Pygame library using pip:

```bash
pip install pygame
```

### Download the Game

1. Clone the repository:

```bash
git clone https://github.com/riteshranjansah/Flappy-Bird-Game.git
```

2. Navigate into the project directory:

```bash
cd Flappy-Bird-Game
```

3. Run the game:

```bash
python flappy.py
```

### Game Assets

The game uses the following assets located in the `assets/` and `sound/` folders:
- **Background Image**: The background of the game.
- **Bird Images**: The bird's different flapping animations.
- **Pipe Images**: The pipe graphics that the bird must avoid.
- **Floor Image**: The moving base of the game environment.
- **Sound Effects**: Sounds for bird flapping, collisions, and scoring.

Make sure that the assets are placed in their respective folders (`assets/` and `sound/`). You can modify the file paths in the script if needed.

## How to Play

- **Controls**: Use the **Space Bar** to make the bird flap and navigate through the pipes.
- **Objective**: The goal is to keep the bird flying and avoid the pipes. The longer you survive, the higher your score.
- **Game Over**: The game ends when the bird:
  - Collides with a pipe.
  - Falls to the ground (bottom of the screen).
- **Score**: The score increases every time the bird successfully passes between pipes. The score is displayed at the top of the screen during gameplay and at the end of the game.

## Game Logic

### Bird Mechanics

- **Flap**: Pressing the space bar makes the bird flap, which moves the bird upwards.
- **Gravity**: Gravity pulls the bird down, simulating natural falling.
- **Rotation**: The bird rotates slightly as it falls, giving it a more realistic appearance.

### Pipe Mechanics

- **Pipe Creation**: Pipes are created at regular intervals and have random heights. 
- **Movement**: Pipes move from right to left across the screen, and when they move off the screen, they are removed and replaced with new pipes.
- **Collision**: The game checks for collisions between the bird and pipes or the floor to determine if the game is over.

### Scoring

- **Score**: The score increments each time the bird successfully passes between pipes.
- **High Score**: The high score is tracked across sessions and is displayed at the end of the game.

## Directory Structure

```
Flappy-Bird-Game/
│
├── assets/
│   ├── background-day.png    # The background image
│   ├── base.png              # The floor image
│   ├── bluebird-downflap.png # Bird image (downflap)
│   ├── bluebird-midflap.png  # Bird image (midflap)
│   ├── bluebird-upflap.png   # Bird image (upflap)
│   ├── pipe-green.png        # Pipe image
│   └── message.png           # Game over image
│
├── sound/
│   ├── sfx_wing.wav          # Flap sound
│   ├── sfx_hit.wav           # Collision sound
│   └── sfx_point.wav         # Score sound
│
├── flappy.py                 # Main game script
└── README.md                 # This file
```

## Contributing

If you'd like to contribute to this project, you can:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request on GitHub.

## License

This project is open-source and available for personal use and modification. No formal license has been applied, so feel free to use or modify the code as per your needs.
