It increases the availability and use of rental cars among travelers and visitors in the state.Used to calculate its cost and minimum distance traveled in a trip.

Floyd Warshall Algorithm:

1) Consider first row and first column.
  include all dis[i][j] and dis[i][k],which have direct edge.
  execute d(i, j) = min{d(i, j), d(i, k) + d(k, j)}

2) For every pair (i, j) of the source and destination vertices respectively, there are two possible cases. 
  k is not an intermediate vertex in shortest path from i to j. We keep the value of dist[i][j] as it is. 
  k is an intermediate vertex in shortest path from i to j. We update the value of dist[i][j] as dist[i][k] + dist[k][j] if dist[i][j] > dist[i][k] + dist[k][j]

3) Next we repeat same for each row and column.
