![image](https://github.com/user-attachments/assets/a27f4225-92c8-455c-9dd5-bce720384619)# Ex25 Adjacency List Representation
## DATE:16.04.25
## AIM:
To write a C program to represent the given graph using the adjacency list.

## Algorithm
1. Read the number of vertices and number of edges.
2. Read all edge pairs (source and destination) and store them.
3. Create a graph using the input edge list.
4. Print the adjacency list representation of the graph.

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: GOKUL SHARAN R
RegisterNumber: 212223040052
*/
```
```
int main(void)
{ int n,i;
 scanf("%d",&N);
 scanf("%d",&n);
 // input array containing edges of the graph (as per the above diagram)
 // (x, y) pair in the array represents an edge from x to y
 struct Edge edges[n];
 for (i = 0; i < n; i++)
 {
 // get the source and destination vertex
 scanf("%d",&edges[i].src);
 scanf("%d",&edges[i].dest);

 }

 // construct a graph from the given edges
 struct Graph *graph = createGraph(edges, n);
 // Function to print adjacency list representation of a graph
 printGraph(graph);
 return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/fded249a-7d1e-430d-a16a-8200aa367940)





## Result:
Thus, the C program to represent the given graph using the adjacency list is implemented successfully
