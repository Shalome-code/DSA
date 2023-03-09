# DSA
BFS-for finding the shortest path from a node to all the other nodes.
Shortest path in unweighted graph
1. Initialize dist[v]={inf,inf,inf,....}
2. dist[s]=0
3. Create a queue, q
4. Initialize: visited[v]={false,false,...}
5. q.push(s), visited[s]=true
6. while(q is not empty)
u=q.pop()
for every adjacent v of u
{
if(visited[v]==false)
{
dist[v]=dist[u]+1
visited[v]=true
q.push(v)
}
}
print dist[]
Complexity = O(V+E)

Detect cycle in undirected graph


DFS- is recursive technique

Topological sorting (Kahn's Algorithm)
In directed graph- eg - when some tasks are dependent on other and need to be traversed first
for this we need to have indegree[] of the graph, if we have controll over addEdge method, we can invcrement the indegree array when we add an edge. Or we can travse the adj list of the graph and increment the indegree[] array.
Algorithm
1. Store indegree of every vertex.
2. Create a queue, q
3. Add all 0 indegree vertexs to the queue
4. while(q is not empty){
a) u=q.pop()
b) print u
c)For every adjacent v of u
 i)reduce degree of v by 1
 ii)If indegree of v becomes 0, add v to the q.
}
Complexity - O(V+E)

============================================
Minimum Spanning Tree/ Prim's algorithm
Its used for weighted, undirected, connected graph
