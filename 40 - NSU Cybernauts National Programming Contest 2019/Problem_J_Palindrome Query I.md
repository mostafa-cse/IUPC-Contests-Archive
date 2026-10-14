# Palindrome Query I

**URL:** https://toph.co/p/palindrome-query-i  

---

You are given a string of length

L

. You have

Q

queries. In each query, you will be asked to either update or delete a character in the string or check whether there is a palindrome in the string from index

i

to index

j

(inclusive).

Input

The first line of the input contains a string

S

. The string contains only English letters. The following line contains an integer

Q

denoting the number of queries for string

S

.

Each query can be one of the followings:

•

U i c

(update index

i

of string

S

with the character

‘c’

)

•

D i

(delete index

i

of string

S

)

•

C i j

(check whether the substring within index

i

and

j

(inclusive) of

S

is a palindrome or not)

Here, the first index is considered as 1.

1 ≤ |S|, Q ≤ 105

There is no such query that results in string of length 0. The value of

i, j

will be less or equal to the length of the string at that point of the query.

Output

For each query

C i j

, print

“Yes!”

if the substring within index

i

and

j

(inclusive) is palindrome, print

“No!”

otherwise.

Example

Notes

Explanation:

Original String: helloworld

C 5 7 -> hell

owo

rld

C 4 8 -> hel

lowor

ld

D 8 -> hellowo

r

ld -> hellowold

C 4 8 -> hel

lowol

d

U 9 l -> hellowol

d

-> hellowoll

C 3 9 -> he

llowoll


---

## Samples

### Sample Input 1
```
helloworld
6
C 5 7
C 4 8
D 8
C 4 8
U 9 l
C 3 9
```

### Sample Output 1
```
Yes!
No!
Yes!
Yes!
```
