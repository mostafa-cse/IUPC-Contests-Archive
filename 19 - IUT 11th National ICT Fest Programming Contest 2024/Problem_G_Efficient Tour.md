# Efficient Tour

**URL:** https://toph.co/p/efficient-tour  

---

Gopher is embarking on yet another adventurous tour, this time across

$N$

cities, each

$uniquely$

defined by its two-dimensional coordinates and having

$distinct$

Power. Gopher will visit all the cities but can only visit each city once. He will start from the city with the lowest Power and return to the starting city after visiting all the cities.

But, as with any journey, there are rules to abide by:

Before reaching the city with the highest Power, Gopher can go from city

$i$

to city

$j$

only if the Power of city

$i$

is lower than that of city

$j$

$(Power_i < Power_j)$

.

Once he reaches the city with the highest Power, Gopher's path can go from city

$i$

to city

$j$

if the Power of city

$i$

is higher than that of city

$j$

$(Power_i > Power_j)$

.

The cost of moving from city

$i$

to city

$j$

is calculated using the formula

$\sqrt{(x_i - x_j)^2  + (y_i - y_j)^2}$

, where

$(x_i, y_i)$

represents the coordinates of city

$i$

and

$(x_j, y_j)$

represents the coordinates of city

$j$

.

Gopher could complete his tour through various routes, he wants to accomplish it with the minimum cost. Thus, he turns to you for assistance in this.

Input

The first line will contain one integer

$N(2\leq N \leq 3\times{10}^3)$

denoting the number of cities Gopher will visit in his tour.

Next

$N$

lines will contain three integers

$Power_i(1 \leq Power_i\leq N)$

,

$x_i,y_i(1 \leq x_i,y_i \leq {10}^6)$

,

$Power_i$

denoting the Power of

$i_{th}$

city and

$x_i,y_i$

denoting the coordinator of

$i_{th}$

city.

Output

Print a single line containing the minimum cost to visit all the cities in the Gophers tour. Errors less than

$10^{-4}$

will be ignored.

Example


---

## Samples

### Sample Input 1
```
4
1 2 3
2 6 3
3 3 7
4 5 2
```

### Sample Output 1
```
14.9225
```
