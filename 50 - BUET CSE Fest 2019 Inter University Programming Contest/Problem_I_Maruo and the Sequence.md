# Maruo and the Sequence

**URL:** https://toph.co/p/maruo-and-the-sequence  

---

Maruo has a sequece A =

{a1,a2,......an}

.

Let us define a function

func(A,l,r)

which is the minimum

i

such that

ai

is the maximum value where

l<=i<=r

.

Two sequences

A

and

B

are similar if they have the same length

n

and for every

1<=l<=r<=n

,

func(A,l,r)

=

func(B,l,r)

.

For any given sequence A=

{a1,a2,......an}

, we define the weight of a sequence B=

{b1,b2,......bn}

be

∑bi

, where

1<=i<=n

, if the two sequences

A

and

B

are similar. Otherwise, we let the weight be equal to

0

. If each element of

B

is chosen independently and uniform randomly between 0 and 1, find the expected weight of

B

.

Please note that the elements of

B

are real numbers between

0

and

1

inclusive, and not necessarily only

0

or

1

.

Input

The first line will contain

n

(the length of the sequence)

1<=n<=1000000

.

The second line contains

n

integers (1<=ai<=n) denoting the sequence.

Output

The expected weight will be a rational number

p/q

, where p and q are co-prime numbers.

Output the answer modulo 109+7 i.e. output

pq-1

modulo 109+7.

Example


---

## Samples

### Sample Input 1
```
3
1 2 3
```

### Sample Output 1
```
250000002
```
