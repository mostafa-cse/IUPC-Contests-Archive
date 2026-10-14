# Just Primes II (Easy)

**URL:** https://toph.co/p/just-primes-ii-easy  

---

Given a positive integer N, calculate the minimum number of distinct primes required such that their sum equals to N.

Input

The first line contains an integer

T

(1 ≤ T ≤ 50), denoting the number of test cases. Each of the next T lines contains a single integer

N

(1 ≤ N ≤ 50).

Output

For each test case, output one integer X. X denotes the minimum number of distinct primes required such that their summation equals to N. If it is not possible to express N as a summation of distinct primes, set X to -1 and output it.

Example

Notes

When N = 10, the minimum number of distinct primes is 2 and there is only 1 way to represent 10 as a sum of 2 different prime numbers:

$ 3 + 7 = 10 $

When N = 27, the minimum number of distinct primes is 3:

$ 3 + 5 + 19 = 27 $


---

## Samples

### Sample Input 1
```
4
1
2
10
27
```

### Sample Output 1
```
-1
1
2
3
```
