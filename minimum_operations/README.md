This project implements a solution to the "Minimum Operations" problem. The problem statement is as follows: given a text file starting with a single character 'H', determine the fewest number of operations needed to reach exactly n 'H' characters in the file. The only operations allowed are 'Copy All' and 'Paste'.

Problem Description
Initial State: The file starts with a single character 'H'.
Operations:
Copy All: Copy everything in the file.
Paste: Paste the copied characters.
Objective: To reach n characters in the file with the least number of operations.
Constraints: If n is less than 2 or not achievable by the given operations, the function returns 0.
Algorithm
The solution to this problem involves understanding the optimal use of 'Copy All' and 'Paste' operations. The key is to minimize the number of operations by efficiently multiplying the number of 'H' characters.

The algorithm finds the prime factors of n.
The sum of these prime factors gives the minimum number of operations required.
Each factor represents a 'Copy All' followed by (factor - 1) 'Paste' operations.
