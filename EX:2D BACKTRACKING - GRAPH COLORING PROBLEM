# EX:2D BACKTRACKING - GRAPH COLORING PROBLEM

### DATE:

## AIM:
To solve the Graph Coloring Problem using backtracking, assigning colors to the vertices of a graph such that no two adjacent vertices share the same color while minimizing the number of colors used.

## ALGORITHM:

1. Start with the first vertex v = 0.
2. Try all colors 1 to m for vertex v.
3. For each color, check if it’s safe (i.e., no adjacent vertex has the same color).
4. If safe, assign the color and recursively assign colors to the next vertex.
5. If all vertices are colored successfully, return success.
6. If no color can be assigned, backtrack and try a different assignment.
7. If all possibilities are exhausted, print that no solution exists.

## PROGRAM:

```
# Program to implement Graph Coloring Problem using backtracking.
#Developed by: SWATHI D
#Register Number: 212222230154
```
``` 

class Graph:
    def __init__(self,vertices):
        self.V=vertices
        self.graph=[[0 for row in range(vertices)] for column in range(vertices)]
        
    def isSafe(self,v,colour,c):
        for i in range(v):
            if self.graph[v][i]==1 and colour[i]==c:
                return False
        return True
        
    def graphColourUtil(self,m,colour,v):
        if v==self.V:
            return True 
        for i in range(1,m+1):
            if self.isSafe(v,colour,i):
                colour[v]=i
                if self.graphColourUtil(m,colour,v+1):
                    return True
        return False
        
    def graphColouring(self,m):
        colour=[0]*self.V
        if not self.graphColourUtil(m,colour,0):
            print("No solution Exist")
            return False
        print("Solution exist and Following are the assigned colours:")
        
        for c in colour:
            print(c,end=' ')
        print()
        return True
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/c304d885-a973-45a1-adeb-f4bba4e75c1b)

## RESULT:

The Graph Coloring Problem was successfully implemented using backtracking. The program correctly assigns colors to the vertices such that no two adjacent vertices have the same color.
