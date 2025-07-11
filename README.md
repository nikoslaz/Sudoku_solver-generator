# Sudoku Solver and Generator

A C program that can solve, validate, and generate Sudoku puzzles with options for unique solutions.

## Features

- **Solve** existing Sudoku puzzles
- **Validate** whether a Sudoku puzzle is correct
- **Generate** new Sudoku puzzles with:
  - Configurable number of filled cells
  - Option for puzzles with unique solutions
- Error detection and reporting

## Requirements

- C compiler (gcc recommended)
- Standard C library

## Installation

1. Clone this repository
2. Compile the program:
   ```bash
   make
   
## Usage

```bash
./sudoku [options]

## Options

- `(no options)` — Solve the puzzle read from stdin  
- `-c` — Check if the puzzle (from stdin) is valid  
- `-g <nelts>` — Generate a new puzzle with `<nelts>` filled cells  
- `-u` — (with `-g`) Ensure puzzle has unique solution
```

## Input/Output Format

- Puzzles are represented as 9x9 grids  
- Empty cells are represented by `0`  
- Numbers are space-separated  

**Example:**

```txt
5 3 0 0 7 0 0 0 0
6 0 0 1 9 5 0 0 0
0 9 8 0 0 0 0 6 0
8 0 0 0 6 0 0 0 3
4 0 0 8 0 3 0 0 1
7 0 0 0 2 0 0 0 6
0 6 0 0 0 0 2 8 0
0 0 0 4 1 9 0 0 5
0 0 0 0 8 0 0 7 9
```
## Implementation Details

- Uses backtracking algorithm for solving  
- Puzzle generation ensures validity at each step  
- Unique solution check performed during generation  
- Cell choices tracking for efficient solving  

---

## Limitations

- Generation of very sparse puzzles (<25 clues) may be slow when requiring unique solutions  
- No graphical interface (terminal only)  
