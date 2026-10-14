# Find the primes?

**URL:** https://toph.co/p/find-the-primes  

---

For a positive integer n, let’s define a function f:

f(n) = sum of positive integers less than n which are relatively prime to n.

Suppose,

n = 6. So, f(6) = 1 + 5 = 6.

n = 10. So, f(10) = 1 + 3 + 7 + 9 = 20.

Given f(n) you have to find n. If there are multiple answers print any of them.

If there is no answer then just print -1.

Input

The first line of the input contains a single integer T denoting the number of test cases. The description of test cases follows. For a single test case, there will be a single integer denoting f(n).

Constraints:

1 ≤ T ≤ 500, 1 <= f(n) <= 10^18

Output

For each case, print the answer in a separate line.

Example

Notes

Note : x is relatively prime to y if greatest common divisor of x and y is 1.


---

## Samples

### Sample Input 1
```
4
2
3
4
10
```

### Sample Output 1
```
-1
3
4
5
```
