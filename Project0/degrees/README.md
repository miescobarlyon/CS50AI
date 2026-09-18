# Degrees

An AI that finds the shortest chain of movies connecting any two actors — inspired by the [Six Degrees of Kevin Bacon](https://en.wikipedia.org/wiki/Six_Degrees_of_Kevin_Bacon) game.

Built as part of [CS50's Introduction to Artificial Intelligence with Python](https://cs50.harvard.edu/ai/) — Week 0: Search.

## Demo

```
$ python degrees.py large
Loading data...
Data loaded.
Name: Emma Watson
Name: Jennifer Lawrence
3 degrees of separation.
1: Emma Watson and Brendan Gleeson starred in Harry Potter and the Order of the Phoenix
2: Brendan Gleeson and Michael Fassbender starred in Trespass Against Us
3: Michael Fassbender and Jennifer Lawrence starred in X-Men: First Class
```

## How It Works

The program models actors as **nodes** and shared movies as **edges** in a graph, then uses **Breadth-First Search (BFS)** to find the shortest path between any two actors.

BFS guarantees the shortest path because it explores all connections at distance 1 before distance 2, and so on — making it ideal for this "fewest degrees of separation" problem.

## Project Structure

```
.
├── degrees.py       # Main program — loads data and runs search
├── util.py          # Node, StackFrontier, and QueueFrontier classes
├── small/           # Small dataset for testing
│   ├── movies.csv
│   ├── people.csv
│   └── stars.csv
└── large/           # Full IMDb-sourced dataset
    ├── movies.csv
    ├── people.csv
    └── stars.csv
```

## What I Implemented

CS50 provided the data loading, user input handling, and utility classes. I implemented the `shortest_path` function in `degrees.py`, which:

- Takes a source actor and a target actor
- Uses BFS to explore the graph of actors connected by shared movies
- Returns the shortest sequence of (movie, actor) pairs connecting them, or `None` if no connection exists

## Getting Started

### Prerequisites

- Python 3.12+

### Run

```bash
# Using the small dataset (faster, for testing)
python degrees.py small

# Using the full dataset
python degrees.py large
```

## Concepts

- Graph search
- Breadth-First Search (BFS)
- Frontier-based exploration
- State-space modeling

## Acknowledgments

Project spec and starter code by [Brian Yu](https://brianyu.me) and [David J. Malan](https://cs.harvard.edu/malan/) at Harvard University. Movie data courtesy of [IMDb](https://www.imdb.com/). Used with permission.