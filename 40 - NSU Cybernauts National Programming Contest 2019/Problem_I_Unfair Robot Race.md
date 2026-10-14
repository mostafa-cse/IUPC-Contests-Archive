# Unfair Robot Race

**URL:** https://toph.co/p/unfair-robot-race  

---

Two teams of robots,

Team A

and

Team B

, are racing in a 2D grid. There will be a total of 6 rounds. Teams will play any round at random, but each team is guaranteed to play 3 rounds each.

Each team consists of a robot that can go North, South, East or West in a single move, in the given 2D grid. These robots are rectangular in shape and can vary in size for each round for either team. The entire rectangle of the robot on the map will be shown with a group of characters 'A' or 'B'. Note that, the robots will not be able to rotate from their position. They can only move one step at a time.

The scoring system is a simple one. There is a place in the grid, marked as 'S'. A robot (any part of that robot) will have to reach the 'S', with minimum moves. The number of moves is the score for that team in that round. As there are obstacles (marked as '#' and cannot be crossed by any part of the robot) on the way, there is a chance that it is not possible to reach there. In that case, we call that

infinite

moves. As you do not have much time to figure out who wins, you consider any score

more than

500 to be infinite as well.

A team wins a round (say 1st round) if it scores less than the other team (on their corresponding 1st round) or the other team scores an infinite and vice versa. A round will be called a draw, if both teams' scores are the same or both take infinite moves to finish the round. A team wins the race if it wins maximum rounds and it is considered a draw if both the team wins the same number of rounds in the whole race.

Input

First line of the input contains an integer

T

, the number of test cases.

Each test case contains 6 rounds and each round starts with two integers

r

and

c

, followed by r lines containing c characters each describing the 2D grid.

Constraints

1<=T<=1000

3<=r,c<=100

It is guaranteed that there will be one 'S' in the grid and the size of the robot will be less than the grid and at most 9 on either side.

Output

Print the case number and "Team A", "Team B" or "Draw", depending on the result of the race.

On the next 3 lines, print the corresponding scores of Team A and Team B in their 1st, 2nd and 3rd round, separated by a space. If the score is infinite, print

inf

.

Example

Notes

** Dataset is huge. Please use faster I/O.


---

## Samples

### Sample Input 1
```
1
15 24
........................
........................
....................#.S.
......#.................
...........#.......##...
........................
......AAA...............
......AAA...............
......AAA..........#....
........................
......#..........#......
........................
........................
........................
........................
7 5
.....
...S.
.....
..###
.....
..BB.
.....
5 6
.....S
..#...
..#...
..####
....AA
13 24
........................
........S......##.......
....................#...
.#....#.........#.......
...........#.......##...
........................
....AAAAA...............
........................
.........#.........#....
........................
.........#.......#......
..................##....
........................
13 9
.........
........S
.........
.#....#..
.........
.........
....BB...
.........
.........
.........
......#..
.........
.........
3 2
#S
#.
#B
```

### Sample Output 1
```
Case 1: Team B
19 8
12 8
inf 2
```
