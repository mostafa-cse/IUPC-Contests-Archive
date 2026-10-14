# Game of Tic-Tac-Toe, Again

**URL:** https://toph.co/p/game-of-tic-tac-toe-again  

---

Alice and Bob are playing a game of Tic-tac-toe, to be precise a variant of tic-tac-toe called Notakto. In a game of Notakto, there will always be a winner.

Notakto is played across one or several

$3 \times 3$

Tic-tac-toe boards with both players marking the board with

$\texttt{X}$

. Alice always makes the first move. A game ends when all the boards contain three consecutive

$\texttt{X}$

in any direction (horizontal/vertical/diagonal), at which point the player to have made the last move loses the game. If there is 3 consecutive

$\texttt{X}$

in a board already, then no more moves can be made on that particular board.

Given a configuration of the game, you have to find out the winner.

Input

You are given an integer

$t$

(

$1 \le t \le 100$

), the number of games.

For each game, you are given

$n$

(

$1 \le n \le 10^4$

), the number of boards.

For each board, you are given a

$3 \times 3$

grid. Each grid cell is empty (denoted by a dot), or occupied by a cross (denoted by an

$\texttt{X}$

).

Output

For each game, print the winner of that game, in the format

$\texttt{Game \#c: winner}$

. Here,

$c$

is the game number.

Example


---

## Samples

### Sample Input 1
```
4
1
...
...
..X
1
XX.
X.X
.XX
2
XX.
X.X
.XX
XX.
X.X
.XX
3
XX.
X.X
.XX
XX.
X.X
.XX
XX.
X.X
.XX
```

### Sample Output 1
```
Game #1: Alice
Game #2: Bob
Game #3: Alice
Game #4: Bob
```
