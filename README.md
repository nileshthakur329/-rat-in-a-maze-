# -rat-in-a-maze-
problem statement                                                      
A Maze is given as N*N binary matrix of blocks where source block is the upper left most block i.e., maze[0][0] and destination block is lower rightmost block i.e., maze[N-1][N-1]. A rat starts from source and has to reach the destination. The rat can move only in two directions: forward and down. 

In the maze matrix, 0 means the block is a dead end and 1 means the block can be used in the path from source to destination. Note that this is a simple version of the typical Maze problem. For example, a more complex version can be that the rat can move in 4 directions and a more complex version can be with a limited number of moves.

Algorithm                                                                                  
1.Create a solution matrix, initially filled with 0’s.
2.Create a recursive function, which takes initial matrix, output matrix and position of rat (i, j).
3.if the position is out of the matrix or the position is not valid then return.
4.Mark the position output[i][j] as 1 and check if the current position is destination or not. If destination is reached print the output matrix and return.
5.Recursively call for position (i+1, j) and (i, j+1).
6.Unmark position (i, j), i.e output[i][j] = 0.
