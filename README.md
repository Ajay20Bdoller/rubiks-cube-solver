# rubik's-cube-solver
A C++ implementation of a Rubik’s Cube solver using multiple search algorithms.
The project explores efficient cube representations and heuristic-driven solving techniques to tackle the challenge of 43 quintillion possible states.


## Features

**Multiple cube representations**:
3D Array, 1D Array, and Bitboard models.

### Implemented solvers:
***BFS (Breadth-First Search)*** – guarantees shortest solution but memory-heavy.
DFS (Depth-First Search) – memory efficient, may return longer solutions.

IDDFS (Iterative Deepening DFS) – balance of DFS + BFS.

IDA* – heuristic-driven, fast for large state space.

Pattern Databases for corner heuristics to improve performance.

Modular design – easy to extend with new heuristics or cube models.
