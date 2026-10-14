# Walking Down The Road

**URL:** https://toph.co/p/walking-down-the-road  

---

There is an M meter long road with the leftmost point of the road being the 0 meter point and the right most point being the M meter point. N people are standing at different points on the road. Akina is a great problem solver. He likes to solve problems that are related to real life. Akina is thinking if the N peoples wanted to meet at certain point and they will just walk straight to that point from their position. If X is point where they can meet such that the summation of the distances each has to walk is minimum is called “Fuchka” point. Suppose a point can contain infinitely many people.

You are given a similar problem. Suppose you have to say a random point between 0 to M. What is the probability of the random point being the “Fuchka” point?

Input

First line will contain an integer

T (1 ≤ T ≤ 5)

, the number of test case. Then for each case There will be two lines. First line will contain two integers

N

and

M

;

(1 < N ≤ 100000)

and

(N ≤ M ≤ 2000000)

and

N is even

.

The next line will contain

N

number of integers the value of which will be between

0

to

M

inclusively. These points are the position of the people. No two points will be same.

Output

For each case output a real number, the probability of the point being Fuchka point in a line.Error less then .000001 will be acceptable.

Example


---

## Samples

### Sample Input 1
```
2
4 4
1 2 3 4
2 6
0 6
```

### Sample Output 1
```
.250000
1.000000
```
