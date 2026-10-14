# Be Efficient!!

**URL:** https://toph.co/p/be-efficient  

---

Little Anita was again thinking about a problem! Recently she was thinking about installing some food carts; as people in Dhaka seems to be only fond of foods, the business might be very profitable. The problem arose when she was thinking about the Home Delivery Service.

You will be given a cost matrix

W

, where

W_ij

represents the traveling time from location

i

towards location

j

. Knowing the cost for installing a food cart at any location

i

, you have to choose a set of locations for installing carts such that, any location is reachable within

K

traveling time (inclusive) from at least one food cart. You also have to minimize the total cost of installing carts.

Input

The first line will contain a single positive integer

T

, denoting the number of test cases.

Of Each test case, the first line will contain two integers

N

, denoting the number of locations and

K

. The second line will contain

N

space separated integers denoting the cost for installing a cart at

i'th

location. Next

N

lines will contain

N

space separated integers each, denoting the matrix

W

.

T <= 100

0 < N <= 22

0 < Cost for installing food cart <= 10^4

0 <= W_ij <= 10^4

0 <= K <= 10^4

Output

Print the indices (starting from 0) of the selected locations. If multiple valid set of locations exists with minimum cost, then print the one which has lexicographically smallest indices.

Example


---

## Samples

### Sample Input 1
```
1
6 16
1 1 1 1 1 1
0 10 20 30 30 20
10 0 25 35 20 10
20 25 0 16 30 20
30 35 16 0 16 25
20 20 30 16 0 14
20 10 20 25 14 0
```

### Sample Output 1
```
Case 1: 1 3
```
