# Sudoku Solver

This is a simple Sudoku solver implemented in Python using backtracking algorithm.

## Overview

The Sudoku solver consists of three main functions:

- `find_next_empty(puzzle)`: Finds the next empty cell in the Sudoku puzzle.
- `is_valid(puzzle, guess, row, col)`: Checks if a guess is valid for a given cell in the puzzle.
- `solve_sudoku(puzzle)`: Solves the Sudoku puzzle recursively using backtracking.

## Usage

To use the Sudoku solver, simply create a Sudoku puzzle as a list of lists, where each inner list represents a row in the puzzle. Use `-1` to represent empty cells. Then call the `solve_sudoku` function with the puzzle as an argument.

Example usage:

```python
example_board = [
    [3, 9, -1, -1, 5, -1, -1, -1, -1],
    [-1, -1, -1, 2, -1, -1, -1, -1, 5],
    # Add remaining rows here
]

if solve_sudoku(example_board):
    print("Solution found:")
    print_sudoku(example_board)
else:
    print("No solution exists!")
