# DAA_Assignments

Name : Aparna Jha

Roll no: A 04

DAA Assignment 1

Aim : Google Map database and construction of Minimum Cost Spanning Tree From any selected City Input: Google Map actual data: Refer google map and find out distance between 7 cities. Construct distance matrix. Use distance matrix to construct Minimum Cost Spanning Tree using Prims Algorithm. Write three observations on the output.

Theory :

It starts with an empty spanning tree. The idea is to maintain two sets of vertices. The first set contains the vertices already included in the MST, the other set contains the vertices not yet included. At every step, it considers all the edges that connect the two sets and picks the minimum weight edge from these edges. After picking the edge, it moves the other endpoint of the edge to the set containing MST.

The idea behind Prim’s algorithm is simple, a spanning tree means all vertices must be connected. So the two disjoint subsets (discussed above) of vertices must be connected to make a Spanning Tree. And they must be connected with the minimum weight edge to make it a Minimum Spanning Tree.

Follow the given steps to find MST using Prim’s Algorithm:

Create a set mstSet that keeps track of vertices already included in MST.

Assign a key value to all vertices in the input graph. Initialize all key values as INFINITE. Assign the key value as 0 for the first vertex so that it is picked first.

While mstSet doesn’t include all vertices

Pick a vertex u which is not there in mstSet and has a minimum key value.

Include u in the mstSet.

Update the key value of all adjacent vertices of u. To update the key values, iterate through all adjacent vertices. For every adjacent vertex v, if the weight of edge u-v is less than the previous key value of v, update the key value as the weight of u-v.

Observation

1.The shortest distance according to the minimum cost spanning tree is from nagpur to hyderabad.

2.The first two selected edges are Amritsar and Patna having the shortest distance according to the matrix.

3.Hyderabad is close to Mumbai and Kanyakumari similarly Patna is close to Kolkata and nagpur as compared to others.
