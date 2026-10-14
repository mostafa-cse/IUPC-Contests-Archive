# Ultra-Secured Lab

**URL:** https://toph.co/p/ultra-secured-lab  

---

Professor Lukaku is going to build a lab on a convex polygon region with

$n$

vertices for his experimental purpose. To ensure the confidentiality of his works, he needs to build wall vertical with polygon plane (i.e. in our case, the polygon is on XY-plane and the wall height is expanded along positive Z-axis) having negligible density along the edges of the polygon. However, Professor Lukaku has a weird requirement regarding the wall:

For each possible pair

$(P, B)$

where

$P$

belongs to the set of all points inside the polygon (

including points on the edges of the polygon

) and

$B$

belongs to the set of all points on the edges of the given polygon, if the distance between

$P$

and

$B$

is

$d$

, the height of the wall at

$B$

must be at least

$d^2$

.

The height of the wall need not to be uniform. You need to figure out the minimum possible surface area of the wall.

Input

The first line contains an integer,

$1 \le T \le 2000$

, the number of test cases.

For each test case, the first line contains an integer, the number of vertices of the convex polygon,

$3\le n \le 500$

. Each of the next

$n$

lines contains two integers:

$-5 \times 10^4 \le x \le 5 \times 10^4$

and

$-5 \times 10^4  \le y  \le 5 \times 10^4$

describing a vertex of the polygon. Vertices are given in counterclockwise order. No three consecutive points of a polygon will lie on the same line.

Output

For each test case, output the minimum possible area of the wall. Your output will be considered correct if the absolute or relative error is not larger than

$10^{-6}$

.

Example

Notes

The polygon of the first case:

For this case:

Wall height at point

$(2, 1)$

is

$25$

.

Wall height at point

$(2,-2)$

is

$32$

.

Wall portions on four edges are identical. So we are showing the wall portion from

$(2, -2)$

to

$(2, 2)$

. The height of the wall in this part

$z$

can be represented as,

$z = (y - 2)^2 + 16$

when

$-2 \le y \lt0$

,

$z = (y + 2)^2 + 16$

when

$0 \le y \le 2$

,

$z = 0$

otherwise. The wall area of this portion is

$\frac{304}{3}$

. So the total area is

$4(\frac{304}{3}) = \frac{1216}{3}$

.

The wall portion from

$(2, -2)$

to

$(2, 2)$

is shaded in the following figure:


---

## Samples

### Sample Input 1
```
3
4
-2 -2
2 -2
2 2
-2 2
4
-4 -4
4 -4
4 4
-4 4
4
-4 -2
4 -2
4 2
-4 2
```

### Sample Output 1
```
405.33333333
3242.66666667
1440.00000000
```
