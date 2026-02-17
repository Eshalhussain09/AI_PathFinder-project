# AI Pathfinder – Visual Search Algorithms

A Python-based visualization tool that demonstrates uninformed search algorithms using Pygame. This project allows users to see how different algorithms explore a grid step-by-step to find a path from a start point to a target.


##  Features

### 6 Search Algorithms with Real-Time Visualization

- BFS (Breadth-First Search)
- DFS (Depth-First Search)
- UCS (Uniform-Cost Search)
- DLS (Depth-Limited Search)
- IDDFS (Iterative Deepening DFS)
- Bidirectional Search

### Interactive Grid

- Place Start node
- Place Target node
- Add Obstacles (Walls)

### Live Statistics Display

- Nodes explored
- Path length
- Frontier size
- Execution time
- Adjustable visualization speed

### Additional Features

- Dynamic obstacles appearing during search
- Pause / Resume
- Reset and Clear controls


## Requirements

- Python 3.7 or higher  
- Pygame 2.0 or higher  

## Installation

### Step 1: check python version
```bash
python --version
```
### Clone the repository
```bash
git clone https://github.com/MaryamZahid-gh/AI-PathFinder-Project
```
### Go into the project folder
```bash
cd AI-PathFinder-Project
```
### Install dependencies
### If using Python 3.14 (recommended)
```bash
pip install pygame-ce
```
### OR if using older Python (3.12 or below)
```bash
 pip install pygame
```
### OR using requirements file
```bash
 pip install -r requirements.txt
```
### Run the application
```bash
python gui_main.py
```


## Controls
| Action                               | Control     |
| ------------------------------------ | ----------- |
| Select algorithm (BFS–Bidirectional) | Keys 1–6    |
| Start / Pause visualization          | SPACE       |
| Reset search                         | R           |
| Clear grid                           | C           |
| Adjust speed                         | + / -       |
| Exit application                     | ESC         |
| Place start, target, walls           | Mouse Click |

## Algorithms Overview
| Algorithm     | Description                        | Optimal | Complete |
| ------------- | ---------------------------------- | ------- | -------- |
| BFS           | Explores level by level            | Yes     | Yes      |
| DFS           | Goes deep before backtracking      | No      | No       |
| UCS           | Expands lowest-cost node first     | Yes     | Yes      |
| DLS           | DFS with depth limit               | No      | No       |
| IDDFS         | Repeated DFS with increasing depth | Yes     | Yes      |
| Bidirectional | Searches from start and goal       | Yes     | Yes      |

## Project Structure
```
AI-PathFinder-Project/
│
├── gui_main.py        # Main application and user interface
├── algorithms.py      # All search algorithm implementations
├── grid_model.py      # Grid and node data structures
├── requirements.txt   # Project dependencies
└── README.md          # Project documentation
```

## Color Legend
| Color  | Meaning           |
| ------ | ----------------- |
| Green  | Start node        |
| Red    | Target node       |
| Gray   | Wall/Obstacle     |
| Yellow | Frontier nodes    |
| Blue   | Explored nodes    |
| Purple | Final path        |
| Orange | Dynamic obstacles |

## How It Works
1. Click to place the start point (green)  
2. Click to place the target point (red)  
3. Click to add walls (gray)  
4. Press 1–6 to select an algorithm  
5. Press SPACE to start visualization  
6. Watch the algorithm explore and find the path  

## requirements.txt Content
pygame>=2.0.0
