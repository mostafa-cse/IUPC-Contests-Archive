# All the Cuts

**URL:** https://toph.co/p/all-the-cuts  

---

In a two dimensional plane, there are “R” red points, “B” blue points and “G” green points. These points are expressed as ordered pair (x, y), x being the abscissa and y being the ordinate. For red points, y > 0. For other points, y < 0. We will call CD a cut on AB if line segment AB intersects line segment CD where A is a red point, B is a blue point and C, D are green points. For a line segment AB there can be arbitrary number of cuts.

Let us define a function F(i, j) to be the number of ways there can be “i” cuts on line segment "j" where "j" is a line segment connecting a red point and a blue point as mentioned above. Again, let us define a function g(p, q, j) as:

$ g(p, q, j) = (F(p, j) - F(p+1, j) + F(p+2, j) - F(p+3, j) \space ... upto \space F(q, j)) \space modulo \space (10^9 + 7) $

Find the sum of g(p, q, j) for all j, modulo 109+7.

Input

The first line will contain integer

T

denoting number of test cases.

The next line will contain integer

R

denoting number of red points. The next R lines will contain two integer denoting the co-ordinate of the red points. The sum of all red points over all test cases will be between 1 and 2000 (inclusive).

The next line will contain integer

B

denoting number of blue points. Next B lines will contain two integer denoting the co-ordinate of the blue points. The sum of all blue points over all test cases will be between 1 and 2000 (inclusive).

The next line will contain integer

G

denoting number of green points. Next G lines will contain two integer denoting the co-ordinate of the green points. The sum of all green points over all test cases will be between 1 and 2000 (inclusive).

The x and the y co-ordinates of all points will be between -108 and 108 (inclusive).

Next line will contain two integer denoting

p

and

q

(1 ≤ p ≤ q ≤ 108).

For a single test case, there will not be any 3 points lying on same straight line.

Output

Print one line for each test case denoting the answer. Check sample output for actual output format.

Example

Notes

In the first test case, for segment AB joining point (0, 5) and (0, -500) there can be at most 2 cuts. So,

$ F(1, AB) = 2 $

$ F(2, AB) = 1 $

So,

$ g(1, 2, AB) = F(1, AB) - F(2, AB) = 2 - 1 = 1 $

Since, in there can be only one segment joining red points and blue points g(1, 2, AB) is the answer.

In the second test case, there will be two segment for which we have to calculate function g. For both of them the value of function g is 1. So, the answer is 1 + 1 = 2.


---

## Samples

### Sample Input 1
```
2

1
0 5
1
0 -500
3
-1 -1
1 -1
1 -2
1 2

1
0 5
2
0 -500
-1 -501
3
-1 -1
1 -1
1 -2
1 2
```

### Sample Output 1
```
1
2
```
