# Level Up

**URL:** https://toph.co/p/level-up  

---

You are playing a game that has 16 levels. You start with level 1 and after gaining a certain amount of experience, you get to next level, however, once you reach 16, you can not level up any further. Now, there are three kinds of ability in the game, let's say A;B and S. You can use each level to upgrade an ability. There is a catch though. You can not level S up until you get to level 6. That is, in order to level up ability S, you need to be of level 6 at least. Also, you can level up S only thrice throughout the whole game. The first time you need to be at least level 6, the second time you need to be at least level 12. And for the last time you need to be level 16, that is you pretty much have to use level 16 to upgrade S. In short, you have to level up ability S exactly thrice maintaining the restrictions above. Apart from those three levels where you upgrade S, you are free to upgrade any ability you like. You can upgrade an ability as many times (possibly 0) as you want.

There are n types of abilities in the game, only one of them works same as the S ability mentioned above. S ability can be upgraded only three times (once at the final level like before). To upgrade S for the first time, you need to be at least level a and to upgrade it the second time you need to be at least level b. You have to find out the number of ways you can level up abilities maintaining the restrictions imposed above.

Input

First line denotes the number of test cases,

$T$

(

$1 \le T \le 1000$

). Then follows

$T$

lines. Each line consists of four positive integers:

$n$

(

$3 \le n \le 2^{63}-1$

),

$a$

,

$b$

, and

$l$

(

$0 < a < b < l \le 2^{63}-1$

).

$n$

is a positive integer greater than

$2$

,

$0 < a < b < l$

where

$l$

is the total number of levels (so final upgrade of S is at level

$l$

).

Output

Output

$T$

lines, each containing the number of ways this can be done. Since the numbers can be huge, output the number modulo

$10^9 + 7$

(a prime number).

Example


---

## Samples

### Sample Input 1
```
4
3 1 2 3
3 2 4 6
10 2 4 6
1000000000 1 2 3
```

### Sample Output 1
```
Case 1: 1
Case 2: 40
Case 3: 3645
Case 4: 1
```
