# Sequence Query

**URL:** https://toph.co/p/sequence-query  

---

You are given

$N$

integer numbers

$(A_1, A_2, A_3 … A_N)$

. You will also be given some query. Each query will be of the format

$(L, R)$

. For each query you need to find all the sequence such that

$L \le v_1 < v_2 < v_3 … < v_k \le R$

, and

$(Av_1 + Av_2 + Av_3 + … + Av_k)$

is divisible by

$M$

. You need to find out the sum of product of all the numbers in all such sequences. Basically

$\text{SUM of all possible}(Av_1 * Av_2 * Av_3 * … * Av_k)$

.

Input

The first line contains three integers

$N$

,

$Q$

,

$M$

(

$1 \le N, Q \le 300000, 1 \le M \le 30$

). The following line contains

$N$

integers

$A_1$

,

$A_2$

,

$A_3$

, …,

$A_N$

(

$0 \le A_i < 1000000000$

). The next

$Q$

lines each contain two integers

$L$

,

$R$

(

$1 \le L \le R \le N$

).

Output

Print

$Q$

lines, each line must contain the result of the query modulo 1000000007

Example


---

## Samples

### Sample Input 1
```
5 2 2
1 2 3 4 5
1 5
2 4
```

### Sample Output 1
```
359
14
```
