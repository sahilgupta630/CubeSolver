# Rubik's Cube Solver

A C++ program that models a Rubik's Cube in multiple ways (1D Array, 3D Array, Bitboard) and solves it using various graph search algorithms (BFS, DFS, IDDFS, IDA*). It also includes a Pattern Database for more efficient heuristic estimates during search.

## Features
- **Models**:
  - `RubiksCube1dArray`: A flat array representation.
  - `RubiksCube3dArray`: A 3x3x6 multi-dimensional array representation.
  - `RubiksCubeBitboard`: A compacted 64-bit integer based representation per face for extremely fast operations.
- **Solvers**:
  - Breadth-First Search (BFS)
  - Depth-First Search (DFS)
  - Iterative Deepening DFS (IDDFS)
  - Iterative Deepening A* (IDA*) using Corner Pattern Databases
- **Pattern Databases**: Database to compute heuristic bounds for IDA*.

## Build
Use CMake to build the project.
```bash
mkdir build
cd build
cmake ..
cmake --build .
```
