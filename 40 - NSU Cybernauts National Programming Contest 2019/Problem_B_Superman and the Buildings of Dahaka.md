# Superman and the Buildings of Dahaka

**URL:** https://toph.co/p/superman-and-the-buildings-of-dahaka  

---

To end the long-running feud between Superman and Goku fans regarding who's stronger, Zeron has decided to step in. He wants to assess these two heroes' capabilities himself first. So, he has invited Superman to the city of Dahaka and gave him a challenge. (He will judge Goku later).

The city of Dahaka has

N

buildings. A building is a rectangular-shaped object that has a height and width. The width of each building is the base that is aligned horizontally with the ground and it is always 1.

Yes, I know, Dahaka is a very weird city, where the buildings are 2D geometrical shapes!

Moreover, the buildings in Dahaka are actually alive and always need to be in touch with their parents. Otherwise they crumble to dust, except for a single building which has no parent (will be termed as the first building from hereon).

Now, Zeron told Superman that he will give him information about all the buildings (height, parent). For each building

X

, Superman has to use his massive strength to create a histogram such that the parent of the

i

th building is the

i-1

th building and the last building of the histogram is

X

while the first building is at the start of the histogram (see sample case explanation for further elaboration). The buildings of a histogram are aligned at a common baseline.

Furthermore, since strength is not everything in a battle, Superman needs to calculate the area of the largest rectangle in each of the histograms. Your task is to do that for him.

Graphically speaking, a histogram is a sequence of some bars/rectangles standing on the same baseline. For this problem, imagine there is no space between two consecutive rectangles i.e. their sides are touching.

A rectangle is considered inside a histogram when the full part of it is on one or more bars of the histogram. For each histogram (made for each building), Superman needs to find the rectangle with the largest area.

In the above figure, the rectangular area in the histogram with the largest area is marked within the red area as an example. No rectangle with a larger area can be drawn inside this histogram.

Input

Input starts with an integer

N

, the number of buildings.

Each of the following

N

lines contains 2 space-separated integers

Hi and Pi

, where

Hi

is the height of the ith building and

Pi

th building is the parent of the ith building. If

Pi

=

i

, it means that the ith building has no parent.

It is guaranteed that only the first building will have no parent and the first building is the ancestor of all other buildings.

Constraints:

1 ≤ N ≤ 500000

1 ≤ Hi ≤ 500000

1 ≤ Pi ≤ N

Output

Print

N

separate lines. The

i

th line should contain an integer, the maximum area that Superman can make for the

i

th building as described in the problem statement.

Example

Notes

Dataset is huge, use faster I/O (like scanf/printf in C or C++).


---

## Samples

### Sample Input 1
```
6
5 1
3 1
10 2
8 1
4 4
11 4
```

### Sample Output 1
```
5
6
10
10
12
16
```
