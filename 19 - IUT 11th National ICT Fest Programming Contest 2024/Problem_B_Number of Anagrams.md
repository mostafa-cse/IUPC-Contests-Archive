# Number of Anagrams

**URL:** https://toph.co/p/number-of-anagrams  

---

You will be given a list

$L$

. Each element

$L_{i}$

will contain a list of integers. You have to perform two types of queries in list

$L$

.

$1$

$i$

$l$

$r$

$x$

$y$

This is the query of type 1 which asks you to replace the elements

$L_{i_{k}} (l \leq k \leq r)$

with

$y$

if

$L_{i_{k}} = x$

.

$2$

$i$

Query type 2 asks you to determine the number of anagrams of

$L_{i}$

in list

$L$

.

Definitions:

Anagram

: Two arrays are anagrams if one can be formed by rearranging the elements of the other. Note that, in this problem, we consider an array to be an anagram of itself.

Input

The first line of the input file will contain a positive integer

$N(1\leq N \leq 10^{5})$

which denotes the number of elements in list

$L$

.

Each of the next

$N$

lines will start with a positive integer

$M$

denoting the number of elements of

$L_{i}$

. Following by a space there will be

$M$

space separated positive integers. Note that,

$(1\leq L_{i_{j}} \leq 10^{4})$

.

Then, you will be given a positive integer

$Q(1\leq Q \leq 6 \times 10^{5})$

in a new line.

After that you will be given the queries in the next

$Q$

lines as described in the statement.

$1$

$i$

$l$

$r$

$x$

$y$

Here,

$(1 \leq i \leq N)$

,

$(1\leq l \leq r \leq |L_{i}|)$

,

$(1\leq x,y \leq 10^{4})$

$2$

$i$

Here,

$(1\leq i \leq N)$

Note that,

$(1 \leq \sum_{i=1}^{N}{|L_{i}|} \leq 10^{5})$

and there will be at least one query of type 2.

Output

For each query of type

$2$

, print the answer in a new line.

Example


---

## Samples

### Sample Input 1
```
3
2 10 20
2 20 10
2 10 10
5
2 2
2 3
1 1 2 2 20 10
2 2
2 3
```

### Sample Output 1
```
2
1
1
2
```
