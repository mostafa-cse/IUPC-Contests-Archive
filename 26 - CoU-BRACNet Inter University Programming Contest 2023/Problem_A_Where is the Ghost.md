# Where is the Ghost

**URL:** https://toph.co/p/where-is-the-ghost  

---

The ghost exploration team find some

1D

coordinate where the cursed object is located. You will be given

$N$

such cursed positions. All the locations are integers. You need to find the possible ghost spawning area using those cursed object positions.

The ghost has a special affection for numbers

$1$

to

$9$

. An area is said to be a ghost spawning area if it is

divisible

by all the numbers from

$1$

to

$9$

.

Being a member of the ghost exploration team, you need to find out the number of ways of selecting one or more cursed object locations from those

$N$

locations such that the product of those locations returns a ghost spawning area.

Since the answer can be very big, output the answer modulo

$10^9 + 7$

.

Input

The first line of input is an integer

$N$

. The next line will contain

$N$

different integer numbers.

Constraints

$1 \leq N \leq 10^4$

$1\leq\text{all cursed positions}\leq 10^4$

Output

Print the number of ways of selecting one or more cursed object locations modulo

$10^9 + 7$

such that the product of those locations becomes a ghost spawning area.

Examples


---

## Samples

### Sample Input 1
```
7
1 2 3 4 5 6 7
```

### Sample Output 1
```
4
```

### Sample Input 2
```
6
1 2 3 4 5 6
```

### Sample Output 2
```
0
```
