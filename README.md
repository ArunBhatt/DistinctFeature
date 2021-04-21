# DistinctFeature
You are given N positions in a queue Each of the positions contains elements of specific features denoted by specific integers. You can traverse the whole queue and select K positions that contain the same features. The selected K positions are deleted from the queue. The remaining places are considered for the next iteration. If you cannot select K positions, then no places can be deleted from the queue

Your task is to minimize the numbers of distinct specific integers in the queue available after each iteration You are given Q queries and each query contains an integer P For each query, print the number of distinct specific integers present in the queue after P iterations

Input format
• First line. Three space-separated integers N. K. and Q
• Next line: N-space-separated integer Os denoting the specific feature present at the position
• Next Q lines: An integer Pdenoting the number of iterations
Output format
• For each query print the answer in we
Constraints
• 1<=N<=10^6
• 1<=K<=10
• 1<=Q<=10^5
• 0<=Ci<=10^5
• 1<=P<=N


Sample Input:
	5 1 3
	5 0 1 2 1
	1
	5
	3
	
Sample output:
	3
	0
	1


Explanation
Let's consider the number of distict colors after 3 iteration(3rd query). In each iteration Mrs Carterremoves 1 student from the line.
One of the possibles ways can be:
1. In iteration 1 she removes student 1 with '5' colored candy from the line
2. In iteration 2 she removes student 2 with '0' colored candy from the line
3. In iteration 3 she removes student 4 with '2' colored candy from the line
Hence only 2 candies both of color '1' remains in line. Number of distict color remaining is 1.
