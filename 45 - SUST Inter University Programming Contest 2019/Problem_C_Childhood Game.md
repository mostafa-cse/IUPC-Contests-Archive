# Childhood Game

**URL:** https://toph.co/p/childhood-game  

---

About twenty years ago, when we had only 16MB RAMs and 5GB hard disks, playing games might seem like a difficult thing to do. But luckily we did not require very high end hardware back then to play some amazingly engaging games. One of these games are called, the "Brick Buster".

The idea behind Brick Buster or similar games was like this: You have a bouncing ball and a tray inside of a rectangular grid. The grid is closed on the three sides: left, right and top. The bottom side is empty. When the ball keeps bouncing inside the grid, it hits different walls on the left, right or top. After hitting the walls, the ball just changes it's direction, but keeps moving at it's initial speed. But when it reaches the bottom of the grid, it falls off and the game ends. A tray floats near the bottom of the grid, which a player can move to left or right of the screen. The purpose of the player is to move his tray in such a way, that the ball does not fall off the grid. Additionally, there are some bricks near the top of the board, you have to break those bricks by hitting the bricks with the bouncing balls.

Your are cranking up a new company and want to reproduce this game for portable devices. You thought to yourself, well, this is easy. But soon you figured, it is not. Time is running out, and meeting with your investor is coming near. As a result, you have decided to create an easier version of the game.

In your "easier" game, there are no bricks, no trays, not even an empty side at the bottom of the grid. You have a 500 * 500 board, where the upper-left corner has the coordinate (0,0). There are just some moving balls, that keeps bouncing all over the board. Initially, every ball has a specific position and a fixed velocity. Whenever a ball hits the wall, it just changes its direction by the following rules:

If the ball hits the left or the right wall, then only the direction towards the x axis changes to the opposite.

If the ball hits the top or the bottom wall, then only the direction towards the y axis changes to the opposite.

A collision between two balls takes place when the distance between the two balls is less than or equal to the sum of their radius. When two balls collide, they change their direction by following these rules:

If two balls have been moving in the same direction in terms of x-axis, their movement towards the x-axis will not change after the collision. Otherwise, both of the balls movement towards the x-axis will change to the opposite.

If two balls have been moving in the same direction in terms of y-axis, their movement towards the y-axis will not change after the collision. Otherwise, both of the balls' movement towards the y-axis will change to the opposite.

Now, given some balls and their initial velocity, you have to determine the position of the balls after some certain number of seconds.

You can apply the following assumptions for your calculations:

The game only renders one frame every second. The transition from one frame to the next is discrete and the information between two consecutive frames are lost.

If more than two balls get collided with each other at the end of a second, then the collisions must be processed sequentially in the lexicographical order of the balls. If three balls B1, B3 and B5 collide together at the end of a second, then the collisions must be processed in this order: (B1,B3), (B1,B5), (B3,B5). Here, 1, 3 and 5 are the indexes of the balls in their input sequence.

If a ball is in collision with the other balls and walls at the same time, then the collision with the balls will be calculated first.

Every ball starts moving at the 0-th second. After the end of a second, collisions will be calculated.

If a ball touches or exceeds the boundary of a wall at the end of a second, then the ball can be said to be collided with the wall.

You can safely assume that initially no ball is in collision with other balls or the wall.

Input

Input starts with

$B$

(

$1 ≤ B ≤ 50$

), the number of balls. Then follow

$B$

lines, each having two integers

$X$

and

$Y$

(

$6 ≤ X, Y ≤ 494$

), the initial position of the center of the balls. No balls will be at the same place in the beginning. For simplicity, assume that each of the balls is a circle with a radius of 5. Then follow another

$B$

lines, each with two numbers

$V_x$

and

$V_y$

(

$|V_x|=1$

,

$|V_y|=1$

), the original velocity towards the

$x$

axis and the

$y$

axis for each of the ball.

In the last line of input, you will be given an integer

$T$

(

$T≤10000$

), the number of seconds from the start of the game, where you need to report the position of the balls.

Output

For each case, output

$B$

lines, one for each ball. In each line, you will have two real numbers

$X_i$

and

$Y_i$

, the position of the

$i$

-th ball (according to the input sequence) after

$T$

seconds. Your answer needs to be accurate for 2 decimal places.

Example


---

## Samples

### Sample Input 1
```
1
10 20
1 1
1
```

### Sample Output 1
```
11.000000 21.000000
```
