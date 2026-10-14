# Fuel Finance

**URL:** https://toph.co/p/fuel-finance  

---

X Game Studio is working on their next super-hit game. The game is quite simple. The player has a car and there are

$n$

bridges in front of them. The player has to use their car to cross each bridge once, they can, however, choose in what order to cross the bridges. The

$i$

th bridge has a fuel usage value

$f_i$

and a fuel refill value

$r_i$

. When the player’s car crosses the bridge, the car loses

$f_i$

units of fuel, but at the end of the bridge, the car gets additional

$r_i$

amounts of fuel. Of course, if the fuel ever becomes negative, the car will stop and the player will lose. The player has one chance to initially fill the car’s fuel by some amount. So the player needs to do some calculations to know how much fuel to keep in the beginning and in what order to cross the bridges. If they keep too little fuel, the car will stop on some bridge; if they keep too much, they waste their in-game currency.

The developers found that this was too easy, so they added some more mechanics. The bridges can have some locks at their entrance. In particular, the

$i$

th bridge has a lock with the color

$l_i$

in its entrance. If

$l_i$

is 0, then the bridge has no lock. Also, the

$i$

th bridge has a key with the color

$k_i$

at the end of the bridge. Here,

$k_i$

being 0 means the bridge has no key.

Note that multiple locks might have the same color, but for each color, there is at most one key.

This lock-key mechanic creates more restrictions in the game, as to open a lock, player must have the corresponding key (keys can be used multiple times). Now happy with the rules, the developers have made the levels so that it’s possible to finish the level. But now they need to know the minimum amount of fuel the player needs to fill initially to cross all the bridges as this value can be used to quickly give verdicts instead of making players fumble around with bridges. This is where you come in, The level description is given. You have to find the minimum initial fuel needed to make sure the player can finish the game.

Input

The first line of input will have a positive integer

$T$

, the number of independent test cases. Each test case will begin with a positive number

$n$

, the number of bridges. Then the next

$n$

lines each will have 4 space-separated values denoting

$f_i, r_i, l_i, k_i$

.

$1  \leq T \leq 10^5$

$1 \leq n \leq 10^5$

$1 \leq f_i, r_i \leq 10^5%$

$0  \leq l_i, k_i \leq 10^5$

On a level, no two bridges have the same positive

$k_i$

.

It is guaranteed that there is some sequence of bridges using which the player can finish the level.

The sum of

$n$

over all test cases

$\leq 5 \times 10^5$

Output

For each testcase, output the minimum initial amount of fuel the player needs to fill initially to finish the game in a separate line.

Example


---

## Samples

### Sample Input 1
```
1
4
2 5 0 1
3 3 1 0
4 2 1 2
10 5 2 0
```

### Sample Output 1
```
9
```
