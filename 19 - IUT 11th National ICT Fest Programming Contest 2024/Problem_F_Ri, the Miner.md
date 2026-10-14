# Ri, the Miner

**URL:** https://toph.co/p/ri-the-miner  

---

Gondor has

$n$

circular gold mines with IDs from

$1$

to

$n$

containing some gold. Each mine’s center can be located by a 2D coordinate.

Ri, the miner, lives in a place in Gondor that a coordinate on a 2D plane can locate. She can dig mines that only cover her place. In other words, she can dig a mine if her location lies inside or on the boundary of that mine.

Even though it would have been better to dig all the mines, she is unable to move much for sickness and can only dig one mine at most. So, she wants to dig the mine that contains the most amount of gold. Help her find the most suitable one.

Input

The first line of the input will consist of an integer

$t\ ( 1\le t\le 10^5)$

$-$

the number of testcases. The description of each testcase follows:

The first line of the testcase will consist of an integer

$n\ ( 1\le n\le 3\cdot10^5)$

$-$

the number of gold mines.

Next

$n$

lines will contain four integers,

$M_{x_i},\ M_{y_i},\ r_i,\ a_i$

$(-10^9\le M_{x_i}, M_{y_i}\le 10^9,$

$\ 1\le  r_i,\ a_i\le 10^9)$

$-$

the coordinates of the center of the mines, the radius of the mines, and amount of gold in each mine respectively.

Next line will contain an integer

$q\ (1 \le q \le 3\cdot10^5)$

$-$

number of queries.

Each query will contain two integers in a line,

$x_i, y_i\ ( -10^9\le x_i, y_i\le 10^9)$

$-$

coordinates of Ri’s location.

Additional constraints for the queries: Either

$x_i - x_{j} = 0$

or

$y_i - y_{j} = 0$

or both for all

$1\le i < j\le q$

.

Moreover, you can assume that the sum of

$n$

and the sum of

$q$

over all testcases will not exceed

$3\cdot10^5$

respectively.

Output

For each query, print the ID of the mine that Ri will dig. If there are multiple mines, print the minimum ID. If no mines cover Ri’s place, print

$-1$

.

Example


---

## Samples

### Sample Input 1
```
1
3
0 0 1 3
-1 0 1 10
-1 -1 2 9
3
-1 -2
-1 1
-1 2
```

### Sample Output 1
```
3
2
-1
```
