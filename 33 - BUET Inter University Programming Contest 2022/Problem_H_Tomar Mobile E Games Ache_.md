# Tomar Mobile E Games Ache?

**URL:** https://toph.co/p/tomar-mobile-e-games-ache  

---

After a long and hectic Eid day you are finally relaxing. But then your 5 year old cousin comes and wants to play games on your phone. Luckily you still have a nokia 1600. You open snake xenzia in the legendary phone, activate a cheat code to make the snake never grow, hand it over to the kid and watch as he plays.

If the snake moves out of screen from the top, it reappears from the bottom in the same column. If the snake moves out of screen from the left, it reappears from the right in the same row. Similar thing occurs for bottom and right. You notice that the snake takes

$16$

moves to repeat its position if allowed to move vertically. The snake takes

$20$

moves to repeat its position if allowed to move horizontally. A move can be defined as movement of the snake in one unit time, upward, downward, to the left or to the right. The goal of the snake is to eat a reward located somewhere on the screen.

Now you wonder, if the whole screen is regarded as a grid of size

$16\times20$

of possible positions for the snake and also for the reward, what is the minimum number of moves required for a snake at cell

$(i_1, j_1)$

to reach a reward at cell

$(i_2, j_2)$

.

Input

The first line contains a single integer

$T (1 \leq T \leq 30)$

— the number of test cases.

Each of the following T lines consist of

$4$

integers

$i_1, j_1, i_2, j_2$

,

$(1 \leq i_1, i_2 \leq 16, 1 \leq j_1, j_2 \leq 20 )$

.

Output

Print the answer of each test case in a new line.

Example


---

## Samples

### Sample Input 1
```
5
1 1 16 20
4 20 16 1
9 9 9 9
1 15 16 15
10 10 15 15
```

### Sample Output 1
```
2
5
0
1
10
```
