# Palindromist

**URL:** https://toph.co/p/palindromist  

---

Prof. Ying Zang has an affinity for symmetric objects. Perhaps that is why she loves palindromes. So during class when she gets bored she takes out her notebook and writes various palindromic strings.

A palindromic string is a string that reads the same backward. For example, “madam” is palindrome since if you reverse “madam”, you still get “madam”. “mister” is not palindrome as “mister” backward reads “retsim”.

Over the years, she has been through many boring classes and hence gained lots of experience with palindromes. Her experience allows her to detect palindromic strings rather quickly. Utilizing her unique skill, she has invented a game where she excels beyond imagination. The name of the game is “Palindromist”. She has declared that anybody who clears the game “Palindromist”, will be entitled “The Palindromist” by her.

The rules of the game are very simple. There will be an initial string

S

given. After that, Ying Zang is going to perform some operations on the string. At each operation, he will either prepend some characters on the left side of the string or append some characters to right side of the string. After each operation, the challenger must state whether the formed string is palindrome or not.

The operations will be of the following form:

s c k

, where

s

is either “

L

” or “

R

” denoting prepending at left side or appending at right side,

c

is a lowercase character that Ying Zang is going to append/prepend and

k

is the number of times c is added to string.

For example, the following is a game simulation of “Palindromist”.

Suppose the initial string given is “aba”.

So, do you think you have what it takes to be crowned as “The Palindromist”?

Input

The first line contains a single integer

T (1 <= T<=100)

, denoting the number of test cases. Next follows T test cases.

For each test case, first line contains the initial string

S (1 <= |S| <= 10,000)

. Next line contains a single integer

U (1 <= U <= 10,000)

denoting number of updates. Next, U lines follow with updates. Each update is of the form:

s c k

, where

s

is either “L” or “R” denoting prepending at left side or appending at right side, c is a lowercase character that Prof. Ying Zang is going to append/prepend and

k (1 <= k <= 100)

is the number of time

c

is added to string.

Output

For each test case, first print the case number in a single line. Then on next

U

lines, print whether the string formed by the corresponding update operation is a palindrome or not. If it is a palindrome, print “Yes”, otherwise print “No”. See sample input/output for more details.

Example


---

## Samples

### Sample Input 1
```
1
aba
4
L b 2
R b 1
R b 1
L z 3
```

### Sample Output 1
```
Case 1:
No
No
Yes
No
```
