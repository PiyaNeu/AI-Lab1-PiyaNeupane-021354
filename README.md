# Vacuum Cleaning Agents

This project implements three types of intelligent agents for a vacuum cleaning environment, modeled on a 10x10 grid world. Each agent demonstrates a different level of intelligence in decision-making, from simple reflex responses to utility-optimized behavior.

## Environment

- Grid: 10x10
- Each cell: Can be either **clean** or **dirty**
- Agent Actions: `suck`, `move up`, `move down`, `move left`, `move right`
- Agent's start position is randomized
- Goal: Clean all dirty cells efficiently

---

## Agents

### 1. Simple Reflex Agent

A simple reflex agent that selects actions based solely on the current percept (clean or dirty).

- **Input:** Current cell state (dirty or clean)
- **Output:** Action (`suck`, `move` in random direction)
- **Behavior:** If cell is dirty, suck. Otherwise, move randomly.
- **Simulation:** 20 steps
- **File:** `simple_reflex_agent.py`

---

### 2. Goal-Based Agent

A goal-based agent that maintains an internal model of the environment and uses search strategies to clean all dirty cells.

- **Input:** Current cell state and internal model of the grid
- **Output:** Sequence of actions to clean grid
- **Behavior:** Move to the nearest dirty cell and clean it
- **Simulation:** Until grid is fully clean
- **File:** `goal_based_agent.py`

---

### 3. Utility-Based Agent

A utility-based agent that selects actions to maximize cumulative utility (e.g., cleaning efficiency and minimal movement).

- **Input:** Current cell state and internal model of the grid
- **Output:** Sequence of utility-optimized actions
- **Utility Function:**  
  - Cleaning dirty cell: +5  
  - Each move: -1
- **Behavior:** Clean cells while minimizing movement cost
- **File:** `utility_based_agent.py`

---

## Getting Started

### Requirements

- Python 3.x

### Run Agents

```bash
python simple_reflex_agent.py
python goal_based_agent.py
python utility_based_agent.py
