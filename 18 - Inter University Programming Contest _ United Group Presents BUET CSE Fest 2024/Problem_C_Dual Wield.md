# Dual Wield

**URL:** https://toph.co/p/dual-wield  

---

For an array

$X$

of natural numbers, define

$F(X) =  Len^{\dag}(Set^{\ddag}(X))$

. You are given two arrays

$A$

and

$B$

of size

$n$

. For any

$1 \leq i \leq n$

, you can swap

$A_i$

and

$B_i$

. Output the maximum value of

$F(A) + F(B)$

along with

$A$

and

$B$

after doing all operations. You can do any non negative integer number of operations.

$\dag Set(X) = \{x: x \in X\}$

i.e. the set formed by taking unique elements from array

$X$

.

$\ddag   Len(S) =$

Number of elements in set

$S$

.

Input

The input format is as below.

$N$

$A_1 \; A_2 \; \cdot\cdot\cdot A_N$

$B_1 \; B_2\; \cdot\cdot\cdot B_N$

Here

$N$

is the size of array

$A$

and

$B$

.

$\textbf{Constraints:}$

$1 \leq N \leq 2\times 10^5$

$1 \leq A_i \leq 2N$

$1 \leq B_i \leq 2N$

Output

Print

$3$

lines. On the first line, print the maximum possible value of

$F(A) + F(B)$

. On the second and the third line, print array

$A$

and

$B$

respectively after doing all operations.

Examples

Notes

In the

$1^{st}$

sample, after swapping

$A_2$

and

$B_2$

,

$F(A) = 2$

and

$F(B) = 1$

. Thus

$F(A) + F(B) = 3$

which is maximum.


---

## Samples

### Sample Input 1
```
2
1 1
1 2
```

### Sample Output 1
```
3
1 2
1 1
```

### Sample Input 2
```
1
1
1
```

### Sample Output 2
```
2
1
1
```
