### How To Run
```
./Graph_Maxflow 8 1000 '/home/vietph/workspace/GraphCutCuda/images/160_15.637790_1608895250805.png' '/home/vietph/workspace/GraphCutCuda/images/168_30.608816_1608895250965.png' 1 64 2 10 10
```

- 1st arg: **blockDimy:** size of block_dim_y (8).
- 2nd arg: **number_loops:** maximum number loop for running push, relable kernels.
- 3nd arg: left side image.
- 4th arg: right side image.
- 5th arg: number of iteration to calculate average execution time.
- 6th arg: **backwardCycle:** number of iterations between 2 backward bfs calls.
- 7th arg: **relabelCycle:** number of iterations between 2 relabel kernal calls.
- 8th arg: **averageDistance:** number of latest iterations to calculate average number of active nodes.
- 9th arg: **stopPoint:** lower threshold of average number active nodes to terminate algorithm.