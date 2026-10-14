# Problematic Problem Setters

**URL:** https://toph.co/p/problematic-problem-setters  

---

A new national level contest will be held next month. So chief judge asked some problem setters to set the problem and provide some easy problems. These problem setters live in a city called “Bazingapore”, where they have a very good metro rail system. This metro rail system consists of MRT stations. MRT stations are connected with other MRT stations by rail tracks on which train travels both ways. And obviously, these rail tracks don’t create any kind of loops (what’s the point, huh?).

Now problem setters require to discuss with each other, so they need to meet. But some of the problem setters are quite lazy, so they don’t want to cross MRT stations more than K times. So that means, from their starting stations to the ending stations there should not be more than K stations (including the ending one, excluding the starting one). This constraint made the Chief judge worried, so he wants to find out how many stations are there which can be visited by these problematic problem setters given that they don’t want to cross more than

K

MRT stations.

Input

Input starts with an integer

T (≤ 10)

, denoting the number of test cases.

Each case starts with three integers

N M K(2 ≤ N, M ≤ 100,000, 1 ≤ K ≤ 100,000)

denoting the total number of MRT stations in the system, the total number of problematic problem setters and value K stated above. The stations are numbered from 1 to N. Each of the next N-1 lines will contain two integers

u v (1 ≤ u, v ≤ N, u ≠ v)

denoting that station

u

and

v

are connected by a two-way rail track. Then the next line will contain

M

integers which denote the starting station numbers for each of the problematic problem setters.

Output

For each test case, output one line containing Case x: y, where x is the test case number (starting from 1) and y is the total number of MRT stations where all these problematic problem setters will be able to meet with each other without crossing more than

K

stations.

Example

Notes

Explanation:

There are 8 MRT stations, 3 problem setters will start from these 1, 4, 5 numbered station and no problem setters want to cross more than 2 stations. So from the station 1 one problem setter can go to any station except station numbered 8. On the other hand, both problem setter from station 4 and 5 can go to stations numbered 1, 3, 4, 5. So all the problem setters can meet on any of these stations 1, 3, 4, 5.

Hint: Think the MRT map as a Tree.


---

## Samples

### Sample Input 1
```
1
8 3 2
1 2
1 3
1 6
3 4
3 5
6 7
7 8
1 4 5
```

### Sample Output 1
```
Case 1: 4
```
