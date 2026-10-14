# Explosion

**URL:** https://toph.co/p/explosion  

---

There is a house named Larcana. It is a very weird house. There are exactly N rooms in total and between any two adjacent rooms there is a door. You can reach any room from any other rooms by using one or more doors.

Now Trump and Putin are in two distinct rooms in this house. They are moving randomly in this house. In each second each of them chooses a door of his room randomly and uses it to go to an adjacent room.

If at any time. both of them are in the same room, a explosion occurs. So before Putin and Trump start to move, Gabbar chooses a room randomly where none of them are in and destroys it to prevent the explosion.

You can assume the doors are built in such a way that they do not meet halfway changing rooms. For example, let room 1 and room 2 be adjacent. Then there is a door between them. If Trump is in room 1 and Putin is in room 2 then they can immediately switch room without meeting each other. After switching, Trump will end up in room 2 and Putin will end up in room 1. Since they did not meet in any particular room no explosion will occur.

Now find the probability that no explosion occurs.

Input

In first line there will be a single integer

$T$

(

$1 \le T \le 100$

) denotes the number of test cases. For each test cases, in the first line three integers

$N$

(

$3  \le N \le 10000$

),

$R$

,

$P$

(

$1 \le P, R \le N, P \ne R$

) will be given which denotes the number of rooms in this house, the room number of Trump and the room number of Putin respectively. Then n-1 lines follow, pair of integers

$u$

and

$v$

(

$1 \le u,v \le N$

) denotes that room

$u$

and room

$v$

is adjacent and there is a door between them.

Output

For each test cases, print two integers

$X$

and

$Y$

where the probability of no explosion is

$\frac{X}{Y}$

and

$X$

,

$Y$

are co-prime

Example


---

## Samples

### Sample Input 1
```
2
3 1 3
1 2
2 3
4 1 3
1 2
2 3
3 4
```

### Sample Output 1
```
1 1
1 2
```
