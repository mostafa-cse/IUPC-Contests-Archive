# Office Para

**URL:** https://toph.co/p/office-para  

---

The streets of Office Para were dark at night because the lamps on the streets weren’t working and the city corporation did not do much to fix the lamps even after several complains. So, people from some of the offices came up with an idea to put lamps on top of their building that will illuminate the streets. The light from the lamps would spread equally in all directions as long as nothing is blocking it. However, since the buildings were tall, some of them would be blocking lights from the lamps on top of some other buildings. This would result in some parts of the streets being dark.

Here, the street is represented by a straight line of length D. By this street, there are buildings of different heights and negligible widths. On top of some buildings, people placed lamps, dimensions of which are also negligible. A certain part of the street is said to be dark if light from no lamp can reach there.

Find the total length of illuminated parts on the street.

Input

First line of input contains the number of test cases T which is less than 25. For each test, first line will give you two integers N (1 <= N <= 3x10^5) and D (1 <= D <= 10^9), the number of buildings and the length of the street respectively. Each of the following N lines will contain a description of a building with P, H and L. Where, P (0 <= P <= D) is an integer describing the position of the city (the left end is 0), H (1 <= H <= 10^9) is an integer describing the height of that building and L is a string which is either “yes” or “no” depending on whether there is a lamp on top of that building or not. Building positions will be presented in a sorting order of distance from the left end and there will be only one building in exact same point.

Output

For each test case, print the length of the illuminated portion of the street. Check sample input and output for details. Precision error lower than 10^-4 will be overlooked by judge.

Example

Notes

Huge input file, use faster IO methods.


---

## Samples

### Sample Input 1
```
2
3 10
2 6 yes
4 3 no
8 2 no
5 15
4 3 no
5 5 yes
6 6 yes
9 2 no
10 3 no
```

### Sample Output 1
```
6.000000
8.500000
```
