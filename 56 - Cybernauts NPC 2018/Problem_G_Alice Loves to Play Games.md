# Alice Loves to Play Games

**URL:** https://toph.co/p/alice-loves-to-play-game  

---

Alice loves to play game. Recently, she downloaded a new game from google play store. In this game, a robot transports some bricks from one location to another location and collects some points for each transportation. The details of this game are given below:

There are

N

locations in a row which are numbered from 1 to N. Robot will start from location 1, then it will go to location 2, then location 3 and thus it will continue to go next location until it reaches location N. After reaching the location N, it will turn back. Then it will go to location N-1, then location N-2 and thus it will continue until it reaches location 1. After reaching location 1, the robot will stop moving.

There are

M

numbers of brick. For each brick

i

, you are given three integers

Xi

,

Yi

and

Ci

where

Xi

is the current location of the brick,

Yi

is the destination location of the brick and

Ci

is the amount of points which can be earned if robot transports the brick

i

from

Xi

location to

Yi

location. In each location robot can perform the following tasks:

If the current location is the destination of one or more bricks which the robot is currently carrying, then the robot will unload them.

If the carrying capacity of the robot is not full and current location has some bricks, then the robot can choose any amount of bricks from this location without exceeding the carrying capacity limit. Please remember, the robot may choose no bricks at all.

Once robot picks up a brick, it will not unload it until the destination is reached. There is a special set of bricks

S

. If robot transports all the bricks belonging to special set

S

, then

B

bonus points will be awarded.

Now, Alice wants to know the maximum amount of points that can be earned. Please note, there is only one robot in this game.

Input

Input starts with an integer,

T (T ≤ 30)

denoting the number of test cases. Each test case starts with five integers,

N (2 ≤ N ≤ 100)

,

M (1 ≤ M ≤ 500)

,

K (1 ≤ K ≤ 100)

,

S (0 ≤ S ≤ M)

and

B (0 ≤ B ≤ 100000)

where

N

is the number of locations,

M

is the number of bricks,

K

is the maximum number of bricks robot can carry,

S

is the size of the special set of bricks and

B

is the bonus points. Each of the next

M

lines contain three integers

Xi

,

Yi

and

Ci (1 ≤ Xi , Yi ≤ N, Xi ≠ Yi , 1 ≤ Ci ≤ 100)

, description of the brick

i

. Last line of the test case contains

S

special bricks where

Si (1 ≤ Si ≤ M)

represents the

Sith

brick from

M

bricks. If

S

is zero, then it means there is no special set of bricks.

Output

For each case, print the maximum amount of points that can be earned.

Example


---

## Samples

### Sample Input 1
```
2
3 2 1 0 0
1 2 3
2 1 1
3 3 1 1 21
1 2 11
2 3 10
1 3 1
3
```

### Sample Output 1
```
4
22
```
