# Interesting Game

**URL:** https://toph.co/p/interesting-game  

---

Alice and Bob are once again playing Nim. There are

$n$

piles of stones, and

$i^{th}$

pile has

$a_i$

​ stones. Alice and Bob take turns, and on each turn, a player must remove a positive number of stones from exactly one pile. The player who cannot make a move because there are no stones left in any pile loses.

But the game is too boring for Bob. To make it more challenging, he decided that he will only make moves on the largest pile during his turn. If there are multiple largest pile during his turn, he can choose any of them. Bob plays optimally under this restriction, choosing to remove stones only from the current largest pile.

At the start of each game, you'll be informed who will play first. Can you find who will win if both players play optimally?

Input

The first line of input contains the number of test cases

$1\le T\le 10^5$

Each test case starts with a line with a number

$1\le n\le 10^5$

Next line contain

$n$

number

$1\le a_i\le 10^9$

Then a line contain either “ALICE” or “BOB”, the player who will go first.

Sum of

$n$

over all test cases is less than

$10^5$

.

Output

For each test case print who will win in a single line “ALICE” or “BOB”

Example


---

## Samples

### Sample Input 1
```
2
5
1 2 3 4 5
ALICE
2
10 10
ALICE
```

### Sample Output 1
```
ALICE
BOB
```
