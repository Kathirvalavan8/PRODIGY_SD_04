Sudoku Solver

This is a Python-based command-line Sudoku solver that uses recursive backtracking to fill in missing numbers in a 9×9 grid. It prints both the unsolved and solved Sudoku boards in a clean, readable format.

Features
- Solves standard 9×9 Sudoku puzzles using backtracking
- Validates moves based on row, column, and 3×3 box rules
- Displays the grid with visual separators for clarity
- Handles unsolvable puzzles gracefully

File Structure
sudoku.py         # Main solver logic and grid display
README.md         # Project documentation



How to Run
python sudoku.py


Works with both Python 2 and Python 3. If using Python 2, replace print() with print "" or use from __future__ import print_function.


Sample Output
Unsolved Sudoku:

5 3 . | . 7 . | . . . 
6 . . | 1 9 5 | . . . 
. 9 8 | . . . | . 6 . 
---------------------
8 . . | . 6 . | . . 3 
4 . . | 8 . 3 | . . 1 
7 . . | . 2 . | . . 6 
---------------------
. 6 . | . . . | 2 8 . 
. . . | 4 1 9 | . . 5 
. . . | . 8 . | . 7 9 

Solved Sudoku:

5 3 4 | 6 7 8 | 9 1 2 
6 7 2 | 1 9 5 | 3 4 8 
1 9 8 | 3 4 2 | 5 6 7 
---------------------
8 5 9 | 7 6 1 | 4 2 3 
4 2 6 | 8 5 3 | 7 9 1 
7 1 3 | 9 2 4 | 8 5 6 
---------------------
9 6 1 | 5 3 7 | 2 8 4 
2 8 7 | 4 1 9 | 6 3 5 
3 4 5 | 2 8 6 | 1 7 9 



How It Works
- print_grid(grid): Displays the Sudoku board with separators
- find_empty(grid): Locates the next empty cell (value 0)
- is_valid(grid, num, pos): Checks if placing num at pos is valid
- solve(grid): Recursively fills the board using backtracking
