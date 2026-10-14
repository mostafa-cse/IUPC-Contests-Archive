# Order of Digits

**URL:** https://toph.co/p/priority-of-digits  

---

You will be given a list

$L$

consisting of

$N$

non-negative integers in a decimal number system. We all know that, in the decimal number system, there are 10 digits

$(0,1,2,3,4,5,6,7,8,9)$

. Their order is defined as

$(0 < 1 < 2 < 3 < 4 < 5 < 6 < 7 < 8 < 9)$

.

In this problem, you will be given some queries. In each query, you will be given a modified order of the 10 digits as a list

$P$

and an integer,

$X$

. Here,

$P$

denotes the modified order of digits as

$P[0] < P[1] < P[2] < P[3] < P[4] < P[5] < P[6] < P[7] < P[8] < P[9]$

. The answer to the query is the number of integers that are less than the given integer

$X$

in list

$L$

(applying the modified digit order described by

$P$

). The order of digit

$0$

will not be modified.

Input

First line of the input contains a single integer

$N$

$(1 \leq N \leq 10^5)$

. The next line will contain

$N$

space-separated integers

$L_{0}, L_{1}, … , L_{N-1}$

which are the elements of the list

$L$

and

$0 \leq L_{i} \leq 10^{18}$

.

After that, there will be an integer

$Q(1 \leq Q \leq 10^5)$

denoting the number of queries. Each of the queries will contain

$11$

space-separated integers. The first

$10$

integers will denote the list,

$P$

. The

$11^\text{th}$

integer will denote the value of

$X$

$(0 \leq X \leq 10^{18})$

. It is guaranteed that

$P[0] = 0$

for each of the queries.

Output

For each test case, print the number of integers that are less than the given integer

$X$

in list

$L$

applying modified digit priority. Print the answer in a new line.

Example


---

## Samples

### Sample Input 1
```
3
10 20 30
1
0 9 8 7 6 5 4 3 2 1 10
```

### Sample Output 1
```
2
```
