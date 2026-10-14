# Fashion Show

**URL:** https://toph.co/p/fashion-show  

---

The CSE Fest of XYZ University of Engineering and Technology is drawing near!

As one of the events of the cultural programs of the festival, it has been decided to include a fashion show, with

N

participants. However, the way the fashion show has been decided to be conducted is very strange.

The stage where the fashion show will occur is considered to be divided into several lanes.

At first, the participants will be assembled in the first lane.

At each second, the shortest person from any one of the non-empty lanes will move to any other lane, provided that the destination lane is either empty, or the person is shorter than all the persons currently placed in that lane.

The fashion show will conclude once all the persons find themselves in the last lane.

Please note that the heights of all the participants are distinct.

Input

There will be

T

testcases. (

1 <= T <= 20

)

For each test case, there will be a single line containing two integers: the number of participants,

N

and the number of lanes,

M

. Here,

1 <= N <= 64

,

4 <= M <= 65

.

Output

For each test case, output X, the minimum number of seconds required to complete the fashion show. In the following X lines, you have to describe how exactly the participants will move to complete the fashion show in X seconds.

For each of the X lines, output 3 space-separated integers a, b, c

(1 <= a <= N, 1 <= b, c <= M)

, which indicates that the a-th participant moves from lane b to lane c. Here, a-th participant refers to the a-th shortest participant among all the participants of the fashion show. See sample input/output for better understanding.

Your output will be judged based on the correctness of the outputted minimum number of seconds required to complete the show, and whether the subsequently outputted moves are valid according to the definitions and parameters of the problem and result in all of the participants being positioned at the final lane after the execution of the X-th move.

Example


---

## Samples

### Sample Input 1
```
1
10 10
```

### Sample Output 1
```
21
1 1 2
2 1 3
3 1 4
4 1 5
5 1 6
6 1 7
7 1 8
8 1 10
9 1 9
8 10 9
10 1 10
8 9 1
9 9 10
8 1 10
7 8 10
6 7 10
5 6 10
4 5 10
3 4 10
2 3 10
1 2 10
```
