# AI Solutions for the Lights Out Puzzle

## Overview
This project implements multiple AI-based search algorithms to solve the *Lights Out Puzzle*, a grid-based logic game where the goal is to turn off all the lights by toggling individual lights, which in turn affects their neighbors. The project explores algorithms such as Breadth-First Search (BFS), Iterative Deepening Search (IDS), A*, and Weighted A*, comparing their efficiency and effectiveness in solving the puzzle.

## Features
- **Breadth-First Search (BFS)**: Guarantees finding an optimal solution, but can be slow due to high memory usage.
- **Iterative Deepening Search (IDS)**: Combines the benefits of BFS and DFS, with lower memory requirements.
- **A* Algorithm**: Uses heuristics to guide the search and find optimal solutions faster.
- **Weighted A* Algorithm**: A faster version of A* that trades off between optimality and speed by weighting the heuristic function.

## Heuristics Used
1. **Disconnected Clusters**: Counts the number of disconnected clusters of ON lights.
2. **Total ON Lights**: Measures how many lights are still on in the puzzle.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/AI-Lights-Out-Puzzle.git
   ```
2. Navigate to the project directory:
   ```bash
   cd AI-Lights-Out-Puzzle
   ```
3. Open the notebook `notebook.ipynb` in Jupyter Notebook to run the algorithms and observe the results.

## Usage

- Run the notebook and experiment with different algorithms to solve the puzzle.
- Compare the performance of various heuristics and algorithms in terms of execution time and nodes visited.

## Results

Based on the test results, here are the average execution times for each algorithm:

- BFS: 0.529 seconds
- IDS: 1.640 seconds
- A* (Heuristic 1 - Disconnected Clusters): 0.172 seconds
- A* (Heuristic 2 - Total Lights ON): 0.292 seconds
- Weighted A* (Heuristic 1, alpha=2): 0.061 seconds
- Weighted A* (Heuristic 2, alpha=1000): 0.003 seconds


