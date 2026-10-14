# A Unique Array

**URL:** https://toph.co/p/a-unique-array  

---

An array is called "unique" if it has no consecutive element with same value(

$\text{A[i] != A[i-1]}$

).

Given a unique array

$A$

of

$N$

integer and

$q$

queries. Each query will contain 2 integer

$x$

,

$y$

which updates the value of index

$x$

to

$y$

(

$\text{A[x] = y}$

). After each query, if the array is not unique, delete some elements from

$A$

to make it unique. Output the maximum size of

$A$

which is unique.

Input

Input starts with an integer

$T$

(

$1 ≤ T ≤ 10$

), denoting the number of test cases. The next line contains two integers N (

$1 ≤ N ≤ 10^5$

), q (

$1 ≤ q ≤ 10^5$

).

The next line contains

$N$

space separated integers forming the array

$A$

.

The next

$q$

lines will contain a query which is in the form

$\text{x y}$

(

$0 ≤ x < |A|$

,

$1 ≤ y ≤ 10^9$

).

Output

For each test case, print the case number in a single line. Then for each query you have to print a line containing the output: the maximum size of

$A$

which is unique.

Example


---

## Samples

### Sample Input 1
```
2
5 3
1 2 3 4 5
0 2
3 3
2 3
1 1
10
0 4
```

### Sample Output 1
```
Case 1:
4
4
2
Case 2:
1
```
