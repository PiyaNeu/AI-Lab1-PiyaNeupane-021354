# 🤖 Heuristic Search

This repository showcases two well-known heuristic search problems implemented in Python:

- The **8-Puzzle Game** solved using **Breadth-First Search (BFS)**, with **Manhattan Distance** used as a measure of cost.
- A **Block Sorting Problem** handled with a **Hill Climbing** strategy using a heuristic based on incorrect block positions.

---

## 📁 Files Included

- `eight_puzzle_bfs.py` — Solves the 8-puzzle using BFS and heuristic guidance.
- `block_arrangement_hill_climb.py` — Applies Hill Climbing to rearrange blocks.
- `README.md` — This guide explaining how everything works.

---

## 🧩 1. 8-Puzzle Using BFS and Manhattan Distance

### 📝 Description
The game consists of a 3x3 board filled with numbers from 1 to 8 and a blank tile (0). The task is to arrange the tiles into the final state:
-1 2 3
-4 5 6
-7 8 0

### 📐 Heuristic Used
- **Manhattan Distance**: Adds up how far each tile is from its correct position in terms of rows and columns.

### 🔍 Program Highlights
- Accepts any valid starting configuration.
- Uses BFS to explore possibilities.
- Shows heuristic values during the search.
- Displays the step-by-step moves to reach the solution.

---

## 🧱 2. Block Sorting Using Hill Climbing

### 📝 Description
You are given a shuffled list of four blocks like `[C, A, D, B]`. The goal is to arrange them as `[A, B, C, D]` by only swapping neighbors.

### 📐 Heuristic Used
- **Misplaced Blocks Count**: Counts how many blocks are out of order compared to the goal.

### 🔍 Program Highlights
- Applies Hill Climbing to improve the state step-by-step.
- Can identify if it gets stuck in a local best (local maxima).
- Prints each move along with the heuristic value.

---

## ⚙️ How to Run

### 📦 Requirements
- Python 3.x must be installed

### ▶️ Execution

To run the 8-Puzzle:
```bash
python eight_puzzle_bfs.py
python block_arrangement_hill_climb.py
