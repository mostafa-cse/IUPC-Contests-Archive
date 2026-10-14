# Play the Lottery

**URL:** https://toph.co/p/play-the-lottery  

---

The statement of this problem is going to be short and sweet because the setter was busy with life and didn't get a lot of time to prepare it. You have gone to a fair in some shady part of USA and all of a sudden you find a tent conspicuously placed in the center of the fair. You go inside the tent and you find M boxes placed side by side with balls of different number written on them. The boxes are not transparent so you can't see the number on the balls of course.

The owner of the tent invites to play the game. "Luck is overrated. Play the game and win prizes!", he cries out. He explains to you that you will choose a number

$N$

at the start of the game and then select one ball from each box randomly and at the end if the sum of numbers on the balls that you collected is equal to the number N you win! You decide to watch the game for a while before playing to know a bit about what kind of balls are in each box. After watching for hours you have made a list of observations that you made about each box. For each box you have discovered the number of balls it has of each number. Given this information can you calculate the number of ways to make different values of N?

Input

The first line of input contains

$M$

(

$1 ≤ M ≤ 10^5$

) - the number of boxes. The next

$M$

lines contain the information of each box. The first number of these lines contain

$X$

(

$0 < X < 10^5$

) denoting the number of types of balls in it. The next

$X$

pairs contain information of the balls. The first number of each pair is the number written on this type of ball and the second one is the amount,

$ci$

(

$0 < ci < 10^3$

) of this type of ball in the box. You may assume that for a single box, all the types will be unique (that is two different types of balls won’t have the same number written on them). Also the total sum possible with the highest numbered balls from each box won’t be greater than

$10^5$

.

Output

For each possible sum that can be made with the balls, print the sum and the number of ways it can be made in each line. Output should be sorted by increasing value of sum. Do not print the sum that cannot be made or the number of ways they can be made is 0 after modulo by 786433. Print the number of ways modulo 786433.

Example


---

## Samples

### Sample Input 1
```
2
2 2 2 1 1
2 3 3 1 1
```

### Sample Output 1
```
2 1
3 2
4 3
5 6
```
