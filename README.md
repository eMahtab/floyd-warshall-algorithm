# Floyd Warshall Algorithm
Floyd Warshall algorithm is used to find the shortest ath from any vertex to any other vertex in a weighted graph.

## Algorithm:
1. Create a 2D array `matrix` of n * n , where n is the number of vertices in the weighted graph
2. Initialize the 2D array `matrix[i][i] = 0` and all other cells as `matrix[i][j] = Integer.MAX_VALUE (some higher value)`
3. Loop over the 2D array n times, k = 0 to less than n, and update the matrix[i][j] as below
```java
for(int k = 0; k < N; k++)
  for(int i = 0; i < N; i++)
    for(int j = 0; j < N; j++)
      matrix[i][j] = Math.min(matrix[i][j], matrix[i][k] + matrix[k][j]);
```

# References :
https://www.youtube.com/watch?v=oNI0rf2P9gE
