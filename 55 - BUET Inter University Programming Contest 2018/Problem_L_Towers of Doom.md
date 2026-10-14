# Towers of Doom

**URL:** https://toph.co/p/towers-of-doom  

---

Alice and Bob are famous for inventing weird games. They just invented a new game called Towers of Doom.

In this game, there are

N

towers and a set of numbers

S

is given. Each tower is built by layers of disks one top of another. The

i

’th tower has

(Hi + 1)

number of disks, numbering from

0

to

Hi

(disk 0 is situated on the bottom, then 1 and so on and disk Hi is on top). The disks are normally indestructible except for the ones whose number is divisible by any number from set

S

. When a disk is destroyed, all of the disks above them fall over and are also destroyed.

Now Alice and Bob are playing the game and taking turns to destroy the disks. In each move, a player must select exactly one destructible disk from any of the tower and destroy it. The player to destroy the last disk wins.

Given the initial configuration of the game, who will win the game if both of them plays optimally. Alice moves first.

Constraints:

T <= 50

1 <= N <= 100

1 <= |S| <= 12

1 <= Hi <= 10^8

1 <= multiplication of all elements of S <= 10^8

Input

First line contains

T

, the number of test cases.

T

test cases follow as described below:

The first line of each test contains

N

and |

S

| (size of set S). Next line contains

N

numbers where

i

'th number is the value of

Hi

. The following line contains |

S

| positive numbers giving all the elements of

S

.

Output

For each test case, print the case number and the name of the player who wins. See sample output for reference.

Example


---

## Samples

### Sample Input 1
```
2
2 1
2 1
1
4 2
4 2 3 7
2 3
```

### Sample Output 1
```
Case 1: Alice
Case 2: Bob
```
