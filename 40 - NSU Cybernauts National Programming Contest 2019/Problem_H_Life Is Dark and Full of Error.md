# Life Is Dark and Full of Error

**URL:** https://toph.co/p/life-is-dark-and-full-of-error  

---

The problem title doesn't mean anything, right? Wrong! It's a fact!

Anyway, let's get to business. There are two weird persons in two countries. The weird fact about them is that the more distant they are from each other, the more their body hurts. And when they are closest, the pain is minimal. One of the countries is circular and the other one is elliptical. The elliptical country has its main axis parallel to the X-axis of the co-ordinate system.

The two persons can go anywhere in their countries, respectively. Can you find out the minimum distance between them?

The equation of an axis parallel ellipse is

$(x-h)^2 / a^2 + (y-k)^2 / b^2 = 1$

, where

$(h, k)$

is the co-ordinate of the center of the ellipse, and

$2 \times a$

and

$2 \times b$

are the lengths of the axes.

Also, if the two countries overlap anywhere, then the distance is 0.

Input

The first line contains an integer

$T$

(

$1 \le T \le 10^5$

), denoting the number of test cases. Each of the test cases contains 2 lines. The first line contains 3 integers:

$x$

,

$y$

,

$r$

(

$-10^5 \le x, y, r \le 10^5$

), denoting the co-ordinate of the center and the radius of the circle, respectively. The second line contains 4 integers:

$h$

,

$k$

,

$a$

,

$b$

(

$-10^5 \le h, k \le 10^5, 1 \le b < a \le 10^5$

), representing the ellipse. Here,

$a > b$

.

Output

For each test case, you have to output the minimum distance between the two persons. The answer should be rounded to 4 digits after decimal.

Example


---

## Samples

### Sample Input 1
```
2
0 0 1
0 0 4 2
-3 3 1
0 0 4 2
```

### Sample Output 1
```
0.0000
0.5219
```
