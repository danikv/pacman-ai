Daniel Kovachev
315870808

1) this solution supports the exploration order because it shows only one path to end, with one cycle that was
    stopped in the middle.

   This solution is no the cheapest, it did not explore a path that was much quicker. The algorithm ran deeply
   on the first path available.

2) Because in this graph search the step cost is 1 (default edge weight) thus by definition of bfs
    it finds the optimal solution -> the cheapest path.

4) on open maze:
    null heuristic - searches almost all the maze (682 node expanded).
    manhattan heuristic - search less than half the maze (211 node expanded)

   it seems that manhattan heuristic optimizes the search complexity that it cuts expanded node searches
   by more than half!