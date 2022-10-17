若您有关于此作业的任何需求，本人主页, 可添加vx：codingtutor 或者qq：122929048

# Computer Science 220S2C (2022)

## Assignment 4 Assignment 4 (traversal and optimisation)
Please submit only Python source code (.py extensions only).
1. Arithmetic trees 30 marks
You are given an input  le with multiple pairs of input lines. The  rst line of each
pair is a tree given as a predecessor array. The second line is the value at the
corresponding node. Values at leaf nodes (nodes with no children) are integers. At
non-leaf nodes, the two possible values are + or  .
The tree represents an arithmetic expression where the value at a non-leaf node u is
the sum of values at the children of u in the case of +, or the product of values at
the children of u in the case of  .
You need to calculate the value at each node and output the calculated value at the
root. The tree is not constrained to be binary.
Input format: Input consists of m pairs of lines of comma separated values, so
2m lines in total. The  rst line is each pair is a comma separated list of integers
representing a tree in predecessor array format where 􀀀1 represents null.
The second line in each pair is a comma separated list of integers and the symbols +
and  . The ith item on the list is the value or operator at the ith node in the tree.
For example:
-1,0,0,0,1,1
+,*,2,3,0,7
2,0,-1,0
+,3,*,3
Output format: For each pair of input lines, output a line containing the value
calculated at the root of the tree.
For the example input above, output would be:
5
6

2. Optimisation 30 Marks
Consider a digraph G with non-negative arc weights. Your task is to  nd the length
of the shortest route from a speci ed source, s, to a speci ed destination, t, with the
added complication that you would also like to pass through node u if doing so does
not increase the route length by more than 25%.
For each input digraph, the program should output one of:
(a) the length of the shortest route from s to t via u so long as this length is no
greater than 1.25 times the shortest path from s to t; or,
(b) the length of the shortest path from s to t if the route through u is too long; or,
(c) -1 if t is not reachable from s.
Any pair, or all three, of the nodes s, t, and u can be identical. All arc weights will
be integers.





## Assignment 3 (Basic graph algorithms and traversals)

This assignment requires you to submit programs in Python that you have written yourself
to the automarker, https://www.automarker.cs.auckland.ac.nz. Your implementation
must be from  rst principles and cannot use an existing library methods that might solve
the problem (eg performs graph operations etc).
The automarker runs on a Linux box. Read the automarker help and FAQ for more
details.
Please submit only Python source code (.py extensions only).


1. Delete a node from a digraph 30 Marks
For each digraphs in a set of digraphs with order at least 3 given as adjacency lists,
read in the digraph, delete the node with index n 􀀀 3 where n is the order of the
digraph, and write the digraph back to  le.
Input format: described below under the heading \Digraph input format".
Output format: the same as the input format. Ensure that you maintain the node
naming conventions.
For the example input shown below, the  rst digraph would have node with index
1 removed, and the second graph would have node index 0 removed, so the output
would be
2. Forward and cross arcs in a DFS 30 Marks
For a given set of digraphs, write a program that performs DFS on each digraph
starting at node 0 and prints out the  rst forward arc and  rst cross arc encountered
in the traversal. Use our standard convention that when there is a choice of white or
grey nodes, the one with the lowest index should be chosen.
Input format: described below under the heading, \Digraph input format".
Output format: For each input digraph, print out two lines. The  rst line has
the  rst forward arc encountered, the second line has the  rst cross arc encountered.
Write the arc (u; v) as u,v. If the required forward or cross arc does not exist, output
an empty line in its place.
For the example input shown below, the output (including blank lines) would be
3. BFS to  nd distances 30 Marks
Write a program that performs BFS on each of a given set of digraphs starting at
node 0 and prints the distance to the most distant node from 0 and reports the node
with the lowest index at that distance. Nodes that are not reachable from 0 have an
unde ned distance and should be ignored.
Input format: described below under the heading, \Digraph input format".
Output format: For each input digraph, print out a line with the distance to the
most distant node, then a space, then the lowest index of a node at that distance.
Ignore nodes that are not reachable from 0.
For the example input shown below, the output would be
