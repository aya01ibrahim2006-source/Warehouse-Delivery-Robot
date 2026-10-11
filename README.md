Warehouse Delivery Robot — Search Algorithms
Project Overview

This project implements two search algorithms to solve a warehouse delivery robot pathfinding problem:

Breadth-First Search (BFS)
A* Search

The robot must find a path from a starting cell (S) to a goal cell (G) on a grid while avoiding walls and accounting for terrain movement costs.

Grid Symbols
Symbol	Meaning	Movement Cost
S	Starting position	0
G	Goal position	1
.	Normal floor	1
~	Rough floor	3
#	Wall	Cannot enter
Algorithms
Breadth-First Search (BFS)

BFS explores the grid level by level and finds a path with the minimum number of moves. It does not guarantee the cheapest path when terrain movement costs differ.

A* Search

A* combines the actual cost from the starting position with a heuristic estimate of the remaining cost to guide its search.

The heuristic used is Manhattan distance:

h(n) = |row_goal - row| + |col_goal - col|

Test Maps

The algorithms are evaluated on MAP_A, MAP_B, and MAP_C.

MAP_C has no valid path from the start to the goal.

How to Run
Open Warehouse_Delivery_Robot.ipynb in Jupyter Notebook or Google Colab.
Run the notebook cells in order.
Set RUN_ALL_MAPS = True to run both algorithms on all three maps.
To run one map only, set RUN_ALL_MAPS = False and choose the desired map using the GRID variable.
Evaluation Metrics

The algorithms are compared using:

Path length
Total path cost
Number of expanded nodes
Maximum frontier size
Execution time
Technologies
Python
Jupyter Notebook
heapq
collections.deque
time

Team Members:
Aya Ibrahim — A* Search implementation.
Esraa Mahmoud — BFS implementation.

course:Intelligent Systems — Task 1
