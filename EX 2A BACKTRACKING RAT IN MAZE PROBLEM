# EX:2A BACKTRACKING - RAT IN MAZE PROBLEM

### DATE:

## AIM:
To implement the Rat in a Maze problem using backtracking.

## ALGORITHM:

1. Start from cell (0, 0).
2. If current cell is the destination (N-1, N-1), mark it and return success.
3. Check if the current cell is safe (inside bounds and value is 1).
4. If safe, mark the cell as part of the path.
5. Recursively try to move right and down.
6. If neither move works, backtrack (unmark the cell).
7. Repeat until a path is found or all options are exhausted.

## PROGRAM:

```
# Program to implement Rat in a Maze.
# Developed by: SWATHI D
# Register Number: 212222230154

def printSolution(sol):
    for i in sol:
        for j in i:
            print(str(j) + " ", end="")
        print("")
def isSafe(maze, x, y, N):
    return 0 <= x < N and 0 <= y < N and maze[x][y] == 1
def solveMaze(maze):
    N = len(maze)
    sol = [[0 for _ in range(N)] for _ in range(N)]
    if not solveMazeUtil(maze, 0, 0, sol, N):
        print("Solution doesn't exist")
        return False
    printSolution(sol)
    return True
def solveMazeUtil(maze, x, y, sol, N):
    if x == N - 1 and y == N - 1:
        sol[x][y] = 1
        return True
    if isSafe(maze, x, y, N):
        sol[x][y] = 1
        if solveMazeUtil(maze, x, y + 1, sol, N):
            return True
        if solveMazeUtil(maze, x + 1, y, sol, N):
            return True
        sol[x][y] = 0
    return False
if __name__ == "__main__":
    maze = [[1, 0, 0, 0],
            [1, 1, 0, 1],
            [0, 1, 0, 0],
            [1, 1, 1, 1]]
    
    solveMaze(maze)
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/675f9368-449d-4ed1-a992-063d4b95be59)

## RESULT:
The Rat in a Maze program executed successfully. A valid path from the start (0, 0) to the destination (N-1, N-1) was found and displayed using backtracking.
