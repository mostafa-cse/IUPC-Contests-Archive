# Shine on You Crazy Diamond

**URL:** https://toph.co/p/shine-on-you-crazy-diamond  

---

This problem is authored by one of our late friends, Sifat, who unexpectedly left us last year. He was a brilliant programmer, an astute philosopher and an amazing human being. Had he been with us, he would have been delighted to see this year’s brilliant IUPC coming to life and would wish you good luck for the contest. We sincerely hope you enjoy his problem.

You are given an array

$a$

of size

$n$

. You can select a number

$x > 1$

(

$x$

may or may not be an element of

$a$

) and remove every multiple of

$x$

from the array. You need to find the minimum size of the array

$a$

after performing this operation exactly twice.

Input

The first line contains an integer,

$n (1 \leq n \leq 10^5)$

.

The second line contains

$n$

space-separated integers

$a_1, a_2, \cdots, a_n (1 \leq a_i \leq 10^6)$

.

Output

On the first line, output a single integer, the minimum size of array

$a$

after performing this operation exactly twice.

On the second line, output two integers

$x_1$

and

$x_2$

$(2 \leq x_1, x_2 \leq 2^{31}-1)$

, the chosen values of

$x$

for the two operations.

Examples


---

## Samples

### Sample Input 1
```
4
4 8 25 21
```

### Sample Output 1
```
1
4 21
```

### Sample Input 2
```
3
2 4 6
```

### Sample Output 2
```
0
2 1605113
```
