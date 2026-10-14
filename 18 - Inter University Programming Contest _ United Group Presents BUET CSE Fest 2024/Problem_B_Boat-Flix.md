# Boat-Flix

**URL:** https://toph.co/p/boat-flix  

---

There are

$N$

swimmers who want to cross a river. You are given

$K$

boats, each with a speed of

$Y$

meters per second, and each boat can be used by only one swimmer at a time. A boat cannot move on its own; it must be driven by a swimmer. The swimmers, on the other hand, can swim at a speed of

$X$

meters per second. The width of the river is

$D$

meters. A swimmer can swim for part of the way, ride a boat for part of the way, and even leave a boat midway for another swimmer to take it.

All swimmers start from the same bank of the river at the same time. Initially the boats are also present on the same bank. Your task is to determine the minimum amount of time required for the last swimmer to reach the opposite bank.

Input

The first line contains an integer

$T$

$(1 \leq T \leq 100)$

, the number of test cases.

Each test case consists of a two lines. First line contains two space separated integers:

$N$

,

$K$

, and the second line contains three space seperated integers,

$D$

,

$X$

, and

$Y$

.

$1 \leq N, K \leq 10^6$

$1 \leq D, X, Y \leq 10^9$

Output

For each test case, output a single line containing the minimum amount of time required for the last of

$N$

swimmers to reach the opposite bank.

Absolute or relative errors of up to

$10^{-6}$

in the output will be ignored.

Example


---

## Samples

### Sample Input 1
```
2
3 2
100 10 15
5 6
120 10 15
```

### Sample Output 1
```
7.7777777778
8.0000000000
```
