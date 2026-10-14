# Eloa’s Secret

**URL:** https://toph.co/p/eloa-s-secret  

---

Eloa, the princess of Byteland has a secret. She is obsessed with Alien names. The general convention of human name is “First name + Space + Last name”. There is one difference in alien name. The space replaced by a “:”. For example,

“donald:trump”

is a valid alien name. Obviously first name and last name can’t be empty. They must have at least one character each and only consists of lowercase English letters. Eloa has a long string

S

consists of lowercase English letters and “:”. She wants to know how many

distinct

sub-strings of

S

are there which can be considered as valid alien names. As she is very busy doing her makeup for the upcoming beauty contest, she ask you to do the task. Remember, you have to find the answer before she finishes her makeup. Otherwise the King of Byteland will hang you!

Input

Input starts with a positive integer

T

(1 ≤ T ≤ 1000), denoting the number of test cases. Each of the next

T

lines

contains a string

S

(1 ≤ |S| ≤ 50000).

It is guaranteed that ∑|Si| ≤ 500000.

Output

For each test case, print the output in the format,

“Case t: rt”

(without the quotes) in a separate line. Here

t

is the case number starting from 1, and

rt

is the number of distinct alien names of

tth

test case.

Example

Notes

Use scanf/printf for faster I/O.


---

## Samples

### Sample Input 1
```
4
a:b
abc
aa:ba:bb
a::b
```

### Sample Output 1
```
Case 1: 1
Case 2: 0
Case 3: 7
Case 4: 0
```
