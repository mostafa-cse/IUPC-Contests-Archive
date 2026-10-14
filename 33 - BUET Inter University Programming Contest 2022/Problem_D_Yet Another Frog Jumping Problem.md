# Yet Another Frog Jumping Problem

**URL:** https://toph.co/p/yet-another-frog-jumping-problem-2  

---

This is an interactive problem. (If you want to know about interactive problems, click

here

)

There are

$N$

stones. Stones are enumerated from

$1$

to

$N$

. There is an intelligent frog too. Jumping capability of the frog never decreases, but it may change at most

$39$

times. If his jumping capability is

$D$

on a given day, he can go

exactly

to stone

$x+D$

from stone

$x$

in a valid jump, if

$x+D$

is not greater than

$N$

.

Initially, all of the stones are uncolored. The frog wishes to color all of the stones. Every morning, the frog discovers himself in the first uncolored stone (i.e. uncolored stone with smallest index). During that whole day, his jumping capability does not change and he keeps jumping

as long as it can

. Whenever he reaches an uncolored stone, he colors it with color

$D$

if his jumping capability is

$D$

during that day. However, the frog is clever. Whenever he reaches an already colored stone, he does not color it again and keeps moving (Note that he must color initial stone of that day). He stops jumping for that day, only if jumping from his current stone is not valid.

Whenever all of the stones are colored, the frog goes back to play with his friends.

You do not know the number of days to complete the task, you do not even know the jumping capability of the frog each day. You can do

$720$

queries, asking for color of a stone.

Retrieve the number of days to complete the task and color of every stone.

Input

First line contains an integer

$T$

$(1 \le T \le 1000)$

, the number of test cases. For each case, first line contains an integer

$N$

$(1 \le N \le 10^5)$

, the number of stones.

Sum of

$N$

over all test cases does not exceed

$10^6$

.

Output

You can ask at most

$720$

queries for each test case. To ask a query just print an integer,

$i$

$(1 \le i \le N)$

, then read an integer

$C$

$(1 \le C \le 10^9)$

, the color of the stone

$i$

. There will be at most

$40$

distinct colors for each test case.

When you can determine the color of all stones print

$0$

(which is not counted as a query). In the next line,

print the number of days

the frog needed to color all stones. In the next line print

$N$

integers,

separated by spaces

,

$C_1, C_2,\cdots,C_N$

where

$C_i$

is the color of stone

$i$

.

After that

read an integer,

$res$

. If

$res$

is

$-1$

, then it means your output is wrong for that test case and you should terminate the program immediately and you will receive Wrong Answer verdict. If

$res$

is not

$-1$

, then process the next test case. If at any moment the number of query asked is greater than

$720$

or an invalid query is asked, then you will receive an integer

$-1$

and you should terminate the program immediately and you will receive Wrong Answer verdict.

Imagine a valid example, where

$T=1$

,

$N=5$

and colors of the stones are

$[2,3,2,3,2]$

.

Interaction may happen as

$—$

,

$>1$

$>5$

$<1$

$>2$

$<4$

$>3$

$<0$

$<3$

$<$

$2$

$3$

$2$

$3$

$2$

$>1$

It takes the frog

$3$

days to complete.

$>$

indicates what your program reads and

$<$

indicates what your program writes. These symbols are here to make it easy to understand. You do not have to print such symbols from your program.


---
