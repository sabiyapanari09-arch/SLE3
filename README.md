SLE-3: Architectural Design Using Full C4 Model (BFS vs. DFS)

This repository contains the architectural design and Full C4 Model documentation for Self-Directed Learning Exercise 3 (SLE-3) in the course 02AML204 – Introduction to Artificial Intelligence.

The project presents the architecture of the BFS vs. DFS Maze Path-Finding System at four levels: Context, Container, Component, and Code.

1. Project Overview & Student Identification
Student Name: Sabiya Abubakar Panari
Course Code: 02AML204 – Introduction to Artificial Intelligence
Division: SY_AIML
Academic Year: 2026–2027
SLE: SLE-3 – Architectural Design Using Full C4 Model
System Title: BFS vs. DFS – Maze Path-Finding Profiling
Primary Deliverable: SLE-3 Architectural Design Report
Repository Content: C4 architecture diagrams, code-level flowchart, documentation, and supporting project files
2. Project Description

The BFS vs. DFS Maze Path-Finding System compares Breadth-First Search (BFS) and Depth-First Search (DFS) on randomly generated grid mazes.

The system finds paths from a start point to a goal and evaluates the algorithms using performance measures such as:

Execution time
Number of nodes expanded
Path length
Profiling information

The SLE-3 architecture represents the system using the Full C4 Model, progressing from a high-level system view to the main code-level functions.

3. C4 Model Architecture

The repository documents the following four levels of the C4 Model:

Level 1 – Context Diagram

Shows the BFS vs. DFS Maze Path-Finding System as a whole and its interaction with the maze input and the resulting path and performance information.

Level 2 – Container Diagram

Describes the major containers/modules of the system:

Maze Input / Generator
Search Engine
BFS Module
DFS Module
Performance Profiler
Output / Results
Level 3 – Component Diagram

Provides a more detailed view of the Search Engine and its internal components:

Frontier
Visited Set
Goal Test
Path Reconstructor

These components work together to control the search process and reconstruct the final path.

Level 4 – Code Level Overview

Shows the major functions involved in implementing the system:

generate_maze() – Generates the maze.
get_neighbors() – Finds valid neighbouring cells.
bfs() – Performs Breadth-First Search.
dfs() – Performs Depth-First Search.
reconstruct_path() – Reconstructs the final path.
time.perf_counter() – Measures execution time.
cProfile – Profiles program performance.
4. Code-Level Flow

The code-level architecture follows this general flow:

generate_maze()
       ↓
get_neighbors()
       ↓
 ┌───────────────┐
 │               │
bfs()          dfs()
 │               │
 └───────┬───────┘
         ↓
reconstruct_path()
         ↓
time.perf_counter() + cProfile
         ↓
Output / Results

This flow represents how the maze is generated, neighbouring cells are identified, BFS and DFS perform the search, the resulting path is reconstructed, and performance information is collected.

5. Repository Structure
SLE-3/
│
├── README.md
│
├── SLE3_PRN_SabiyaPanari.docx
│
├── diagrams/
│   ├── context-diagram.png
│   ├── container-diagram.png
│   ├── component-diagram.png
│   └── code-level-flowchart.png
│
├── code/
│   └── maze_pathfinding.py
│
└── documentation/
    └── SLE3_C4_Architecture.pdf

File names can be adjusted to match the actual files committed to the repository.

6. Design Decisions

The architecture separates maze generation, search algorithms, performance profiling, and output so that each part has a clear responsibility.

BFS and DFS are represented separately because they use different search strategies and data structures. The Search Engine coordinates the search process, while the Performance Profiler records the execution and performance information.

7. Objectives of SLE-3

The main objectives of this SLE are:

To represent the BFS vs. DFS system using the Full C4 Model.
To understand the architecture at Context, Container, Component, and Code levels.
To identify the major modules and components of the system.
To map the architecture to the main implementation functions.
To clearly document the relationship between maze input, search algorithms, profiling, and output.
8. Tools & Technologies
Programming Language: Python
Algorithms: Breadth-First Search (BFS), Depth-First Search (DFS)
Profiling: time.perf_counter(), cProfile
Architecture Model: Full C4 Model
Documentation: Markdown / Word / PDF
Diagrams: C4 architecture diagrams and code-level flowchart
9. Expected Outcome

The SLE-3 deliverable provides a structured architectural view of the BFS vs. DFS Maze Path-Finding System.

The Full C4 Model makes it easier to understand the system from a high-level context down to the individual functions used in the implementation.

10. Conclusion

This repository documents the architectural design of the BFS vs. DFS Maze Path-Finding System using the Full C4 Model. The four C4 levels provide progressively detailed views of the system and show how the maze input, search algorithms, performance profiling, and results are connected.

The architecture complements the SLE-2 performance benchmarking work by providing a clear structural view of the system being evaluated.
