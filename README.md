Problem Statements
There are N people in village, who wants to visit Temple outside the village. To reach the temple, villagers
need to cross the river. So, they hire the only available boat which can carry at most two people. Villagers
decided to hire this boat to reach safely by sailing it by themselves. Every part of journey from village to
temple and temple to village has some cost associated with it which is given by an array A[] elements. Array
A[] has n elements, where A(i) represents the cost ith person has to pay if they sail the boat alone. If two
people sail the vehicle, the cost of travel will be the maximum of cost of two people. Calculate the minimum
total cost so that all N people can reach Temple safely.
Input Format
The first line contains, T, denoting the number of test cases. Each test case contains 2 lines each. The first line
has an integer N, denoting the number of persons. Next line contains N space separated distinct integers
denoting the cost of ith person.
Constraints
1 ≤ T ≤ 10
1 ≤ N ≤ 100000
1 ≤ A[i] ≤ 1000000


Output Format
For each test case, print the minimum cost required so that all people can reach kingdom.
Sample Input
3
4
4
300 400 600 700
2
1321 2450
3
500 123 873
4
600 800 150 700



Sample Output
2200
2450
1496
2400


Explanation
• In the 1st testcase,300 and 400 go together (which costs 400) and 300 comes back (total cost 700
now). Now 600 and 700 go (total cost 1400) and 400 comes back (total 1800) and now 300 and 400 go
(total cost 2200)!
• In the 2nd testcase, both can reach the temple in 2450 as max (1321,2450) =2450.
• In the 3rd testcase, second and third will go first. So, cost will be max (123,873) =873. Now second
person will come back and take the first along with him. So, coming back cost is 123. Then taking first
one along costs max (123,500) =500.
Therefore, total cost = 500+123+873 = 1496
