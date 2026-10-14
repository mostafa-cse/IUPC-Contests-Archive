# Power of a string

**URL:** https://toph.co/p/power-of-a-string  

---

A string has power

$p$

if its can be divided into consecutive blocks of size

$p$

and each block consisting of the same character.

For example:

The string "TTTTAAAAPPPP" has a power of 4 because it can be divided into three blocks of size 4: "TTTT", "AAAA", and "PPPP"

The string "AAPPXXYY" has a power of 2, as it can be divided into four blocks of size 2: "AA", "PP", "XX", and "YY"

The string "CCAATTT" has a power of 1 because each character can be treated as a block of size 1

Given, a string

$S$

and a integer

$p$

, find the length of longest sub-sequence of

$S$

which has a power of

$p$

or more. If there is no such subsequence, then output

$0$

.

Input

The first line contains an integer

$T$

$( 1 \leq T \leq 100)$

representing the number of test cases.

For each test case:

The first line contains a string

$S$

consisting of uppercase English letters

$(1 \leq |S| \leq 100,000 )$

.

The second line contains a integer

$p$

$( 1\leq p \leq |S|)$

The total sum of lengths of all strings

$S$

across all test cases does not exceed

$500,000$

Output

For each test case, output a single integer on a new line, representing the length of the longest subsequence of

$S$

that has a power of

$p$

or more. If there is no such subsequence, then output

$0$

.

Example

Notes

For the first test case, the string “ABACACCBCDBDD” has a subsequence “AAACCCDDD” whose power is

$3$

(which is greater than

$p=2$

). So, the answer for this case is

$9$

.

In the third test case, the string “ABCABCABCABC” has a subsequence “AAAA” whose power is

$4$

(which is greater than

$p=3$

). So, the answer for this case is

$4$

.


---

## Samples

### Sample Input 1
```
5
ABACACCBCDBDD
2
AABBCCDD
1
ABCABCABCABC
3
ABABABABABAB
4
AAAAABBBBBCCCCCDDDDD
4
```

### Sample Output 1
```
9
8
4
6
20
```
