# Computer Science 220S2C (2022)

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


若您有关于此作业的任何需求，本人主页, 可添加vx：codingtutor 或者qq：122929048