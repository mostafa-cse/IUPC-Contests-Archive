# Doctor Strange in the Circleverse

**URL:** https://toph.co/p/doctor-strange-in-the-circleverse  

---

At the beginning of time, there were only two circles in the circleverse (a universe where everyone is a circle). They are called the first generation of the circleverse and known as

$C(a)$

and

$C(b)$

, where

$C(r)$

denotes a circle with radius

$r$

.

Each year, a new generation of the circleverse is created from the previous one. Each generation of the circleverse consists of all circles in it positioned side by side on a straight line. To create the new generation, each pair of adjacent circles of the previous generation creates a new circle and positions it between them. The new circle gets a radius equal to the sum of the two adjacent circles it is created from. The figure below shows the first three generations of a circleverse.

Doctor Strange, the master of mystic arts, has explored the multiverse and found two circleverses

$C_1$

and

$C_2$

. First generation of

$C_1$

consists of circles

$C(0)$

and

$C(1)$

. On the other hand, both circles of the first generation of

$C_2$

are

$C(1)$

. Doctor Strange wants to use

$C_1$

and

$C_2$

to create a new generation of circles he calls super-circles.

Let,

$C(x)$

=

$i$

th circle of the

$n$

th generation of

$C_1$

$C(y)$

=

$i$

th circle of the

$n$

th generation of

$C_2$

$P$

= number of circles in the

$n$

th generation of a circleverse

Doctor Strange will create

$P$

super-circles initially. The

$i$

th super-circle will be created from

$C(x)$

and

$C(y)$

and it will be

$C(x+y)$

. After that, Doctor Strange will destroy all unstable super-circles. A super-circle

$C(x+y)$

is unstable if

$x>y$

or

$y>n$

. To destroy these unstable super-circles, he needs to summon enough energy from the multiverse. The amount of the energy required depends on the number of unstable super-circles.

Since Doctor Strange is the master of mystic arts, not mathematics, he needs your help to calculate the number of unstable super-circles. Given

$n$

, calculate the number of the unstable super-circles Doctor Strange will have to destroy.

Input

First line of the input will contain an integer

$T$

, the number of test cases.

Each of the next

$T$

lines will contain an integer

$n$

, indicating that circles from the

$n$

th generation will be used to create super-circles.

$1≤T≤10^5$

$1≤n≤10^7$

Output

For each test case, print the number of the unstable super-circles modulo

$10^9+7$

in a single line.

Example


---

## Samples

### Sample Input 1
```
5
1
3
5
12
100
```

### Sample Output 1
```
0
0
6
2002
988182602
```
