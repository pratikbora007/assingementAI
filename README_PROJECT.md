# Artificial Intelligence Algorithms Collection

This repository contains implementations of core Artificial Intelligence concepts using Python. The project demonstrates algorithm design, decision-making techniques, probability-based reasoning, and interactive gameplay through practical examples.

The repository includes algorithm visualization, probabilistic state prediction, and AI-driven game logic.

---

## Project Summary

This project is organized into three independent modules that explore important AI techniques and applications.

### 1. Alpha-Beta Search Optimization (`alpha_beta_algorithm.py`)

This module demonstrates the Alpha-Beta Pruning technique used to optimize decision-making in game trees.

The implementation reduces unnecessary evaluations while preserving optimal results from the minimax process.

#### Main Features

* Constructs and evaluates game trees
* Performs Alpha-Beta optimization
* Generates visual representations using Graphviz
* Displays pruning decisions and evaluation flow
* Tracks Alpha and Beta values dynamically

---

### 2. Hidden Markov Model — Viterbi Implementation (`viterbi_algorithm.py`)

This module applies the Viterbi algorithm to determine the most probable hidden state sequence in a Hidden Markov Model.

It demonstrates probabilistic inference and sequence prediction.

#### Main Features

* Computes optimal hidden-state transitions
* Performs sequence decoding
* Displays probability distributions visually
* Supports customizable transition and emission parameters
* Generates probability plots using Matplotlib

---

### 3. AI-Based Tic-Tac-Toe (`tic_tac_toe_game.py`)

A command-line Tic-Tac-Toe application where users compete against an AI opponent.

The AI uses Minimax enhanced with Alpha-Beta optimization to make strategic decisions.

#### Main Features

* Interactive player vs AI gameplay
* Smart move selection using Minimax
* Alpha-Beta optimization for faster decisions
* Automatic game-state evaluation
* Win and draw detection

---

# Requirements

Install **Python 3.6 or later** before running the project.

## Required Libraries

Dependencies are provided in:

```bash
requirements.txt
```

Included packages:

* contourpy
* cycler
* graphviz
* kiwisolver
* matplotlib
* numpy
* packaging
* Pillow
* pyparsing

---

# Installation Guide

## Step 1 — Install Python Dependencies

Open a terminal inside the project folder and run:

```bash
pip install -r requirements.txt
```

---

## Step 2 — Install Graphviz (Windows Users)

Graph visualization requires Graphviz to be installed separately.

### Installation

1. Visit Graphviz official website
2. Download the Windows installer
3. Run installation
4. Enable **Add Graphviz to PATH**
5. Finish installation

If Graphviz is not added automatically:

Default location:

```text
C:\Program Files\Graphviz\bin
```

Add this folder to your system environment variables.

### Confirm Installation

Run:

```bash
dot -V
```

If installed correctly, a version number will appear.

### Optional Path Configuration

If Graphviz is installed elsewhere, update:

```python
# import os
# os.environ["PATH"] += os.pathsep + r"C:\Program Files\Graphviz\bin"
```

inside:

```text
alpha_beta_algorithm.py
```

---

## Step 3 — Test Setup

Execute:

```bash
python alpha_beta_algorithm.py
```

Successful execution should generate a visualization output.

---

# Running the Modules

## Alpha-Beta Visualization

Execute:

```bash
python alpha_beta_algorithm.py
```

Expected Output:

* Generated decision tree
* Pruned branch highlights
* Graph export
* Evaluation statistics

---

## Hidden Markov Model (Viterbi)

Execute:

```bash
python viterbi_algorithm.py
```

Expected Output:

* Hidden state predictions
* Probability matrix
* Visualization graphs
* Transition tracking

---

## Tic-Tac-Toe AI

Execute:

```bash
python tic_tac_toe_game.py
```

Gameplay Rules:

Board layout:

```text
0 | 1 | 2
---------
3 | 4 | 5
---------
6 | 7 | 8
```

Instructions:

* Enter values from 0–8
* Player uses **O**
* AI uses **X**
* Game ends after a win or draw

---

# Troubleshooting

### Graphviz Import Errors

Install:

```bash
pip install graphviz
```

---

### Graph Rendering Issues

Verify:

* Graphviz installation
* PATH configuration
* Restart terminal after installation

---

### Missing Python Packages

Reinstall dependencies:

```bash
pip install -r requirements.txt
```

---

# Repository Layout

```text
AI Assignment/
├── README_PROJECT.md
├── requirements.txt
├── alpha_beta_algorithm.py
├── viterbi_algorithm.py
├── tic_tac_toe_game.py
├── .gitignore
```

---

# Algorithm Information

### Alpha-Beta Optimization

* Best Case: O(b^(d/2))
* Worst Case: O(b^d)
* Used in strategic decision systems

### Viterbi Algorithm

* Complexity: O(N² × T)
* Common in sequence prediction and inference

### Minimax Strategy

* Recursive search model
* Enhanced using Alpha-Beta optimization
* Produces optimal gameplay decisions

---

# Additional Notes

For complete visualization support, Graphviz installation is recommended—especially on Windows systems.

