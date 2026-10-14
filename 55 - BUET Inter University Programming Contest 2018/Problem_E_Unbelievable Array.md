# Unbelievable Array

**URL:** https://toph.co/p/unbelievable-array  

---

You will be given an array A of n integers and q operations. There are two types of operations:

1 x y

, for this operation, you should replace all the occurrences of element

$x$

in the array with

$y$

2 idx

, output the value

$A[idx]$

Input

Input starts with an integer

$T$

(

$1 \le T \le 10$

), denoting the number of test cases.

The first line of each case contains two integers

$n$

and

$q$

(

$1 \le n, q \le 100000$

). The next line contains

$n$

space separated integers

$A_1$

,

$A_2$

,

$A_3$

, …,

$A_n$

(

$1 \le A_i ≤ 100000$

) forming the initial array.

Each of the next

$q$

lines contains the described operations:

1 x y

:

$1 \le x, y \le 100000$

2 idx

:

$1 \le idx \le n$

Output

For each test case, print

$\texttt{Case t:}$

(

$\texttt{t}$

is the test case number) in the first line. Then for each 2nd type of operation, output the answer.

Example


---

## Samples

### Sample Input 1
```
1
5 4
1 2 3 4 5
1 1 3
2 1
1 3 5
2 1
```

### Sample Output 1
```
Case 1:
3
5
```
