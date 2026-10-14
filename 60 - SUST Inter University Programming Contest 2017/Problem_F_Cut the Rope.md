# Cut the Rope

**URL:** https://toph.co/p/cut-the-rope  

---

Fahim is a rope seller. He has a special tool for cutting ropes. But recently this tool is behaving oddly. Everytime he tries to cut some rope, it cuts the rope at a random point from the starting point.

He doesn’t have enough money to repair the machine. As his friend, you need to find the

$k$

-th smallest rope segment after cutting the rope few times with the machine.

Input

There will be several test cases.

The first line of the input contains the integer

$T$

(

$0 < T \le 40$

), the number of test cases.

Every test case starts with a value

$N$

(

$1 < N < 10^{15}$

), the length of the rope. And,

$Q$

(

$1 ≤ Q ≤ 10^5$

).

The next

$Q$

lines each contain a character ('C' or 'F') and an integer

$X$

(

$1 ≤ X ≤ 10^{15}$

). Each line represents a query.

If the line starts with 'C', then the machine cuts the rope at position

$X$

.

If the line starts with 'F' then find the length of the

$X$

-th rope segment, after sorting the ropes by length.

Output

For every test case, print "Case X:" (where X is the case number) as the first line. Then, for every query that starts with 'F' print the length of the desired rope in a single line.

Example


---

## Samples

### Sample Input 1
```
1
10 5
C 4
F 1
F 2
C 9
F 1
```

### Sample Output 1
```
Case 1:
4
6
1
```
