# Sudoku-Solver-in-java-
🧩 Problem Statement:

Write a program to solve a Sudoku puzzle by filling the empty cells.
A Sudoku solution must satisfy all constraints:

Each row must contain digits 1–9 without repetition.

Each column must contain digits 1–9 without repetition.

Each of the 9 sub-boxes (3×3) must also contain digits 1–9.


The input board is partially filled, where empty cells are represented by '.'.


---

Example Input:

[
  ["5","3",".",".","7",".",".",".","."],
  ["6",".",".","1","9","5",".",".","."],
  [".","9","8",".",".",".",".","6","."],
  ["8",".",".",".","6",".",".",".","3"],
  ["4",".",".","8",".","3",".",".","1"],
  ["7",".",".",".","2",".",".",".","6"],
  [".","6",".",".",".",".","2","8","."],
  [".",".",".","4","1","9",".",".","5"],
  [".",".",".",".","8",".",".","7","9"]
]


---

💡 Approach (Backtracking):

1. Traverse the grid to find an empty cell (.).


2. Try filling it with numbers 1–9.


3. Check if the placement is valid:

Same number not in same row, column, or 3×3 subgrid.



4. If valid → recursively try to solve the rest of the board.


5. If no number works → backtrack (reset the cell to '.').

