# Stephen, Bob, and Tomato's Canvas

**URL:** https://toph.co/p/stephen-bob-and-tomato-s-canvas  

---

If Stephen Hawking was right, then there is a universe where Bob Ross is a student of Tomato Yoshi. Bob Ross knows how to paint, but he is not good at writing code. Tomato Yoshi being his sensei gives him a programming challenge every week. And, this week is no different.

Tell me young one, what is it that you like more? Solving problems? Or using your segment tree template? — Tomato Yoshi

The challenge is to take an empty canvas, and perform a number of drawing operations on it. And, at the end print the canvas as a grid of characters. Sounds simple enough, right? Well, it is.

You will be given the size of the canvas as the number of rows and columns. The canvas will have R×C cells, where R is the number of rows and C is the number of columns. The cell at the bottom-left corner of the canvas is denoted as

$(0, 0)$

and the cell at the top-right corner is denoted as

$(C-1, R-1)$

.

You can perform one of the following three operations on the canvas:

Operation

Description

$\texttt{L x0 y0 x1 y1}$

Draw a line from

$(x0, y0)$

to

$(x1, y1)$

. The line will always be either vertical, horizontal or diagonal at 45deg. This operation can overwrite previously filled cells.

$\texttt{R x0 y0 x1 y1}$

Draw a rectangle such as at the two farthest corners of the rectangles are

$(x0, y0)$

and

$(x1, y1)$

. This operation can overwrite previously filled cells.

$\texttt{F c x y}$

Fill the space around the cell

$(x, y)$

with the color

$c$

. A space in the canvas is bounded by lines, edges of rectangles, or the edge of the canvas. This operation can overwrite previously filled cells, but not cells that are part of a line or a rectangle's edges.

Use asterisks (

$\texttt{*}$

) to draw lines and rectangles.

Cells are adjacent only when they are above, below, to the left, or the right of one another. Diagonal cells are not to be considered adjacent.

Input

The first line will contain two integers

$R$

and

$C$

(

$0 < R, C \le 1000$

), the number of rows and columns.

The next line will contain

$N$

(

$0 < N \le 1000$

), the number of operations that you will have to perform on the canvas. And, the next

$N$

lines will contain the specification of the operations.

Please refer to the table in the description above for the format of the operations. There will be at most 50

$\texttt{L}$

and

$\texttt{R}$

operations.

There will not be any fill operations in the input that starts on a cell that is part of a line or rectangle's edges.

Output

Print the canvas as a grid of characters. The coordinate

$(0, 0)$

should be at the bottom-left corner of the grid.

Examples


---

## Samples

### Sample Input 1
```
10 10
4
L 2 2 4 4
R 2 2 5 6
F r 3 4
F g 1 1
```

### Sample Output 1
```
gggggggggg
gggggggggg
gggggggggg
gg****gggg
gg*rr*gggg
gg*r**gggg
gg**.*gggg
gg****gggg
gggggggggg
gggggggggg
```

### Sample Input 2
```
10 10
9
L 0 0 9 9
R 6 1 8 6
L 2 2 2 7
L 2 6 8 6
L 0 3 9 3
F g 3 2
F r 0 2
F b 9 8
F w 4 2
```

### Sample Output 2
```
.........*
........*b
..*....*bb
..*******b
..*..**.*b
..*.*.*.*b
**********
rr*www*.*w
r*wwww***w
*wwwwwwwww
```
