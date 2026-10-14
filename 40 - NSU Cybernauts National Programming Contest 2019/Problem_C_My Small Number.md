# My Small Number

**URL:** https://toph.co/p/my-small-number  

---

You are given two integers

N

and

M

. Find another integer

X

divisible by

M

that has the same number of digits as

N

. If there are multiple such

X

, then print the one with the least number of digits different from

N

. If there are still multiple such

X

, then print the smallest one among them.

Here, the same number of digits mean the number of positions where there the two numbers have same digits. For example, the numbers "123" and "321" have 1 same digit in the second position.

The length of a number will be considered without leading zeroes.

Input

Input contains two space-separate integers

N

and

M

without leading zeroes.

10 ≤ N ≤ 10100

1 ≤ M ≤ 105 , M ≤ N

Output

Output one line containing integer

X

as described above, without leading zeroes.

Examples


---

## Samples

### Sample Input 1
```
10 5
```

### Sample Output 1
```
10
```

### Sample Input 2
```
10 7
```

### Sample Output 2
```
14
```
