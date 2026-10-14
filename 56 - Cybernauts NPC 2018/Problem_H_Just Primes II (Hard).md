# Just Primes II (Hard)

**URL:** https://toph.co/p/just-primes-ii-hard  

---

Given a positive integer

N

, calculate the minimum number of

distinct primes

required such that their sum equals to

N

. Also calculate the number of different ways to select these primes. Two ways are considered to be different iff there exists at least one prime in one set not existing in the other.

Input

The first line contains an integer

T (1 ≤ T ≤ 500,000)

, denoting the number of test cases. Each of the next

T

lines contains a single integer

N (1 ≤ N ≤ 500,000)

.

Output

For each test case, output two integers

X

and

Y

separated by a single space.

X

denotes the minimum number of distinct primes required such that their summation equals to

N

, and

Y

is the number of ways to select these primes. If it is not possible to express

N

as a summation of distinct primes,

set X and Y to -1

and output them. You can safely assume that the answer will always fit in a

signed 32 bit integer

.

Example

Notes

WARNING: Large input and output (around 4 MB), please use faster I/O methods.


---

## Samples

### Sample Input 1
```
20
1
2
10
27
100
666
1000
1729
4572
4991
10000
100000
480480
482790
499799
499847
499901
499979
499999
500000
```

### Sample Output 1
```
-1 -1
1 1
2 1
3 3
2 6
2 31
2 28
3 2393
2 110
3 13396
2 127
2 810
2 8499
2 8291
3 31121027
3 31139901
3 31124665
1 1
3 30974053
2 3052
```
