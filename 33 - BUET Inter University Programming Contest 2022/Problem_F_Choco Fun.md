# Choco Fun

**URL:** https://toph.co/p/choco-fun  

---

You brought

$C$

chocolates to a party where there are

$A$

adults and

$K$

kids.

You know that an adult will always eat the chocolate fully and a kid will always eat the chocolate partially

. For each chocolate, you know how much happiness it brings to one who eats fully or partially. You want to give everyone

exactly one chocolate

so that the total happiness they get is maximized.

Input

The first line contains one integer

$T$

- the number of test cases. For each test case, the first line contains 3 integers

$C$

,

$A$

, and

$K$

denoting the number of chocolates, adults, and kids respectively. For the next

$C$

lines,

$i’th$

line contains two integers

$F_i$

and

$P_i$

, denoting the happiness one gets if he eats the

$i’th$

chocolate fully and partially respectively.

$1 \leq T \leq 10^6$

,

$1 \leq C \leq 10^5$

,

$0 \leq A, K \leq 10^5$

,

$A + K \leq C$

,

$0 \leq P_i \leq F_i \leq 10^9$

,

The sum of

$C$

over all test cases does not exceed

$10^6$

Output

For each test case, output in a line, the maximum sum of happiness they get. See sample for details.

Example


---

## Samples

### Sample Input 1
```
2
2 1 1
30 12
20 1
3 1 1
20 10
12 10
15 15
```

### Sample Output 1
```
32
35
```
