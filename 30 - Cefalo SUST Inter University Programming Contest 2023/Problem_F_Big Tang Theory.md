# Big Tang Theory

**URL:** https://toph.co/p/big-tang-theory  

---

Shell Don (Shelly in short) is a theoretical physicist who is claimed to be highly intelligent with an IQ of 187.

Shelly has decided to drink Tang (a brand of drink mix) regularly. To start out, he made a plan for the next

$N$

days. Through rigorous calculations, he decided that the maximum amount of Tang he can drink on the

$i$

-th day is

$A_i$

. He also decided that he will drink Tang only for a few consecutive days among these

$N$

days and on each of those days, he will drink the same amount of Tang.

After hearing this, to make fun of Shelly's intelligence, Pe Nie decided to give Shell Don a math problem. Pe Nie will ask Shelly

$Q$

queries. In each query, she will give Shelly a range of days

$[L, R]$

. Shelly needs to find the maximum total amount of Tang he can drink within some consecutive subset of days from the

$L$

-th to

$R$

-th day in his schedule (note that he must drink the same amount of Tang on each day of his chosen subset).

More formally, if Shelly’s chosen consecutive subset of days starts from the day

$a$

and ends at the day

$b$

, then

$L\leq a\leq b\leq R$

must be satisfied and he must drink the same amount of Tang on each day of the days in

$[a,b]$

range. What is the maximum total amount of Tang he can consume?

Despite Shelly's phenomenal intelligence in some sectors, he does have trouble showing true intelligence in many other sectors (especially social common sense and math problems like this). So can you help Shelly in solving this problem so that he is not utterly humiliated in front of Pe Nie?

Input

Input starts with two space-separated integers

$N\space(1\leq N\leq 10^5)$

(the number of days in Shelly's schedule) and

$Q\space(1\leq Q\leq 10^5)$

(the number of Pe Nie's queries).

In the next line,

$N$

space-separated integers are given, the

$i$

-th integer

$A_i\space(1\leq A_i\leq 10^9)$

representing the maximum amount of Tang Shelly can eat in the

$i$

-th day.

In each of the following

$Q$

lines, two space-separated integers

$L$

and

$R\space(1\leq L\leq R\leq N)$

are given, representing the range of days Pe Nie provides in her queries.

Output

Print

$Q$

lines, where the

$i$

-th line contains a single integer representing the answer to Pe Nie's

$i$

-th query.

Example


---

## Samples

### Sample Input 1
```
5 4
2 5 2 7 9
1 3
1 2
2 4
2 5
```

### Sample Output 1
```
6
5
7
14
```
