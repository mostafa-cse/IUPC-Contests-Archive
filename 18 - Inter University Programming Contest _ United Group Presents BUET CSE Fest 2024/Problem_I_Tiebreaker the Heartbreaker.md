# Tiebreaker the Heartbreaker

**URL:** https://toph.co/p/tiebreaker-the-heartbreaker  

---

After two hours of a football match between Team X and Team Y, it will be penalties to decide who will win. Team X and Team Y will take shots alternatively, Team X will go first. After 5 penalties each, the team scoring higher number of goals from the penalties will win. However, it may be possible that the match does not require all 10 shots if the winner is certain. You will be provided the results of the previous shots of the penalty shootout, you have to decide whether it is possible to determine the result of the match after this shot. In other words:

If the current shot is scored, the team taking the shot will win

If the current shot is missed, the team taking the shot will lose

No particular outcome of the current shot is enough to determine the winner.

Input

The first line will contain the number of test cases

$1 \le T \le 100$

.

Each of the next

$T$

lines will describe a test case using a binary string of length

$1 \le len \le 9$

indicating the results of the previous shots where the character of position 1 is the result of the penalty shot taken by Team X, the character of position 2 is the result of the penalty shot taken by Team Y, the character of position 3 is the result of the penalty shot taken by Team X, the character of position 4 is the result of the penalty shot taken by Team Y and so on. The character is 0 if the shot is missed, 1 if the shot is scored. It is guaranteed that the winner is not decided yet.

Output

For each test case, output a single integer:

$1$

: If the current shot is scored, the team taking the shot will win

$0$

: If the current shot is missed, the team taking the shot will lose

$-1$

: No particular outcome of the current shot is enough to determine the winner.

Example


---

## Samples

### Sample Input 1
```
3
1100
1101011
1011111
```

### Sample Output 1
```
-1
1
0
```
