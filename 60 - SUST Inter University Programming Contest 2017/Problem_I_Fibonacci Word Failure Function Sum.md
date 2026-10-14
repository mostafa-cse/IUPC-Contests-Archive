# Fibonacci Word Failure Function Sum

**URL:** https://toph.co/p/fibonacci-word-failure-function-sum  

---

The following is based on true events:

One day Nabila decided that she wants to learn algorithms on String. She came to me for advice and I told her to start with KMP algorithm. I gave her some basic ideas on how KMP works and redirected her to “Introduction to Algorithm” book. There she learnt about KMP in more details.

While learning about KMP algorithm, she also learnt about “failure function”. What is the “failure function”? Basically, failure function is a table which is built for a particular string

S

, where for each substring

s

of form

S[1...i]

, we store the length of the longest proper suffix (a proper suffix is a suffix which is not equal to the string itself) of

s

which is also a prefix of

S

at position

i

of failure function table.

For example, if we consider the following string:

S

= “accadaccac”, then it has the following failure function

f(S)

:

Here above,

At i = 6 value of f(s)[6] = 1 because maximum prefix('a') and suffix matching length is 1.

At i = 9 value of f(s)[9] = 4 because maximum prefix('acca') and suffix matching length is 4.

After learning the failure function, Nabila decided to practice calculating failure function on different strings.

The following is based on my imagination:

But eventually, Nabila became bored of calculating failure functions for common strings. So she decided to calculate failure functions for Fibonacci words. She defined the Fibonacci words as following:

F1 = a

F2 = b

F3 = ba

F4 = bab

…

Fn = Fn-1 + Fn-2

Here addition of Fibonacci words means concatenation of strings.

So Nabila picked a value for

n

, then calculated the value for

Fn

and then calculated the failure function for

Fn

. Here is what she did for

n

= 6, i.e,

F6

= “babbabab”:

But eventually she got bored of this too! So in order to make the task more challenging, she tried to calculate the sum of the values in failure function table,

SUM(f(Fn))

.

For example, SUM(f(F6)) = SUM(f(“babbabab”)) = SUM([0,0,1,1,2,3,2,3]) = 0+0+1+1+2+3+2+3 = 12.

The task proved to be too hard for Nabila, so she brought it to me. I found it interesting, so I brought it to you :)

Given the value of

n

, please find the sum of the terms in failure function of

Fn

, where

Fn

is the nth fibonacci word. Since the answer can be large, print the answer modulo 1000000007.

Input

First line contains a single integer

T ( 1 <= T <= 100000 )

, number of test case. Next T lines contains a single integer in each line denoting

n ( 1 <= n <= 1000000000 )

.

Output

For each

n

in test case, output a single integer which is the sum of the terms in failure function of

Fn

, i.e, SUM(f(Fn)). Since the answer can be large, print the answer modulo 1000000007.

Example


---

## Samples

### Sample Input 1
```
3
1
7
1000000000
```

### Sample Output 1
```
0
36
2170
```
