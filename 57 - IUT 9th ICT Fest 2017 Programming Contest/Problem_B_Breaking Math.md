# Breaking Math

**URL:** https://toph.co/p/breaking-math  

---

The worst of them is Heisenburg, a badass physicist and the ultimate druglord. Walter needs Heisenburg’s active support to distribute the methamphetamine he produces. Alas, Heisenburg is a cautious man. Heisenburg is initially skeptical about Walter, and decides to give the following problem to Walter in order to prove his worth.

w(n)

is defined to be the number of distinct prime factors of

n

.

w(1) = 0, w(2) = 1, w(3) = 1, w(4) = 1, w(5) = 1, w(6) = 2, w(30) = 3

f(n, k)

is defined to be the sum of

kw(i)

for

i

in range

1

to

n

.

**

f(n, k) =

Σ

k w(i)

Given

n

and

k

, calculate

f(n, k).

Input

The first line contains an integer

t (1 ≤ t ≤ 100)

, denoting the number of test cases. Each of the next

t

lines contain two integers,

n (1 ≤ n ≤ 1011)

and

k (1 ≤ k ≤ 10)

, separated by a single space. Sum of

n

will not exceed

1011

in an input file.

Output

For each case, output a line of the format

Case X: Y

, where

X

is the case number, starting from

1

, and

Y

is the required answer. You can safely assume that the answer will fit in a

signed 64 bit integer

.

Example

Notes

Heisenburg is Walter's alter ego!


---

## Samples

### Sample Input 1
```
10
1 1
2 2
3 3
4 4
5 5
6 6
7 7
8 8
9 9
10 10
```

### Sample Output 1
```
Case 1: 1
Case 2: 3
Case 3: 7
Case 4: 13
Case 5: 21
Case 6: 61
Case 7: 85
Case 8: 113
Case 9: 145
Case 10: 271
```
