# Rubik's-cube-solver
A C++ implementation of a Rubik’s Cube solver using multiple search algorithms.
The project explores efficient cube representations and heuristic-driven solving techniques to tackle the challenge of 43 quintillion possible states.


## Features

**Multiple cube representations**:
3D Array, 1D Array, and Bitboard models.

### Implemented solvers:
***BFS (Breadth-First Search)*** – guarantees shortest solution but memory-heavy

**DFS (Depth-First Search)** – memory efficient, may return longer solutions.

**IDDFS (Iterative Deepening DFS)** – balance of DFS + BFS.

**IDA*** – heuristic-driven, fast for large state space.

- Pattern Databases for corner heuristics to improve performance.
- Modular design – easy to extend with new heuristics or cube models.

## How to Build & Run
### Prerequisites
- C++17 or later
- CMake 3.10+
- A C++ compiler (GCC/Clang/MSVC)

### Build & Run
clone the repo
git clone https://github.com/<your-username>/rubiks-cube-solver.git
=> cd rubiks-cube-solver

create build directory => mkdir build && cd build

Run CMake => cmake ..

compile => cmake --build . 

Run => rubiks_cube_solver.exe (for windows)
    => ./rubiks_cube_solver (for Linux/macOS)

## What it Shows
- BFS = shortest solutions but memory-heavy
- DFS = faster but longer solutions
- IDDFS = balance of speed & memory
- IDA* = best performance with heuristics

## How It Works
1. The cube is represented internally as arrays or bitboards.
2. A solver algorithm explores possible moves (U, D, L, R, F, B).
3. The algorithm searches until it reaches the solved state.
4. The solution path (sequence of moves) is printed.

***Example (BFS or IDA*)***:

Scrambled Cube → Apply Solver → Solution Sequence → Solved Cube



## Algorithm Comparison

| Algorithm | Completeness | Optimality | Memory Usage | Speed        |
| --------- | ------------ | ---------- | ------------ | ------------ |
| BFS       | ✅ Yes        | ✅ Optimal  | ❌ Very High  | ❌ Slow       |
| DFS       | ✅ Yes        | ❌ No       | ✅ Low        | ⚡ Fast       |
| IDDFS     | ✅ Yes        | ✅ Optimal  | ✅ Low        | ⚡ Medium     |
| IDA\*     | ✅ Yes        | ✅ Optimal  | ✅ Efficient  | 🚀 Very Fast |

## Future Improvements
- Add a 3D visualizer (React + Three.js).
- Create a web API to expose the solver.
- Deploy as a full-stack app where users scramble & solve interactively.

## Skills Demonstrated
- Advanced search algorithms (BFS, DFS, IDA*).
- Heuristic design using pattern databases.
- Memory-efficient data structures.
- C++ programming & build systems (CMake).

    
