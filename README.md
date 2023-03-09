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
