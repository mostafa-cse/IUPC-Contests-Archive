# String Factory

**URL:** https://toph.co/p/string-factory  

---

Welcome to the string factory where strings are generated in a peculiar manner. You are given a string

S

consisting of lowercase English alphabets. You can generate another string from the given string using the following algorithm:

if the ASCII value of character at current position ( say

S[i]

) is smaller than the ASCII value of character at next position ( say S[i + 1] ), you can change character at current position to any characters in between

S[i]

and

S[i + 1]

.

if the ASCII value of character at current position ( say

S[i]

) is greater than the ASCII value of character at next position ( say S[i + 1] ), you can change character at current position to any characters in between

S[i + 1]

and

S[i]

.

if the character at both current and next position is same, you have to change the current character to any other lowercase English alphabets except the current one.

How many distinct strings can you generate using the above mentioned algorithm?

Since, the answer can be very large, print it modulo

1000000007

.

Input

Input starts with an integer

T

(1 <= T <= 5) , denoting the number of test cases.  Each case starts with a string

S

, which may be of at most

50000

in length.

Output

For each case of input, output an integer number which represents the number of possible different strings generated using the algorithm above from given string modulo

1000000007

.

Example


---

## Samples

### Sample Input 1
```
2
acb
abc
```

### Sample Output 1
```
6
4
```
