# Make More Money

**URL:** https://toph.co/p/make-more-money  

---

You, the great businessman of TEUB, arrived at ESC land which consists of

$N$

cities numbered from 1 to

$N$

. You are currently at city 1. For each city

$i$

, you arrive at (including your current city) in ESC land, you do some business and make profit

$a_i$

. The profit can be negative which means you have lost

$|a_i|$

amount of money in your business.But there is a special rule for travelling ESC land:

First you can go from your current location i.e. city 1 to city

$i$

through the path

$1, 2, 3, \cdots, i$

(

$1 \le i \le N$

).

Then you can go from city

$i$

to city

$j$

through the path

$i, i-1, i-2, \cdots, j$

(

$1 \le j < i$

).

So, your profit will be

$a_1+a_2+a_3+...+a_i+a_{i-1}+a_{i-2}+\cdots + a_j$

Note that you may stay at city 1 and you may also choose not to go to reverse direction (i.e. direction to which city index decreases).

Find out maximum profit you can achieve.

Input

First line will be number of test cases

$T$

For each test case:

In the first line, the number of cities

$N$

will be given.

Then there will be

$N$

integers

$a_1, a_2, \cdots, a_N$

where

$a_i$

denotes achievable profit from city

$i$

at a time.

Constraints

$1 \le T \le 10$

$1 \le N \le 10^5$

$-10^4 \le a_i \le 10^4$

Over all test cases,

$\sum{N} \le 2*10^5$

Output

For each test case, print one line containing maximum possible profit you can gain.

Example

Notes

Optimal paths for the 4 testcases are:

path:

$1$

, profit:

$4$

path:

$1 \to 2 \to 1$

, profit:

$4 + (-2) + 4 = 6$

path:

$1 \to 2 \to 1$

, profit:

$5 + 2 +5 = 12$

path:

$1 \to 2 \to 3 \to 4 \to 3 \to 2$

, profit:

$(-1)+3+(-2)+4+(-2)+3=5$


---

## Samples

### Sample Input 1
```
4
1
4
2
4 -2
3
5 2 -10
4
-1 3 -2 4
```

### Sample Output 1
```
4
6
12
5
```
