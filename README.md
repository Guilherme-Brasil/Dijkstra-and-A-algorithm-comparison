# Dijkstra's and A* algorithm comparison
>Author: Guilherme Araújo Brasil
>
>2023.2
## Dijkstra's Algorithm
Dijkstra's algorithm, designed by Dutch computer scientist Edsger Dijkstra in 1956 and published in 1959 calculates, the minimum cost path between vertices of a graph. Choosing a vertex as the root of the search, this algorithm calculates the minimum cost of this vertex for all the other vertices of the graph.
The algorithm begins with a start point or root. Every arc that out or arrive on this root has a positive cost. At the beginning, the Cost Matrix it's full checked with infinity costs. The iterations of the code will write the costs on the locations with output arcs, while the locations with arrive arcs keep with infinity cost.


![image](https://github.com/Guilherme-Brasil/Dijkstra-and-A-algorithm-comparison/assets/75508707/92225b90-3ec1-4023-b04d-98f6034f393f)



When we find a path with lowest cost, the previous root is removed and the new root is the vertex found. The process move on. the code ends when the best path with the lowest cost to the last vertex is found.


![image](https://github.com/Guilherme-Brasil/Dijkstra-and-A-algorithm-comparison/assets/75508707/bf5193b7-42c5-4d61-a119-e1643a028f0b)



Dijkstra's algorithm is a good algorithm, but its search method requires a long running time. To find the lowest cost path between two points, the algorithm traverses a very large area of ​points to find the correct path, which requires a good amount of processing time.

## A* Algorithm
The A* algorithm is a practical algorithm that is often used to traverse maps to find the shortest path to take. A* was initially designed as a graph traversal problem, to help build a robot capable of finding its own course. 

It looks for shortest paths first, making it an ideal and complete algorithm. An optimal algorithm will find the lowest cost result for a problem, while a complete algorithm will find all possible results for a problem, as is the case with Dijkstra's algorithm.

The A* algorithm can also be implemented in graphs that have costs on their edges, that is, it means that the algorithm can follow the path with the lowest cost and find the best route in terms of distance and time.


![image](https://github.com/Guilherme-Brasil/Dijkstra-and-A-algorithm-comparison/assets/75508707/588545f2-72e9-43e7-9e06-57fec731dc4c)


When analyzing the A* algorithm, we can see that its search time is much smaller than the Dijkstra's algorithm, making its use more advantageous. The method used analyzes points close to the lowest cost path and not a very large area.

A* tries to look for a better path by using a heuristic function, which gives priority to nodes that are supposed to be better than others while Dijkstra's just explore all possible ways. A* uses an additional heuristic function in the cost calculation to inform its search. The heuristic function acts as a hint to guide the algorithm towards the destination, and hopefully reducing the search space. Heuristics are admissible calculations within the scope of the work. There are several formulas that can be implemented in the algorithm under study.

The differential for Dijkstra's algorithm is that, in addition to analyzing the cost of the edges between points, the A* algorithm will calculate the distance between the current point of study and the destination point, giving preference to the point geographically closer to the end point . This reduces processing time and memory usage by the CPU.
