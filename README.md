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
