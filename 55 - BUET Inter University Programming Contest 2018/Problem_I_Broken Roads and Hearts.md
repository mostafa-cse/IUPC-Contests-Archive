# Broken Roads and Hearts

**URL:** https://toph.co/p/broken-roads-and-hearts  

---

Have you heard of the sad story of the place of Banasree? People cannot travel because of the terrible road condition. Students cannot go to their school in time, workers cannot reach their workplaces in time and even lovers cannot meet each other in time which is leading to so many breakups. The entire area is a complete mess which the authority is well aware of. Thus in order to reduce the difficulties that the people of Banasree are facing they have planned up some experiments to conduct on the several roads in the area.

There are

$N$

buildings in Banasree, ranging from residence to police headquarters, each of the buildings have a unique identifier from 1 to

$N$

. Which building is which is not important to us, but it is important to know that there are bidirectional roads which spans from the gate of one building to another. The authority was also intelligent enough to make the road network such that it is possible to travel from any building to any another by means of using some series of roads, and also that the roads do not intersect. Also there is exactly

$N-1$

roads, that is the number of roads is one less than the number of buildings.

Initially, before the authority ran any experiments they noted the current traveling time of each road, where traveling time is the average time to travel the entire road once. The authority will now perform Q experiments, and there are two types of them:

Type 1:

A road with number

$R$

(which is numbered by the input order) is selected and have its traveling time permanently changed to value

$V$

until other experiments change this value. It is not necessary that the new traveling time is less than the previous one.

Type 2:

Two buildings with identifier

$X$

and

$Y$

are selected and the minimum average time taken to travel between the two buildings are measured.

The experiments will be listed to you in chronological order. For every experiment of Type 2 print the value measured.

Input

The first line of the input contains one integer

$N$

(

$2 \le N \le 10^5$

), the number of the buildings in Banasree. Each of the next

$N-1$

lines contain three integers each

$X$

and

$Y$

(

$1 \le X, Y \le N$

) and

$V$

(

$1 \le V \le 10^9$

), denoting that there is a road with initial traveling time V spanning from the building with identifier

$X$

to the building of identifier

$Y$

. Remember that for experiment of Type 1 the selected road will be identified with it’s order in these

$N-1$

lines.

The next line contains a single integer

$Q$

(

$1 \le Q \le 10^5$

), the number of experiments conducted. The following

$Q$

line contains three integers each,

$T$

(

$T= \{1, 2\}$

),

$A$

and

$B$

,denoting that the experiment is of Type T, and if

$T$

is 1 then

$A$

and

$B$

denotes

$R$

(

$1 \le R \le N-1$

) and

$V$

(

$1 \le V \le 10^9$

), and if

$T$

is 2 they denote

$X$

and

$Y$

(

$1 \le X, Y \le N$

).

The given input guarantees that it is possible to travel from any building to another, and that the experiments are given in chronological order.

Output

For each experiment of Type 2, print the values that will be measured.

Example


---

## Samples

### Sample Input 1
```
10
2 6 9
6 10 4
10 7 2
10 3 1
3 1 8
10 9 9
1 4 1
6 5 6
4 8 4
10
1 5 10
2 7 6
1 4 4
2 9 5
1 5 7
1 5 1
2 4 3
1 5 8
2 4 3
2 8 8
```

### Sample Output 1
```
6
19
2
9
0
```
