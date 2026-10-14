# Bikpik Colony

**URL:** https://toph.co/p/bikpik-colony  

---

Bikpiks are very small aliens. Day by day they are becoming very dangerous for human being. They live at some colonies in space. The colonies are so small, you can assume a colony as a point in 3D cartesian coordinate. It is guaranteed that all colonies are

coplanar

(a set of points in space are coplanar if there exists a geometric plane that contains them all).

Captain Gomo is assigned to save the earth from Bikpiks. He decided to destroy all the Bikpik colonies. To destroy the colonies:

1. He encloses a volume with a particular cover.
2. The colonies inside the volume which are at least **D** units away from the cover, are destroyed. Note that, there might be a point inside the volume which is not **D** units away, in that case, it will not be destroyed. Also, the cover is not reusable. He repeats this process until all the colonies are destroyed.

The ingredients of the cover are costly. So he wants to minimize the total surface area required for the covering task.

Input

The first line of the input contains an integer

T

(

T ≤ 25

), the number of test sets.

Each set of input starts with line containing two integers

N

(

N ≤ 12

) and

D

(

1 ≤ D ≤ 103

).

N

denotes the number of Bikpik colonies. Following

N

line contain three space separated integers

X

,

Y

and

Z

(

−103 ≤ X, Y, Z ≤ 103

) denoting three coordinates of each colonies.

Each test set starts with a blank line.

Output

For each case, print the minimum surface area in single line. Error less than

10-4

will be ignored.

Example

Notes

In second test case, he covers up first three colonies together and remaining one in separately.


---

## Samples

### Sample Input 1
```
2

1 10
3 4 -5

4 10
0 0 0
0 10 0
10 0 0
999 999 0
```

### Sample Output 1
```
1256.6370614359
3685.8809474056
```
