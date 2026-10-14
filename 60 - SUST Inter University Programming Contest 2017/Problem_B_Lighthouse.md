# Lighthouse

**URL:** https://toph.co/p/lighthouse  

---

Safwan is the new governor of the country Homeland. Homeland is formed with set of N islands having N-1 bidirectional bridges among them forming the topology of a tree. Each bridge has unit length of 1 kilometer. Initially some island have small transportable lighthouse. These lighthouse can be lit if it has power supply in it. Power can be supplied directly from a generator located in the same island or any other lighthouse which already has power supply, via cable connection. You have infinite supply of 1 kilometer long cables. You cannot cut or merge any cable but make connection between two lighthouses in adjacent islands. Each island have different cost to install a generator. Now you want to install a generator on an island and powerup all the lighthouses. While moving an island can contain multiple lighthouse and/or a generator but after moving all lighthouses, an island can either contain a generator and a lighthouse or a single lighthouse. The cost of moving a lighthouse to any adjacent island is 1 unit. Now your task is to help Safwan finding the minimum cost.

Input

First line contains number of test cases T (1<=T<=10). First line of each case contains N (1 ≤ N ≤ 100) representing the number of islands. Then there are N-1 lines, i’th line having two integers xi and yi (0 ≤ xi , yi ≤ N-1), representing there is a bidirectional bridge between island xi and yi. Next line contains N integers costi representing cost to install generator at i’th island (0 ≤ costi ≤ 100). Last line contains M (0 < M ≤ N), number of lighthouses, followed by M different integers posi, ( 0 ≤ posi ≤ N-1) representing the initial position of lighthouses in the island.

Output

For each case, print minimal cost to install a generator and power up all the lighthouses, possibly by moving them, along with their case number.

Example


---

## Samples

### Sample Input 1
```
2
5
0 1
1 2
2 3
2 4
2 10 1 5 2
2 1 3
5
0 1
1 2
2 3
2 4
11 4 12 13 14
2 0 3
```

### Sample Output 1
```
Case 1: 2
Case 2: 6
```
