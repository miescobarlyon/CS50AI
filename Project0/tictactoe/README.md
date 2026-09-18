# Tic-Tac-Toe

An AI that plays Tic-Tac-Toe optimally using the **Minimax** algorithm — it will never lose.

Built as part of [CS50's Introduction to Artificial Intelligence with Python](https://cs50.harvard.edu/ai/) — Week 0: Search.

## Demo

```
$ python runner.py
```

Choose to play as X or O, then try to beat the AI — spoiler: you can't.

## How It Works

The AI treats the game as a tree of all possible future board states and uses **Minimax** to evaluate each one recursively:

- **X (maximizing player)** picks the move that leads to the highest score.
- **O (minimizing player)** picks the move that leads to the lowest score.
- Terminal states are scored: **+1** (X wins), **-1** (O wins), **0** (draw).

By exploring every possible game to completion, the AI always chooses the optimal move — guaranteeing it never loses.

## Project Structure

```
.
├── runner.py        # Pygame interface (provided by CS50)
├── tictactoe.py     # Game logic and AI implementation
├── requirements.txt
└── README.md
```

## What I Implemented

CS50 provided the Pygame runner and UI. I implemented the full game logic in `tictactoe.py`:

| Function    | Description                                             |
|-------------|---------------------------------------------------------|
| `player`    | Determines whose turn it is based on the board state    |
| `actions`   | Returns all available moves on the board                |
| `result`    | Returns a new board state after a given move            |
| `winner`    | Checks rows, columns, and diagonals for a winner       |
| `terminal`  | Checks if the game is over (win or draw)                |
| `utility`   | Scores a terminal board (+1, -1, or 0)                  |
| `minimax`   | Returns the optimal move using recursive Minimax search |

## Getting Started

### Prerequisites

- Python 3.12+
- Pygame

### Installation

```bash
pip install -r requirements.txt
```

### Run

```bash
python runner.py
```

## Concepts

- Adversarial search
- Minimax algorithm
- Game trees
- Recursive decision-making
- Terminal state evaluation

## Acknowledgments

Project spec and starter code by [Brian Yu](https://brianyu.me) and [David J. Malan](https://cs.harvard.edu/malan/) at Harvard University.