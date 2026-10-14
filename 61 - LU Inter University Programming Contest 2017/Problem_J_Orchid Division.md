# Orchid Division

**URL:** https://toph.co/p/orchid-division  

---

Quido has a square orchard full of various fruit and nut trees. The trees are planted in regular rows and columns forming a rectangular grid. There are as many rows as there are columns. To be able to maintain the orchard more easily Quido wants to divide the orchard into four rectangular parts. First, he will divide the orchard into northern and southern part by one straight path running from east to west between two rows of the trees. Next, he will divide the northern part by one straight path running from the north perpendicularly to the east-west path. The southern part will be divided similarly by a straight path running from south perpendicularly to the east-west path. These two additional path need not to meet at the same point. The resulting situation might look like the one in the picture bellow.

Quido has assigned a quality index to each tree, the index may be positive or negative or zero. The quality of each of four parts of the orchard will be the sum of qualities of all trees in that part. Quido wants the resulting parts to be of similar quality, in fact, he wants the qualities of the four parts be as close to each other as possible. Therefore, he must choose the positions of the three dividing paths according to this demand.

An example of orchard divided according to Quido's demands. Values represent the qualities of the trees. The qualities of the four parts are (clockwise from north-west) 10, 8, 13, 11. The maximum difference of qualities of any two parts in this division is 5.

You are given the quality of each tree in the orchard. The task is to divide the the orchard in the way described above so that the difference between the quality of the part of the highest quality and the part of the lowest quality is minimized.

Input

The input contains more text lines describing the orchard. The first line contains single integer

$N$

specifying the size of the orchard. There are

$N × N$

trees in the orchard. Each of next

$N$

lines specifies one row of trees in the orchard. The line contains

$N$

integers separated by one or more spaces. Each integer represents a quality of one tree. The order of lines and the order of values on the lines reflect exactly the order of the trees in the orchard. All tree qualities are integers from the interval

$⟨−10^6, 10^6⟩$

. The value of

$N$

will not exceed 3025.

Output

The output contains one integer representing the minimum possible difference between the quality of the part of the highest quality and the part of the lowest quality among all possible divisions of the orchard in the Quido's plan. The output value is supposed to be non-negative and it will not exceed

$10^8$

.

Examples


---

## Samples

### Sample Input 1
```
5
3   0   2  -8  -8
5   3   2   2   3
2   5   2   1   4
3   4  -1   4   2
-3   6   2   4   3
```

### Sample Output 1
```
5
```

### Sample Input 2
```
6
1  2  3   4   5   6
2  4  6   8  10   8
3  6  9  12   9   6
4  8 12   8   4   0
5 10  5   0  -5 -10
6  0 -6 -12 -18 -24
```

### Sample Output 2
```
16
```

### Sample Input 3
```
8
100 -1 -2 -3 -4 -5 -6 -7
-1 -1 -1 -1 -1 -1 -1 -1
-1 -1 -1 -1 -1 -1 -1 -1
-1 -1 -1 -1 -1 -1 -1 -1
-1 -1 -1 -1 -1 -1 -1 -1
-1 -1 -1 -1 -1 -1 -1 -1
-1 -1 -1 -1 -1 -1 -1 -1
30 -1 -1 -1 -1 -1 -1 -30
```

### Sample Output 3
```
67
```
