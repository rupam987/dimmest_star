# dimmest_star

Dimmest Star
Sophia is sitting on the roof of her house on a moonless night looking up at a collection of stars. She mentally marked them with numbers from 1 to n. She picked out the brightest star in the sky and connected them with other stars in decreasing order of brightness.

She’s bewildered with such a large connected network of stars. She wants to know which star is dimmest. Can you help her?

The problem can be seen as a uni-directional non-cyclic graph with n-1 edges.

Example
[refer graph.png]


Here 5 is the brightest and 1 is the dimmest. You may assume that stars in one “level” of the graph are of the same brightness. That is, in the case above, stars 6 and 2 are of the same brightness level while 3 and 4 are also equally bright.

So the output will be 1.

Note that if there’s more than one dimmest star, the output should be the star with the lowest index.

Input Format
The first line contains ‘t’ which is the no. of test cases.

For each test case, the first line is an integer n which is the number of stars. Then n - 1 lines follows consisting of two space separated integers a b. This represents a directed edge connecting a to b.

The last line is an integer which represents the starting point (the brightest star.)

Output Format
For every test case, print out a single integer which is the index of the dimmest star.

Constraints
0 < t < 200 (number of test cases)

0 < n < 10000 (number of points in the graph)

Sample input
2
7
5 6
5 2
6 4
6 3
4 7
7 1
5
10
7 2
7 3
7 6
7 4
7 10
3 5
6 8
6 1
8 9
7
Sample Output
1
9
Explanation of Sample test case:
There are 2 test cases. The first test case is explained in the example where the result was 1.

In second test case there are 10 points in the graph and 7 is the starting point.

The longest path from 7 is 7->6->8->9. So, 9 is the answer. And just to be clear, in this example, stars 4, 2, 6, 3 and 10 are of the same brightness level. 1, 8 and 5 are all equally bright as well.
