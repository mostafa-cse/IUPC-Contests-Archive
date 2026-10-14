# Biswa and Restaurant Business

**URL:** https://toph.co/p/biswa-and-restaurant-business  

---

After huge success in Borhani business, Biswa has recently started restaurant business. He’s got the information about the numbers of customers for

$N$

days, a sequence of

$N$

integers

$a_1, a_2, …, a_N$

. He wants to calculate the popularity of his restaurant from this data. First he’ll choose a window of size

$K$

(

$K ≤ N$

). Then for each K-sized window from the original sequence (first

$K$

-sized window will contain

$a_1, a_2, …, a_K$

, second one will contain

$a_2, a_3, …, a_{K+1}$

, and so on), he’ll calculate the number of all possible continuous increasing sequences in it and write them down in order. It’ll create a sequence of

$N - K + 1$

integers

$b_1, b_2, …, b_{N-K+1}$

. Finally he’ll run the following function on the later found sequence:

Output of this function is the popularity that Biswa desires to calculate.

A sequence is increasing if for every two adjacent elements in it, the later one is greater than the previous one. A sequence containing a single element is considered to be a increasing sequence as well.

Input

First line of the test case contains a positive integer

$T$

(

$0 < T ≤ 10$

) denoting the number of scenarios. For each scenario the first line will contain two positive integers

$N$

and

$K$

(

$1 ≤ K ≤ N ≤ 10^5$

). The second line contains a sequence

$a_1, a_2, …, a_N$

(

$1 ≤ a_i ≤ 10^5$

), where

$a_i$

equals to the number of customers on

$i$

-th day.

Output

For each scenario, output a single integer - the popularity in a separate line. The answer may be large so compute it modulo

$10^9+7$

.

Example


---

## Samples

### Sample Input 1
```
1
4 3
1 2 3 2
```

### Sample Output 1
```
16
```
