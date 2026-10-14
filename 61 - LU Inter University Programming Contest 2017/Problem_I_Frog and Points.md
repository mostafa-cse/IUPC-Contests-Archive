# Frog and Points

**URL:** https://toph.co/p/frog-and-points  

---

There are N stones on across the diameter of a perfectly circle shaped pond at equal distance. The 1st stone is on one side of the pond and Nth stone being on the other side. A frog will cross the pond by jumping over the stones. However, his jump length will be constant. If a frog is in the

a

th stone, then a jump length of

L

will get him to

(a+L

)th stone. There are integer points in each stone. Points can be negative or positive. Positive points will be added to the frog’s score and negative point will be deducted from the frog’s score. What is the maximum number of points the frog can collect by crossing the Path once? He can go to a stone

b

from

a

if

b>a

; However due to the wave of the water at the pond, points of a particular stone can be changed. if his jump length is

L

the frog will land on the

L

th stone in his first jump. When he will reach the

N

th or jump pass the

N

th stone the game ends. He will get to the other side.

Input

First line of the input will be a number

T

that represents the number of Cases.

1<=T<=5

. Then there will be

T

cases. In the first line of input there will be an integer number

N

, the number of stones.

1<=N<=105

. Then in the next line there will be

N

integer numbers

xi

, where

|xi | <=106

,

i

th number will represent the number of coins in the

i

th stone. Then next there will be a number

Q

,the number of queries..

1<=Q<=105

. In next

Q

lines there will be a number

A

. If

A=1

then print then maximum number of stones the frog can collect. If

A=2

, it will be followed by

2

numbers

B,C

. It means then number of coins of the

B

th stone is changed to

C

.

|X|

it means modulus of

X

.

1<=B<=N

and

|C|<=109

.

Output

For each case print “

Case

“then the case number and then “

:

“. Then print a newline. Then print the desired answer of each query type

1

(when

A

is equal to 1) in a line.

Example


---

## Samples

### Sample Input 1
```
1
5
1 2 3 4 5
1
1
```

### Sample Output 1
```
Case 1:
15
```
