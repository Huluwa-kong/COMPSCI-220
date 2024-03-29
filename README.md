若您有关于此作业的任何需求，本人主页, 可添加vx：codingtutor 或者qq：122929048

# Computer Science 220SC (2023)

## Assignment 3 (Hashing and Graph Representation)

Problem Statement
Two programs are required to understand basic hashing techniques. We will use open ad- dressing collision resolution with rightward (increase) probing. For a digraph G, let DS be the concatenation of integers (as strings) from a decreasing sorted degree sequence of G. Program 1: OALP hashing with H1 Program 2: OADH hashing with H1 and   = H2 H1: do middle-squaring on DS.

Let d equal the integer obtained from the three middle digits of DS. (append 0's if length of DS < 3 or even)
Hash value is the integer denoted by the three middle digits of d2. (also append 0's if needed) H2: do truncation on DS.
The initial hash value is the integer denoted by the  rst three digits of DS plus one. (prepend 0's if length of DS < 3)
For subsequential probes decrease this hash value by one until it is one. Input will be a sequence of adjacency lists of digraphs (at most 1000) and we want to hash each to an integer using these two hash functions H1 and H2. Input will follow the adjacency list format as described in the CS220 textbook. Here, the  rst line for eaach diagraph is an integer n indicating the order of the digraph. This is followed by n white space separated lists of (out-) adjacencies for nodes labeled 0 to n 􀀀 1. The last digraph of the sequence will be a digraph of order 0 and this is not to be processed (e.g. not added to hash table). For both programs output a binary string of length 1000, which is your  xed hash table size. The bit at position i denotes that some digraph was (1/true) or was not (0/false) hashed to value i. Output each bit on a single line using characters 0' and 1' and terminated with a newline `nn'. Thus, your program's output will be  xed at 1000 lines (2000 bytes). After experimenting with your programs (on several data sets), can you say which program performs better in practice in hashing random sequence of digraphs? Consider cases where there are few (<100) graphs and many (>800) graphs, with respect to your hash table size.
Submission and Due Date
Submit your source code to https://www.automarker.cs.auckland.ac.nz. There will be two test cases provided for each problem. A maximum of 10 submissions is allowed before a penalty of 20% will be applied. The deadline is 23.59pm (automarker time) on the 30th of September. The marks for this assignment is worth 7.5% of your course grade. Some partial credit may be given if you do not achieve \Correct" (green) on the automarker. Note we use plagiarism detection software so do not share any source code with your fellow students, nor use any AI tools (see https://academicintegrity.cs.auckland.ac.nz/).




## Assignment 3 (Basic graph algorithms and traversals)
1. Delete a node from a digraph and record number of arcs removed 30 Marks
For each digraphs in a set of digraphs given as adjacency lists, read in the digraph,
delete the node with index n − 3 where n is the order of the digraph, and write the
digraph back to the terminal. After the adjacency lists, write out how many arcs
have been removed in the process. Assume input digraphs have order at least 3.
Input format: described below under the heading “Digraph input format”.
Output format: the same as the input format but with one extra line after each
digraph stating the number of arcs that were removed when the node was removed.
Ensure that you maintain the node naming conventions.
For the example input shown below, the first digraph would have node with index
1 removed, and the second graph would have node index 0 removed, so the output
would be
3
2
0
3
2
0
2
0
Here the first line indicates the order of the new digraph is 3, the next three lines
are the three adjacency lists showing the arcs of the this digraph, and the 3 on line
5 indicates that three arcs were removed from the input digraph. The next line has
a 2 indicating that the next digraph has order 2 and so on.

2. Back and cross arcs in a DFS 30 Marks
For a given set of digraphs, write a program that performs DFS on each digraph
starting at node 0 and prints out the total number of back arcs and cross arcs resulting
from the traversal. Use our standard convention that when there is a choice of white
or grey nodes, the one with the lowest index should be chosen.
Input format: described below under the heading, “Digraph input format”.
Output format: For each input digraph, print out a line with the number of back
arcs, then whitespace, and then the number of cross arcs.
For the example input shown below, the output would be
1 0
0 1

3. BFS to find distances 30 Marks
Write a program that performs BFS on each of a given set of digraphs starting at
node 1 and prints the distance to the most distant node from 1 and reports the node
with the highest index at that distance. Nodes that are not reachable from 1 have
an undefined distance and should be ignored.
Input format: described below under the heading, “Digraph input format”.
Output format: For each input digraph, print out a line with the distance to the
most distant node, then a space, then the highest index of a node at that distance.
Ignore nodes that are not reachable from 1.
For the example input shown below, the output would be
2 0
0 1





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
