# Chop Chop

**URL:** https://toph.co/p/chop-chop  

---

There is a convex polygon

$A%$

of

$n$

vertices and you want to divide it into two convex polygons

$P$

and

$Q$

such that their areas are equal (half of

$A$

) and the sum of perimeters of

$P$

and

$Q$

is minimum possible.

Input

The first line of the input is an integer

$T$

which denotes the number of test cases.

For each test case, the first line contains an integer

$n$

, denoting the number of vertices in the polygon

$A$

.

$n$

lines follow,

$i^{th}$

line containing two real numbers (with four digit precision after decimal point)

$x_i, ~y_i$

denoting the co-ordinate of the

$i^{th}$

vertex of

$A$

in a counter-clockwise manner.

Constraints:

$1 \le T \le 100$

.

$3 \le n \le 2 \times 10^5$

.

$-10^7 \le x_i, ~y_i \le 10^7$

.

Sum of

$n$

across all testcases is less than or equal to

$2 \times 10^5$

.

Output

For each test case, output the minimum total sum of perimeters of

$P$

and

$Q$

on a single line.

Your output will be considered correct if the absolute or relative error is less than or equal to

$10^{-6}$

.

Example


---

## Samples

### Sample Input 1
```
1
3
0.0000 0.0000
1000.0000 0.0000
500.0000 1.0000
```

### Sample Output 1
```
2002.0019989980
```
