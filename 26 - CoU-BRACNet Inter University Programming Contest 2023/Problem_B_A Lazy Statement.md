# A Lazy Statement

**URL:** https://toph.co/p/lots-of-cubes  

---

Milk has created an account in the newly launched social network Coffeebook. However, she cannot decide on a password for her account. So she’s asked Mocha for help (don’t ask me why she trusts Mocha this much).

Mocha has decided to make the process interesting for himself. At each step, he applies the following procedure to come up with a random number.

He creates a

non-empty

array

$A$

of

at most

$N$

integers. Formally,

$1\leq |A|\leq N$

.

The array elements should be positive integers at most

$M$

. Formally,

$1\leq A_i\leq M$

for each

$1\leq i\leq |A|$

.

Each element of the array (except the first one) should be divisible by the previous element. Formally,

$A_i\mid A_{i+1}$

should hold for each

$1\leq i<|A|$

.

After creating such an array, Mocha raises

the last

element of the array to the power

$K$

. This gives him a random number.

Mocha doesn’t want to bore himself with the same array over and over again. So at each step, he creates

a new array

(satisfying the above conditions), an array he hasn’t created before. He stops only when he runs out of arrays satisfying the above conditions. Then he adds up all the powers he’s extracted out of these arrays and adds them up. The result, modulo

$10^9+7$

, is the password he’ll suggest to Milk.

However, soon after coming up with this plan, Mocha realizes that it will take him a long time to go through all possible arrays. He can’t do it on his own. Can you help him?

Input

The only line of input will contain three space-separated positive integers

$N$

— the limit on the size of the array,

$M$

— the limit on the array elements,

$K$

— the power Mocha raises the last element of each array to.

These integers satisfy

$1\leq N,M\leq 10^{9}$

and

$0\leq K\leq 100$

.

Output

Print a single line containing the password, which is the sum (modulo

$10^9+7$

) of the last elements of all possible arrays satisfying the aforementioned conditions, raised to the power

$K$

.

Examples


---

## Samples

### Sample Input 1
```
1 3 0
```

### Sample Output 1
```
3
```

### Sample Input 2
```
2 2 3
```

### Sample Output 2
```
26
```

### Sample Input 3
```
314 15 92
```

### Sample Output 3
```
168177682
```
