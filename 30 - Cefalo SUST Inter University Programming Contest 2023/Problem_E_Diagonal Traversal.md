# Diagonal Traversal

**URL:** https://toph.co/p/diagonal-traversal  

---

You are given an

$n \times m$

grid. You can go from point

$(x_1, y_1)$

to any point

$(x_2, y_2)$

of grid if and only if

$x_1$

is not equal to

$x_2$

and

$y_1$

is not equal to

$y_2$

and their Euclidian distance is an integer value. You have to tell whether you can go from the top left point

$(1, 1)$

to the bottom right point

$(n, m)$

using any number of valid moves.

Input

The first line of input contains a single integer

$T$

$(1 \le T \le 1000)$

, the number of test cases..

For each test case, there are two integers

$n$

$(1 \le n \le 10^{6})$

and

$m$

$(1 \le m \le 10^{6})$

.

Output

For each test case, print “Case X: S”, where “X” is the case number. “S” will be “YES” if it is possible to go from the top left cell (

$1$

,

$1$

) to the bottom right cell (

$n$

,

$m$

), and “NO” otherwise.

Example

Notes

Euclidean distance between two points coordinates (

$x_1$

,

$y_1$

) and (

$x_2$

,

$y_2$

) is given by

$\text{dist}\left(\left(x_1, y_1\right), \left(x_2, y_2\right)\right) = \sqrt{\left(x_1 - x_2\right)^2 + \left(y_1 - y_2\right)^2}$


---

## Samples

### Sample Input 1
```
2
1 1
2 2
```

### Sample Output 1
```
Case 1: YES
Case 2: NO
```
