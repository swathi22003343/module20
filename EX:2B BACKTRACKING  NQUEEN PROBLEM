# EX:2B BACKTRACKING - NQUEEN PROBLEM

### DATE:

## AIM:
To solve the N-Queen problem using backtracking, which places N queens on an N*N chessboard such that no two queens threaten each other.

## ALGORITHM:

1. Start placing queens column by column, beginning from the first column.
2. For each column, try placing the queen in each row one by one check if the position is safe (no other queen in the same row, upper diagonal, or lower diagonal).
3. If safe, place the queen and recursively try to place the rest.
4. If placing the queen leads to a solution, return True.
5. If no safe row is found, backtrack by removing the previously placed queen.
6. Repeat until all queens are placed or no solution exists

## PROGRAM:

```
Program to implement N-Queen problem using backtracking.
Developed by: SWATHI D
Register Number: 212222230154
```
```

def printSolution(board, N):
    for i in range(N):
        for j in range(N):
            print(board[i][j], end=" ")
        print()
def isSafe(board, row, col, N):
    for i in range(col):
        if board[row][i] == 1:
            return False
    for i, j in zip(range(row, -1, -1), range(col, -1, -1)):
        if board[i][j] == 1:
            return False
    for i, j in zip(range(row, N, 1), range(col, -1, -1)):
        if board[i][j] == 1:
            return False
    return True
def solveNQUtil(board, col, N):
    if col >= N:
        return True
    for i in range(N):
        if isSafe(board, i, col, N):
            board[i][col] = 1
            if solveNQUtil(board, col + 1, N):
                return True
            board[i][col] = 0
    return False
def solveNQ(N):
    if N < 1 or N > 4:
        print("Solution does not exist")
        return False
    board = [[0 for _ in range(N)] for _ in range(N)]
    if not solveNQUtil(board, 0, N):
        print("Solution does not exist")
        return False
    printSolution(board, N)
    return True
if __name__ == "__main__":
    N = int(input())
    solveNQ(N)
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/44d07fa1-2efa-4a75-b620-3c0c24896364)

## RESULT:
The N-Queens problem was successfully implemented using backtracking. A valid arrangement of N queens was displayed such that no two queens attack each other.
