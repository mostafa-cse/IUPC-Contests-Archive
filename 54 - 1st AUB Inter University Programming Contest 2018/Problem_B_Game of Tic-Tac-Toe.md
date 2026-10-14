# Game of Tic-Tac-Toe

**URL:** https://toph.co/p/game-of-tic-tac-toe  

---

Alice and Bob is a playing a game of tic-tac-toe, to be precise a variant of tic-tac-toe called Notakto. In a game of Notakto, there will always be a winner.

Notakto is played on 3×3 tic-tac-toe board with both players playing X. A game ends when the board contains three consecutive X, at which point the player to have made the last move loses the game.

Given a configuration of the board, you have to find out the winner. Alice always makes the first move.

Input

You are given an integer

n

(0 < n < 200), number of games.

For each game, you are given a 3×3 grid, each grid cell is empty (denoted by dot), or occupied by a cross (denoted by X).

Output

For each game, print the winner of that game, in the format "Game #x: winner". Here, x is the game number.

Examples


---

## Samples

### Sample Input 1
```
1
.X.
.X.
..X
```

### Sample Output 1
```
Game #1: Bob
```

### Sample Input 2
```
2
.X.
.XX
X.X
...
.XX
...
```

### Sample Output 2
```
Game #1: Bob
Game #2: Alice
```
