# GoodNodes
We have a list of N nodes with each node pointing to one fo the N nodes. It could even be pointing to itself. We call a node 'good', if it satisfies one of the following properties:

*It is the tail node (marked as node 1)
*It is pointing to the tail node (node 1)
*It is pointing to a good node

You can change the pointers of some nodes in order to make them all 'good'. You are given the description of the nodes. You have to find out what is minimum number of nodes that you have to change in order to make all the nodes good.

Input:
The first line of input contains an integer number N which is the number of nodes.
The next N lines contains N numbers, all between 1 and N.
The first number, is the number of node pointed to by Node 1.
The second number, is the number of node pointed to by Node 2.
The third number, is the number of node pointed to by Node 3.

N is no larger than 1000.

Output:
Print a single integer which is the answer to the problem.

Sample input 1:
5
1
2
3
4
5

Sample output 1:
4

Explanation:
We have to change pointers for four nodes (node #2 to node #5) to point to node #1. Thus, 4 changes are required.

Sample input 1:
5
5
5
5
5
5

Sample output 2:
1

Explanation:
We have to just change node #5 to point to node #1 (tail node) which will make node #5 good. Since all the other nodes point to a good node (node #5), every node becomes a good node.
