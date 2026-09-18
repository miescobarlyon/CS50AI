# CS50's Introduction to Artificial Intelligence with Python

My solutions to the projects from [CS50's Introduction to Artificial Intelligence with Python](https://cs50.harvard.edu/ai/), offered by Harvard University.

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white)
![CS50 AI](https://img.shields.io/badge/CS50-AI-crimson)
![License](https://img.shields.io/badge/License-MIT-green)

## About

This course explores the concepts and algorithms at the foundation of modern artificial intelligence, covering topics from classical search algorithms to neural networks and natural language processing. Each week pairs a lecture with one or two hands-on projects where I implemented the AI logic in Python.

## Projects

### Week 0 — Search

| Project | Description | Concepts |
|---------|-------------|----------|
| [Degrees](Project0/degrees/) | Finds the shortest connection between any two actors via shared movies | BFS, graph search |
| [Tic-Tac-Toe](Project0/tictactoe/) | An AI opponent that plays optimally and never loses | Minimax, adversarial search |

### Week 1 — Knowledge

| Project | Description | Concepts |
|---------|-------------|----------|
| [Knights](knights/) | Solves Knights & Knaves logic puzzles | Propositional logic, model checking |
| [Minesweeper](minesweeper/) | An AI that can play Minesweeper using logical inference | Knowledge representation, inference |

### Week 2 — Uncertainty

| Project | Description | Concepts |
|---------|-------------|----------|
| [PageRank](pagerank/) | Ranks web pages using both sampling and iteration methods | Markov chains, probability |
| [Heredity](heredity/) | Predicts the likelihood of a genetic trait using family data | Bayesian networks, joint probability |

### Week 3 — Optimization

| Project | Description | Concepts |
|---------|-------------|----------|
| [Crossword](crossword/) | Generates crossword puzzles from a given structure and word list | Constraint satisfaction, backtracking |

### Week 4 — Learning

| Project | Description | Concepts |
|---------|-------------|----------|
| [Shopping](shopping/) | Predicts whether a user will complete an online purchase | k-NN, supervised learning |
| [Nim](nim/) | An AI that teaches itself to play Nim through repeated games | Q-learning, reinforcement learning |

### Week 5 — Neural Networks

| Project | Description | Concepts |
|---------|-------------|----------|
| [Traffic](traffic/) | Classifies road signs from images using a convolutional neural network | CNNs, TensorFlow, computer vision |

### Week 6 — Language

| Project | Description | Concepts |
|---------|-------------|----------|
| [Parser](parser/) | Parses English sentences and extracts noun phrase chunks | Context-free grammars, NLP |
| [Questions](questions/) | Answers questions by retrieving the most relevant passage from a corpus | TF-IDF, information retrieval |

## Tech Stack

- **Language:** Python 3
- **Libraries:** TensorFlow / Keras, scikit-learn, nltk, Pygame
- **Concepts:** Search, knowledge representation, probability, optimization, machine learning, neural networks, NLP

## Getting Started

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO
```

Each project folder has its own dependencies. Generally:

```bash
pip install -r requirements.txt
```

## Acknowledgments

All project specs, starter code, and course materials are by [Brian Yu](https://brianyu.me) and [David J. Malan](https://cs.harvard.edu/malan/) at Harvard University. I implemented the AI logic for each project.

Course link: [cs50.harvard.edu/ai](https://cs50.harvard.edu/ai/)