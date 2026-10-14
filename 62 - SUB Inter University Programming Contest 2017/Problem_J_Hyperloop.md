# Hyperloop

**URL:** https://toph.co/p/hyperloop  

---

Hyperloop is the latest product from Inter Union Pathway Committee. Hyperloop is used to accelerate a car to go from one union to another. More precisely, Hyperloop consists of a circle of radius

r

, connected to a road at point

A

. The road is a linear segment of

D

distance, from

A

to

B

point.

Any car wants to travel through Hyperloop starts at

A

point with 0 velocity. For practical purpose, you can consider it as a point. From

A

point, it can go on the circle with acceleration

a

. That is all the time it spent in the circle, it's velocity will be increased with acceleration

a

. When crossing the

A

point, the car can choose to leave the circle and go through the road to point

B

crossing

D

distance with a constant velocity.

We want to minimize the time needed to go from point

A

to point

B

. Help us to choose an optimal radius

r

for the cycle so that the car needs minimum time to go through it. Notice the minimum time should consist of the time spent in the circle as well as the time spent on road.

Input

First line of the input is positive integer T(T<=1000000), number of test cases. Then T lines follows. In each line there will be two integers, a and D(1<= a,D <= 1000000000000000000 or 10^18).

Output

For each test case, print the value of r which ensure minimum travel time. Difference less 1e-7 will be ignored.

Example


---

## Samples

### Sample Input 1
```
1
2 2
```

### Sample Output 1
```
0.159154943
```
