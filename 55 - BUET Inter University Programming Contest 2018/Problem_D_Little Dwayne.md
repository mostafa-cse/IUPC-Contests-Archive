# Little Dwayne

**URL:** https://toph.co/p/little-dwayne  

---

Little Dwayne Johnson is hosting a programming contest. A lot of teams mail him everyday to ask about various things. Little Dwayne uses Kmail to send reply mails. But Kmail only allows sending

$K$

mails per day. If some teams don't get any reply they become dissatisfied.

Little Dwayne forgets everything after each day. So if a team mailed him on

$i$

-th day, he will not reply them after

$i$

-th day. Now little Dwayne wonders what is the total number of dissatisfied teams. Help him or he'll start to cry.

Input

First line contains the number of test cases

$T$

(

$1 ≤ T ≤ 100$

). Each test case starts with two integers

$D$

and

$K$

(

$1 ≤ D ≤ 100$

,

$0 ≤ K ≤ 100$

), where

$D$

is the number of days to consider and

$K$

is the maximum number of mails little Dwayne can send per day. Next line contains

$D$

integers where

$i$

-th integer,

$a_i$

(

$0 ≤ a_i ≤ 100$

) denotes the number of mails little Dwayne received on

$i$

-th day.

Output

For each test case print the number of dissatisfied teams.

Example

Notes

In the sample, little Dwayne can send reply to at most 10 teams on first day. So 2 teams are dissatisfied. On second day no teams are dissatisfied. On third day 4 teams are dissatisfied. So total 6 teams are dissatisfied.


---

## Samples

### Sample Input 1
```
1
3 10
12 5 14
```

### Sample Output 1
```
6
```
