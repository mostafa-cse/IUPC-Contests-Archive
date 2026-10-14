# The Assignment

**URL:** https://toph.co/p/the-internship  

---

Bolt is working at a prominent company called Icefire. He has been given a task for evaluation. The task is about substring triplets. A string

$s$

of length

$n$

is given at first. To build a substring triplet

$(s_1, \, s_2, \, s_3)$

, the following procedures are followed (

$1$

-based indexing):

At first, three unique integers

$b_1, \, b_2, \, b_3$

$(1 \leq b_1, \, b_2, \, b_3 \leq n)$

are selected

Then an integer

$p$

$(1\leq p\leq n; \space \max(b_1, \, b_2)+p\leq n+1)$

is chosen such that the following two conditions are satisfied:

For each

$i$

$(0\leq i < p)$

,

$s_{b_1+i} = s_{b_2+i}$

If

$\max(b_1, \, b_2)+p \leq n$

,

$s_{b_1 +p} \neq s_{b_2+p}$

Let,

$e_1$

be

$\min(n, \, b_1+p)$

. The substring

$s_1$

is the substring

$s_{b_1}, s_{b_1+1}, \dots, s_{e_1}$

Similarly, another integer

$q$

$(1\leq q\leq n;\space \max(b_3,b_2)+q\leq n+1)$

is chosen such that the following two conditions are satisfied:

For each

$i$

$(0\leq i < q)$

,

$s_{b_3+i} = s_{b_2+i}$

If

$\max(b_3, b_2)+q \leq n$

,

$s_{b_3 +q} \neq s_{b_2+q}$

Let,

$e_3$

be

$\min(n, b_3+q)$

. The substring

$s_3$

is the substring

$s_{b_3}, s_{b_3+1}, \dots, s_{e_3}$

Finally, the substring

$s_2$

is generated. Let,

$e_2$

be

$\min(n, b_2 + \max(p, q))$

. The substring

$s_2$

is the substring

$s_{b_2}, s_{b_2+1}, \dots, s_{e_2}$

The score of the substring triplet is

$p\times q$

.

For example, let a string

$s$

of length

$n=10$

is

$\tt{abababcxya}$

and

$b_1=3, b_2=1, b_3=10$

. According to the conditions above, the value of

$p$

will be

$4$

and so,

$e_1 = \min(n, b_1+p) = \min(10, 3+4) = 7$

. So, the substring

$s_1 = \tt{ababc}$

from

$\tt{ab\underline{ababc}xya}$

. Similarly, the value of

$q$

will be

$1$

and so,

$e_3 = \min(n, b_3+q) = \min(10, 10+1) = 10$

. So, the substring

$s_3 = \tt{a}$

from

$\tt{abababcxy\underline{a}}$

. Finally, the value of

$e_2$

will be

$\min(n, b_2+\max(p,q)) = \min(10, 1+\max(4,1)) = 5$

. So, the substring

$s_2 = \tt{ababa}$

from

$\tt{\underline{ababa}bcxya}$

. The score of this substring triplet

$(\tt{ababc}, \tt{ababa}, \tt{a})$

is

$p\times q = 4\times 1 = 4$

.

Icefire tells a substring triplet good if the substrings

$s_1, s_2, s_3$

are non-empty and lexicographically

$s_1 < s_2 < s_3$

satisfies. Bolt has already generated all possible good substring triplets. Now, he needs to calculate the sum of their scores. Can you calculate it for him?

A substring of a string

$s$

is a string that consists of some consecutive characters from string

$s$

. A string

$a$

is lexicographically smaller than a string

$b$

if either

$a$

is a prefix of

$b$

and

$a \neq b$

, or in the first position where

$a$

and

$b$

differ, the string

$a$

has a letter that appears earlier in the alphabet than the corresponding letter in

$b$

.

Input

The first line contains an integer

$T\space(1\leq T\leq 10^5)$

— the number of test cases.

The second line contains an integer

$n\space (3\leq n \leq 5\times 10^5)$

— the length of the string.

The third line contains the string

$s$

— which consists of only lowercase English letters.

The sum of

$n$

over all test cases will not exceed

$5\times 10^5$

.

Output

In each test case, print a single integer in a line, the sum of the scores of the good substring triplets. As the answer can be very large, print it modulo

$998244353$

.

Example


---

## Samples

### Sample Input 1
```
2
10
abababcxya
5
zzzax
```

### Sample Output 1
```
19
2
```
