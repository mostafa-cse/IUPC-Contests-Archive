# Stone Hopping

**URL:** https://toph.co/p/stone-hopping  

---

Link has finally defeated the evil calamity Ganon, and peace has once again been restored in the kingdom of hyrule. Link and Zelda are on their way to lake Hylia to enjoy their long sought tranquility. After arriving, Zelda tells Link that she wants to play a game with him. There are many floating stones on the lake. One can easily stand on these stones, however after jumping off a stone, it gets submerged into the water. Zelda says that Link needs to submerge all of the stones.

Link agrees to this game, however he wants to make it a bit more interesting. Link has many fairy friends, and he wants to summon some of them to help him as there are many stones on the lake. The fairies have magical powers and can jump at any distance. However, the area is quite windy, so they won’t be able to jump in any direction as they wish to. We can imagine the entire lake as an

N x M

grid, where each

(x, y)

coordinate might contain a stone. A fairy starts from

(N + 1, M + 1)

and finishes at

(0, 0)

by jumping on a certain number of stones in between. Note that

(0, 0)

and

(N + 1, M + 1)

both are actually part of the ground and not the lake. Due to the wind, they can only jump from one coordinate to another only in a south-western direction, i.e., he can only jump from coordinate

(x1, y1)

to coordinate

(x2, y2)

iff

x1 > x2

and

y1 > y2

.

Even though Link has many fairy friends, he wants to bother as few as possible, which is why he wants to know the minimum number of fairies it would take to submerge all of the stones in the lake. Given the initial state of the lake, can you figure out this number?

Input

The first line contains

T (1 ≤ T ≤ 20)

.

T

test cases follow.

Each test case starts with

N

,

M

and

S

on a single line

(1 ≤ N, M ≤ 300, 1 ≤ S ≤ N * M)

.

Each of the next

S

lines contain two space separated integers

xi

and

yi

(1 ≤ xi ≤ N, 1 ≤ yi ≤ M)

, which denote the

x

and

y

coordinates of the

ith

stone respectively. There can be at most one stone on each coordinate.

Output

For each case, print the case number, followed by the minimum number of fairies it would take to submerge all of the stones. See the sample input/output and explanation for more clarification.

Example

Notes

Explanation

Case 1:

a possible solution is:

(6, 6) -> (4, 4) -> (3, 3) -> (1, 2) -> (0, 0)

(6, 6) -> (3, 2) -> (2, 1) -> (0, 0)

Case 2:

a possible solution is:

(6, 6) -> (4, 4) -> (2, 3) -> (1, 2) -> (0, 0)

(6, 6) -> (3, 3) -> (2, 2) -> (0, 0)

(6, 6) -> (3, 2) -> (2, 1) -> (0, 0)


---

## Samples

### Sample Input 1
```
2
5 5 5
1 2
2 1
3 2
3 3
4 4
5 5 7
1 2
2 1
2 2
2 3
3 2
3 3
4 4
```

### Sample Output 1
```
Case 1: 2
Case 2: 3
```
