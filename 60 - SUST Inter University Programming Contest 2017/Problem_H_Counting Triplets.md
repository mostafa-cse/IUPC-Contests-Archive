# Counting Triplets

**URL:** https://toph.co/p/counting-triplets  

---

Given an array of

$N$

integers

$A_1$

,

$A_2$

,

$A_3$

, …,

$A_N$

. Vector has to find the number of Fibonacci Triplets in the array meaning how many triplets

$(i, j, k)$

are there such that

$1 ≤ i < j < k ≤ N$

and

$A_i$

+

$A_j$

=

$A_k$

.

For example,

$(2, 3, 5)$

,

$(4, 9, 13)$

are Fibonacci Triplets but

$(2, 4, 5)$

,

$(4, 3, 8)$

are not.

Input

First line of the input contains an integer

$T$

(

$1 ≤ T ≤ 5$

) denoting the number of test cases. Next line contains an integer

$N$

(

$1 ≤ N ≤ 10^5$

) denoting the size of the array. Following line contains N space separated integers

$A_1$

,

$A_2$

,

$A_3$

, …,

$A_N$

(

$1 ≤ A_i < 2^{16} – 1$

).

Output

For each test case, print the number of ways to choose a Fibonacci Triplet from the array of

$N$

integers in a separate line.

Example

Notes

The input files are large. Please use faster I/O.


---

## Samples

### Sample Input 1
```
1
6
2 3 3 4 7 11
```

### Sample Output 1
```
3
```
