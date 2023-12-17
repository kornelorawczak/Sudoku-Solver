# sudoku-solver
Python program which uses generators to recursevily yield all the possible solution of the given sudoku puzzle

## Usage
Create sudoku board that you want to be solved by the program like the one below
```python
test_board = [ #0 means an empty spot to be filled
    [5, 3, 0, 0, 7, 0, 0, 0, 0],
    [6, 0, 0, 1, 9, 5, 0, 0, 0],
    [0, 9, 8, 0, 0, 0, 0, 6, 0],
    [8, 0, 0, 0, 6, 0, 0, 0, 3],
    [4, 0, 0, 8, 0, 3, 0, 0, 1],
    [7, 0, 0, 0, 2, 0, 0, 0, 6],
    [0, 6, 0, 0, 0, 0, 2, 8, 0],
    [0, 0, 0, 4, 1, 9, 0, 0, 5],
    [0, 0, 0, 0, 8, 0, 0, 7, 9]
]
```
Then input the name of the list which conatins your board like below
```python
def main():
    for solution in sudoku_solver(test_board):
        print_board(solution)
```
