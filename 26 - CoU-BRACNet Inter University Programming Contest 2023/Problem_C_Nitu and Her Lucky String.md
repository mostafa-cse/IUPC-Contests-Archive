# Nitu and Her Lucky String

**URL:** https://toph.co/p/nitu-and-her-lucky-string  

---

Recently, Nitu has developed a keen interest in solving string-related problems. She possesses a special 'lucky' string. Just last week, Nitu stumbled upon a fascinating puzzle involving a square matrix, consisting of

$N$

rows and

$N$

columns. Each cell within this matrix contains only lowercase letters. Her objective is to navigate from the top-left cell

$(0, 0)$

to the bottom-right cell

$(N - 1, N - 1)$

while adhering to the following conditions:

Starting from any cell

$(i, j)$

, she can only move either to the right

$(i, j + 1)$

or downward

$(i + 1, j)$

.

During her journey from cell

$(0, 0)$

to cell

$(N - 1, N - 1)$

, she must collect all the letters encountered along the way. Subsequently, she will construct a string using these letters, and this string must contain her 'lucky' sequence at least

$M$

times as a substring.

While Nitu acknowledges that there might be multiple paths to reach her destination (from

$(0, 0)$

to

$(N - 1, N - 1)$

), she claims to have solved the problem in a single attempt and is now challenging you. Are you prepared to accept her challenge?

Input

The first line comprises an integer,

$T$

$(1 \leq T \leq 100)$

, representing the number of test cases.

For each test case:

The first line includes two integers,

$N$

$(1 \leq N \leq 100)$

and

$M$

$(0 \leq M \leq 10)$

.

The subsequent

$N$

lines contain strings of length

$N$

, forming a square matrix.

Following the matrix description, there are additional lines containing her "lucky" string contains only lowercase letters and

$1\leq |\text{lucky}|\leq 100$

where

$|\text{lucky}|$

means the length of “lucky“ string.

Output

For each test case, please output a single line in the following format:

$\texttt{Case \#}X\texttt{: }Y$

.

Here

$X$

represents the test case number, and

$Y$

represents the number of paths to reach Nitu's destination (from cell

$(0, 0)$

to cell

$(N - 1, N - 1)$

) modulo

$10^{9} + 7$

.

Example

Notes

A substring is a contiguous sequence of characters within a larger string.


---

## Samples

### Sample Input 1
```
2
3 2
abc
bbc
abb
bbb
4 3
abcd
bbcd
abbc
xyzp
bbb
```

### Sample Output 1
```
Case #1: 2
Case #2: 0
```
