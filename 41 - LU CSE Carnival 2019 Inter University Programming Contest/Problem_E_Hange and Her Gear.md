# Hange and Her Gear

**URL:** https://toph.co/p/hange-and-her-gear  

---

Hange has developed a special gear to attack the Cart Titan. The gear is a round, disc-like object. Its front surface is smooth but the rear surface has

N

small, equal-sized cells along the perimeter. These cells can charge deadly shrapnel. To assemble a gear, Hange picks a sequence of

N

, not necessarily distinct, positive integers and assigns them to the

N

cells. She calls this sequence an assembly. For demonstration purpose, she has sketched a prototypical figure of a gear with

N=4

.

The laziness of a cell is the number assigned to it by Hange which denotes the interval between two shrapnel charges of the cell. If we assume that the gear is thrown around the Titan's neck at time

T = 0

and a cell's laziness is

L

, then the cell will charge shrapnels at times

T =

L

,

2L

,

3L

and so on. Although, there's a small flaw in the current design. When all the

N

cells charge at the same time, the gear explodes on itself immediately after the charge. Once the gear explodes, none of its cell can function anymore.

The Cart Titan is well known for its endurance. It builds a protective shield along its neck as soon as it sees the gear and sadly, the gear can't do any damage to the shield, let alone kill the Titan. There's a slim chance though, as Hange came to know that at time

T = K1

the shield becomes unstable and it remains unstable until

T = K2

. While the shield is unstable, it's possible to kill the Titan. But even without its shield, the Cart Titan is very hard to kill and it will only die if all the

N

cells charge shrapnel simultaneously (thus destroying the gear in the process). Now Hange needs to make her design decisions quickly and she needs your help to figure out, in how many different ways she can assemble a gear so that it can kill the Titan. As the gear is round, two assemblies are considered to be the same if one can be obtained from the other by applying rotations. See the sample I/O to get a more clear idea.

Input

The only line will consist of three integers,

N

,

K1

and

K2

.

1 ≤ N, K1, K2 ≤109, 0 ≤ K2 - K1 ≤ 106

Output

Print a single line containing the number of ways modulo

109+7

.

Examples


---

## Samples

### Sample Input 1
```
4 3 3
```

### Sample Output 1
```
5
```

### Sample Input 2
```
4 9 10
```

### Sample Output 2
```
77
```
