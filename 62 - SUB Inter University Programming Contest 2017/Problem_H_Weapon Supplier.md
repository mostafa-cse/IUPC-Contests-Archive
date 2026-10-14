# Weapon Supplier

**URL:** https://toph.co/p/weapon-supplier  

---

Zorro is the chief in charge of central space station. He supplies weapons to all other space station from the central space station. Space stations are numbered from 1 to N. Number 1 is central space station. He can produce N different weapons everyday. ith weapon is used for the protection of ith space station, no other space station can’t use it. Price of ith (1 < i ≤ N) weapon is Pi. Weapon 1 has no price, since it is used for central space station. Though he has no making charge for each weapon, but he can’t make more than N weapon everyday.

All space stations are tetrahedral shaped consists of four corner vertices. The four corners of each station always define a tetrahedron of nonzero volume, and the two stations are always disjoint. A tetrahedron is a polyhedron composed of four triangular faces, six straight edges, and four vertex corners. The distance between the two space stations is always greater than zero.

He has an interesting space ship A-990, which is used to supply weapon from central space station to other space stations. When A-990 flies from one station to another station, it always use the closest distance between the surface of two stations. Its route is always a straight line when it flies. It can go through anything, even through the space station! If that station stays in his path. If A-990 go through a space station, there is neither waste of time nor any harm for both of them( A-990 and that particular station). The maximum velocity of A-990 is 1 km/s. There is a technical fault in A-990 controlling system. A-990 takes always integer time to travel each journey by ceiling the traveling time to the nearest integer number. Let distance between ith station to jth station is 7.01 km. A-990 will take 8 seconds instead of 7.01 seconds for going ith station to jth station or vice versa. The fuel consumed by A-990 depends on the travelling time of the trip, not on the distance traveled. A-990 can’t take more than one weapon at a time. Therefore, after supplying a weapon he has to go back to central station for another weapon. No time is required for loading weapon into A-990 or unloading weapon from A-990. No time is required by A-990 to move on the surface of any space station.

Everyday Zorro needs to supply weapons to the all space stations except central station. He starts supplying weapons from 10:00 AM by A-990. He can’t start supplying weapons before 10:00 AM. There is not any particular order to supply weapon among space stations. Since he has only one A-990 space ship. He has to supply weapon one by one. He can choose any order for supplying weapons. All stations want their supplies on 10:00 AM. Since time is money, there is a penalty for delay supply. Chief in charge of ith station decrease the price of weapon by Di for each second of delay after 10:00 AM. If Zorro supplies ith weapon after t seconds of 10:00 AM he will get Pi - t * Di as a price of weapon from the chief of ith station.

Zorro has fuel of Q seconds. So he can’t run A-990 more than Q seconds for supplying weapon. After Q seconds A-990 must need to stay on central station as if he can start journey for the next day. Zorro can’t full fill all of his supply always. He only supply a weapon if he can get a positive price and he can return to central station. He want to maximize his profit. Help him to do that.

Input

The input contains several test cases. The first line of the input contains an integer T ( T≤ 30) indicating the number of test cases followed by a blank line.

Each set of input of the T test cases consists of several lines.

First line in each set contains two integer N (2 ≤ N ≤ 25), Q (1 ≤Q ≤ 5000) described above.

Second line contains N - 1 integer describing the prices of weapons. ith integer denotes the value of Pi+1 described weapon price for (i+1)th space station (1 ≤ Pi ≤ 100000).

Third line contains N - 1 integer describing the delay penalty of space stations. ith integer denotes the value of Di+1 described the delay penalty on price by the (i+1)th space station (1≤ Di ≤ Pi).

Following 4N lines describes N space stations. First four lines among 4N lines describe four vertices of 1st space station, second four lines describe four vertices of 2nd space station and so on (ith four lines describe ith station). Each vertex description is a line containing three integers X, Y, Z indicating the coordinate of the vertex in space (−103 ≤ X, Y, Z ≤ 103). Consecutive test cases are separated by a blank line.

Output

For each case of input you have to print the case number followed by maximum price Zorro can get after supplying weapons optimally.

Example


---

## Samples

### Sample Input 1
```
2

3 48
100 200
2 3
0 0 0
10 0 0
0 10 0
0 0 10
10 10 5
30 25 2
30 27 2
30 30 8
-10 -10 5
-30 -25 2
-30 -27 2
-30 -30 8

3 637
16739 14773
5 7
100 10 15
100 0 0
100 1 3
90 -1 -2
-60 -60 -80
-60 -55 -3
-90 -23 11
-70 -77 -5
-60 23 80
-60 53 -3
-90 29 11
-70 71 -5
```

### Sample Output 1
```
Case 1: 183
Case 2: 15939
```
