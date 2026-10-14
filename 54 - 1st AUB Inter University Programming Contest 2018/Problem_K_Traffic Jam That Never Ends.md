# Traffic Jam That Never Ends

**URL:** https://toph.co/p/traffic-jam-that-never-ends  

---

Of all the dysfunctions that plague the world’s megacities, none may be more pernicious than bad (really, really bad) traffic. Sitting still in Dhaka, where bad design takes on epic proportions. In the 2016 Global Liveability Survey, the quality of life report issued annually by the Economist Intelligence Unit, Dhaka ranked 137th out of 140 cities, edging out only Lagos, Tripoli and war-torn Damascus; its infrastructure rating was the worst of any city in the survey. Dhakaites will tell you that the rest of the world doesn’t understand traffic, that the worst traffic jam in Mumbai or Cairo or Los Angeles is equivalent to a good day for Dhaka’s drivers. Experts agree. Sometimes it takes 5 hours to go 5 k.m.

There are many ways to go from one place to another by taking different paths. Zico is very intelligent but lazy. He lives in Dhaka and he needs to go from some places to others. He knows some of the shortest paths and doesn't know some of them. And he is too lazy to figure it out himself. In this problem, the city is represented by a bidirectional graph. The nodes represent places and some queries are given. You have to tell the shortest path from one place to another.

Input

First line will contain an integer denoting the number of test cases, T. Then there will be T cases. Each case will contain two integers N and M. The number of places is N. The places are numbered from 1 to N. And then there will be M lines, each containing three integers a, b, c . It means, there is a direct path from a to b with cost c. Then there will be an integer Q denoting the number of queries. For each query, there will be two integers A, B.

1<=T<=10

1<=N <= 500

1<=M<=1100

1<=Q<=2000

1<=A,B<=N

1<=C<=1000000000

Output

First for each case print "Case #:" without the quote where # represents the case number followed by a newline. Then for each query, print the shortest distance first. Then print the places we need to go through for each query. See sample input and output for details. If it is not possible to go from a to b, just print -1. If there are multiple possible solutions, print the one which is lexicographically largest!

Example


---

## Samples

### Sample Input 1
```
1
7 5
1 2 1
2 3 1
3 4 1
4 5 1
6 7 1
5
1 2
1 5 
6 7
1 6
4 1
```

### Sample Output 1
```
Case 1:
1 1 2
4 1 2 3 4 5
1 6 7
-1
3 4 3 2 1
```
