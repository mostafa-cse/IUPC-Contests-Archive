# A Simple Game

**URL:** https://toph.co/p/a-simple-game  

---

Saif and Sabi is playing a game in a maze. They will start from 2 different initial points and they will try to go to the destination point in the maze. Whoever is the first at reaching destination will be the winner. They can move up, down, right or left in the maze. At any step of the game, only one player will be allowed to move. Which player wins the toss will move on the first step, then at the second step the second player will move, then at the 3rd step the 1st player will move again, and so on. The rule of the game is, at the nth step any player can move up to n blocks in one of any four directions. That means at the 1st step of the game (not of this player) a player can move one block in up, down, right or left direction. In the second step a player can move one block or two blocks in one of the four directions. And so on. While moving for multiple blocks in a certain turn, the player has to go through all the cells in the path. No one is allowed to go outside of the maze or in a block having obstacle. But both of the players can stay at a single block at a time. Now Saif and Sabi both of them let robots to play the game instead of themselves. Those robots moves to the destination following shortest possible path.

Your task is to write a program to find out the winner of the game, given the maze and the winner of toss. Both player will play optimal way.

Input

Input begins with a single positive integer T (T < 30) on a line by itself indicating the number of the cases following. Each test case will start with 3 integers R (1<= R <= 100), C (1 <= C <= 100) and W(1 or 2, 1 means Saif is the toss winner and 2 means Sabi is the toss winner). R is the number of rows of the maze, C is the number of columns of the maze and W is the toss winner of this game. Below this next R lines will contain the maze. In the maze “.” means free cell and “#” means obstacle. Each maze will have a 1 (initial position of Saif), a 2 (initial position of Sabi) and a D (destination position).

Output

For each test case, the output must contain the case number like sample output and the winner name. If Saif reaches the destination first, print “Saif”, if Sabi reaches the destination, print “Sabi” and if no one can reach the destination print ‘IMPOSSIBLE’. See sample output format for further clarification.

Example


---

## Samples

### Sample Input 1
```
2

3 3 2
1#2
..#
.#D

9 11 1
.......#...
........#..
.......#..#
....D.....#
.........#.
...#.......
....#....2.
.....1..##.
..#........
```

### Sample Output 1
```
Case 1: IMPOSSIBLE
Case 2: Saif
```
