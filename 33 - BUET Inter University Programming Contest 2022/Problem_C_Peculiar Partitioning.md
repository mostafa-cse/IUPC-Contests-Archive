# Peculiar Partitioning

**URL:** https://toph.co/p/primordial-partitioning  

---

You are given an array

$a$

of length

$n$

. You need to find a sub-sequence

$S$

of the array such that

$gcd(sum(S), sum(\overline S) )> 1.$

In other words, the gcd of sum of elements in

$S$

and sum of elements not in

$S$

is greater than 1. It is also required that both

$S$

and

$\overline S$

are non-empty.

Input

The first line contains an integer,

$n (2 \leq n \leq 10^6)$

.

The second line contains

$n$

space-separated integers

$a_1, a_2, \cdots, a_n (1 \leq a_i \leq 2000)$

.

Output

If there is no sub-sequence of the array such that print a single word “No” .

Otherwise, on the first line print a single word “Yes” . On the second the line print a single integer

$k  \ (1 \leq k \leq n-1)$

, the length of the chosen subsequence. On the third line print

$k$

space seperated distinct integers

$c_1, c_2, \cdots c_k\ (1 \leq c_i \leq n)$

, the indices of the elements of the chosen subsequence.

If there are multiple solutions, print any of them. You can print the indices of the chosen subsequence in any order.

Examples

Notes

Given a sub-sequence

$S$

of an array

$a$

,

$\overline S$

is the sub-sequence formed by taking all elements in

$a$

and not in

$S$

. For example, given an array

$a = [10, 20, 30, 40, 50]$

and the subsequence

$S = [20, 30, 50]$

, then

$\overline S = [10, 40]$

.


---

## Samples

### Sample Input 1
```
5
6 2 3 5 8
```

### Sample Output 1
```
Yes
3
4 2 3
```

### Sample Input 2
```
2
1 3
```

### Sample Output 2
```
No
```
