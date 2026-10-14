# Not Linkin Park!

**URL:** https://toph.co/p/not-linkin-park  

---

Months have passed. Little Anita has grown up a bit! Instead of playing with simplistic sequences, she grew her interest in real life problems. Recently she encountered a motivating one. It is called LP (Linear Programming):

Maximize or Minimize the cost function:

A

x +

B

y +

C

Absolute value of x and y must be less than or equal to

R

. Also, the following three conditions must hold:

**A1**x + **B1**y operator

C1

**A2**x + **B2**y operator

C2

**A3**x + **B3**y operator

C3

operator might be any of the following: <=, >=, =

An interesting problem indeed. But today Anita is a bit overwhelmed with other thoughts! So you have to solve it on your own; she is rooting for you!

Input

The first line consists of a single positive integer

T

, the number of test cases.

The first line of each test case will contain four space separated integers,

A

,

B

,

C

and

D

.

D = 0

will indicate minimization, and

D = 1

will indicate maximization of the cost function.

The second line will contain one integer,

R

.

Next, there will be exactly three lines each on the format:

**Ai**x + **Bi**y operator

Ci

Constraints:

T<=200

0 < R <= 10^4

All other integers will have absolute value less than or equal to 10^3.

Output

Output the maximum or minimum value as asked, rounded to three decimal places. If no solution exists print "No Solution" without quotes.

Example


---

## Samples

### Sample Input 1
```
1
100 -50 15 1 
100
50 12 <= 100
-10 3 <= 5
7 7 >= 2
```

### Sample Output 1
```
381.917
```
