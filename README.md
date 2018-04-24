# AI1ex3
3.
The program accepts the command line:
search <STACK|FIFO|HEAP> [start] [goal]
For example, if you want to find a path from 0 to 42 using BFS, type
./search FIFO 0 42
.  The
output will be:
Problem: route from 0 to 42
goal reached (5279 nodes visited)
#### fringe statistics:
#size        :   23546
#maximum size:   23547
#insertions  :   28825
#deletions   :    5279
####
The output reports that a path was found after visiting 5279 states (using a FIFO queue, so the
algorithm  is  BFS).  The  search  terminated  after  having  found  the  goal  (42).   At  that  moment,
there were still 23546 states in the FIFO queue left.  The maximum size of the queue during the
search process was 23547 states, and the total number of insertion in the queue was 28825.  The
number of deletions (which is of course the same as the number of visited states) was 5279.
Study  the  supplied  source  code.   Make  sure  you  understand  the  data  structures  used  in  the
program. 


1.  Try to use the program to find paths (using BFS) from 0 to 99, from 0 to 100, and from 0 to
102.  Also try to find a path from 1 to 0, using DFS. Next, try to find a DFS path from 0 to
1.  Explain the results.
2.  Modify the program such that DFS and BFS can solve the above mentioned cases.  Does this
modification have effect on the performance of the algorithm?
3.  Modify the program such that the algorithm prints a solution path and its length and cost.
The above (example) path should be printed as:
0 (+1)-> 1 (*3)-> 3 (*2)-> 6 (*2)-> 12 (*3)->36 (+1)-> 37 (+1)->38
(+1)->39 (+1)->40 (+1)->41 (+1)-> 42
length = 11, cost = 15
4.  Complete the priority queue operations of the abstract data type
Fringe
.
5.  Change the program such that the command line
./search PRIO 0 42
will search for the
optimal cost path from 0 to 42 using the UCS algorithm.  What is (are) the optimal paths
from 0 to 42?
6.  Make (from scratch) a program that solves the problem using iterative deepening.  You are
advised to use explicit recursion.
7.  Compare the performance of the four search algorithms for several inputs.  What are your
conclusion
