# Up You Go

**URL:** https://toph.co/p/up-you-go  

---

Arya is taking part in a game of throwing marbles upwards. There are

$n$

participants in this game in total, where Arya is the participant with label

$1$

. Each participant is given a marble and initially each of the marbles are held at ground level (height

$0$

). Each participant

$x$

throws his marble straight upwards at time

$s_x$

with initial velocity

$u_x$

and it drops back on the ground after some time.

The marble will follow basic rules of physics while travelling in the air. So if a marble hasn't yet dropped back on the ground and

$t$

time units have passed since it was thrown with initial velocity

$u$

, its current velocity

$v$

and current height

$h$

can be expressed as follows:

$v = u - gt$

$h = ut -  0.5 * gt^2$

Here,

$g=10$

.

You have to answer

$q$

queries, where you will be given an integer

$T$

in each query.

For each query, count how many marbles have a strictly greater height than Arya's marble at time

$T$

.

Input

First line of the input contains two space-separated integers

$n$

and

$q$

, denoting the number of participants and the number of queries.

Next

$n$

lines each contains two integers

$s_x$

and

$u_x$

, denoting when participant

$x$

threw the marble and its initial velocity.

Next

$q$

lines each contains one integer

$T$

, denoting the query time.

$1 \le n, q \le 10^5$

$1 \le u_x \le 10^8$

$0 \le s_x, T \le 10^8$

Output

For each query, output a single line containing one single integer denoting the number of marbles with a strictly greater height than Arya's marble at the query time.

Example


---

## Samples

### Sample Input 1
```
5 10
5 40
4 50
3 50
2 50
1 50
1
2
3
4
5
6
7
8
9
10
```

### Sample Output 1
```
0
1
2
3
4
4
4
4
3
3
```
