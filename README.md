# 🔎 Search Explorer: BFS vs DFS on a Directed Graph

**BSD3513 Introduction to Artificial Intelligence · Lab Report 1**

SD24048 WONG JIA YING 

🌐 **Live App:** [https://lab-report-1-4dbaejccwqcel55glfrhsb.streamlit.app/](https://lab-report-1-4dbaejccwqcel55glfrhsb.streamlit.app/)

💻 **Source Code:** [https://github.com/wongjiaying-wjy/Lab-Report-1](https://github.com/wongjiaying-wjy/Lab-Report-1)

![App overview](image/Title.png)

## About
An interactive Streamlit application that visualizes Breadth-First Search (BFS) and Depth-First Search (DFS) on a directed graph, showing the expansion order, frontier, visited nodes, and search path. Neighbours are explored alphabetically.

## Key Features
- Create a graph or use the default Lab 1 graph.
- Choose the starting node, optional goal node, and search algorithm.
- Explore search steps using the slider.
- Watch the search using Autoplay.
- Compare BFS and DFS side by side in a summary table.
- Reset to the default settings.

## Screenshots

| BFS | DFS |
|---|---|
| ![BFS](image/BFS.png) | ![DFS](image/DFS.png) |

**BFS vs DFS comparison**

![Comparison](image/Table_Comparison.png)

## How to Run
```bash
pip install -r requirements.txt
streamlit run "Lab Report 1.py"
```
The app usually opens at http://localhost:8501.

## Code Overview

| Function | Purpose |
|---|---|
| `normalize()` | Cleans node names and sorts neighbours. |
| `edges_from_text()` | Reads and validates graph input. |
| `search()` | Runs BFS or DFS and returns search results. |
| `draw_graph()` | Draws the graph and highlights nodes. |
| `reset_defaults()` | Restores default settings. |

## Repository Structure
```
Lab-Report-1/
├── Lab Report 1.py
├── requirements.txt
├── README.md
└── image/
```

## Built with
Python · Streamlit · NetworkX · Matplotlib · pandas

## Complexity note
For an adjacency-list graph, both BFS and DFS run in **O(V + E)** time. BFS always finds a path with the fewest edges in an unweighted graph, whereas DFS may return a longer one.
