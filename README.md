# Maze AI Agent

An autonomous AI agent that navigates a grid-based maze by reading a local **state vector**
and selecting actions to efficiently reach a goal. The agent interacts with an external
simulator through a defined input/output interface and demonstrates core AI decision-making
concepts such as perception, policy design, and control.

This project was originally developed as part of an Exploratory AI course and has been
refactored into a standalone repository.

---

##  How It Works

- At each timestep, the agent receives a **state vector** representing the 8 surrounding
  cells in the maze (walls, free space, goal, etc.).
- Based on this local observation, the agent selects an action:
  - `UP`
  - `DOWN`
  - `LEFT`
  - `RIGHT`
- The action is written back to the simulator, which advances the environment.
- This loop continues until the agent reaches the goal or the episode ends.

The focus of this project is the **agent’s decision logic**, not the simulator itself.

---
