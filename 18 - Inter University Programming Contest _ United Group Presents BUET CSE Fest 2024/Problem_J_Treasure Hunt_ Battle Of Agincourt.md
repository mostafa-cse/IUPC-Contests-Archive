# Treasure Hunt: Battle Of Agincourt

**URL:** https://toph.co/p/treasure-hunt-battle-of-agincourt  

---

Once upon a time, during the tumultuous years of the Hundred Years' War, a pivotal event known as the Battle of Agincourt took place. This battle was fought between the English army, led by King Henry V, and the French knights. Against overwhelming odds, the English emerged victorious, thanks in part to their clever use of longbows and their determination.

After the battle, the English soldiers found themselves in chaotic battlefield, where the French forces had fled, leaving behind their possessions. The area resembled a maze, filled with tents, supplies, and hidden treasures that the French had once guarded. This maze-like structure was dotted with remaining of the battle and opportunities for the English soldiers to collect what they could find.

Among these soldiers was a brave individual who was not only a skilled warrior but also had a keen eye for treasure. He was particularly fascinated by the tales of the riches left behind by the French knights. Legend had it that scattered throughout the battlefield were unique treasures that represented the wealth and power the French had once held.

With a heart full of determination, the soldier set out on a quest to explore this maze of the battlefield. The layout was like a vast grid, where each cell represented a different location filled with potential rewards, such as weapons, armor, and supplies. Each cell

$(i,j)$

had a specific treasure value

$a_{i,j}$

​ that symbolized the riches and stories left behind by the fallen knights.

Eager to uncover these treasures, the soldier navigated through the pathways of the battlefield, excited about the adventures that awaited him. Each step taken in this chaotic environment was not just about collecting loot but about embracing the stories and lessons from the battle that would stay with him forever.

Starting from the top-left corner of the grid

$(1, 1)$

, the soldier could only move down or right. As he collected treasures from the cells along his journey, he aimed to

maximize

his total profit. He understood that the treasures he gathered were not merely material wealth but a reflection of the hard-fought victory and the history that surrounded him.

The total profit the soldier aimed to achieve was calculated using the following formula:

$Total\ Profit = \left( a_{C_1} + a_{C_2} + \ldots + a_{C_k} \right) - \left( |C_2 - C_1| + |C_3 - C_2| + \ldots + |C_k - C_{k-1}| \right)$

Here,

$C_1, C_2, C_3, ….., C_k$

represented the cells he took treasure from, and

$|C_i - C_j|$

denoted the Manhattan distance between the cells.

The soldier’s mission was clear: to traverse the maze-like battlefield, gathering treasures while reflecting on the lessons learned from the great battle of Agincourt, which was

maximizing

the profit.

Input

First line of the input contains an integer

$T$

, the number of test cases.

The first line of each test case contains two space separated integers

$N$

and

$M$

which represents dimensions of the grid.

Each of the next

$N$

lines contain

$M$

space separated values, where

$a_{i, j}$

represents the treasure value at the cell in

$i$

-th row and

$j$

-th column.

Constraints

$1 \le T \le 1000$

$1 \le N \le 1000$

$1 \le M \le 1000$

$0 \le a_{ij} \le 10^9$

Sum of

$N * M$

of all test cases will not exceed

$10^6$

.

Output

For each test case output a single integer the maximum profit he can earn.

Example


---

## Samples

### Sample Input 1
```
5
4 3
8 4 4
1 1 5
7 9 9
5 5 6
2 4
5 9 7 8
1 2 9 5
1 3
1 9 4
5 1
0
9
9
4
4
3 5
1 4 8 8 4
8 3 0 8 7
2 0 0 8 8
```

### Sample Output 1
```
35
31
12
23
39
```
