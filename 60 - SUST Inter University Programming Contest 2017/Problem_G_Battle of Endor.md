# Battle of Endor

**URL:** https://toph.co/p/battle-of-endor  

---

After myriad battles and death of million rebel soldiers, it is high time to destroy the imperial army, the

Dark Force

. Some brave and patriot rebel spies collected information about the defense mechanism of imperial bases. To destroy all imperial bases one must destroy the defense shield first. After hours of debating and arguing, the rebel alliance decided that Han Solo is the best choice to do this task. Afterall, who else could risk his/her life rather than Han!

Input

Input starts with a positive integer

T (1 ≤ T ≤ 10)

, denoting the number of test cases. Each test case starts with two positive integers

n (1 ≤ n ≤ 104)

and

k (1 ≤ k ≤ n)

, denoting the number of troopers and the minimum distance to activate the power supply devices. Following line will have

n

integers denoting the color of each trooper’s uniform

(1 ≤ ci ≤ n)

. Here,

ci

is the color of the trooper positioned at

i

. Next line will have a positive integer

q (1 ≤ q ≤ 105)

, denoting the number of queries. Each of the next

q

lines will have two positive integer

l

and

r (1 ≤ l ≤ r ≤ n)

, denoting the range.

Output

For each query output the number of strongest groups in a single line.

Example

Notes

Data set is huge

(around 10 MB)

. Please use faster I/O.


---

## Samples

### Sample Input 1
```
2
5 1
1 1 2 2 1
3
1 1
1 2
2 5
7 2
3 1 2 1 2 3 2
5
2 4
3 5
2 5
1 6
2 7
```

### Sample Output 1
```
0
1
1
1
1
2
2
1
```
