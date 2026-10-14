# Prime - Prime - Prime

**URL:** https://toph.co/p/prime---prime---prime  

---

Given an integer

$n$

, print

$n$

unique

integers in the range

$[1, 10^9]$

such that,

The bitwise AND value of all the numbers is a prime number.

The bitwise OR value of all the numbers is a prime number.

The bitwise XOR value of all the numbers is a prime number.

Input

Input consists of a single integer

$n(1 \leq n \leq 10^5)$

.

Output

Print

$n$

space-separated integers in a line. Do not print any extra spaces after the last integer.

Example

Notes

Notes

A

prime number

is a natural number greater than 1 and has exactly 2 divisors which are 1 and the number itself.

Bitwise OR

operation compares bits in the same index in the binary representation of all the numbers in question and if at least one of the bits was 1, it sets the corresponding resulting bit to be 1, otherwise 0.

Similarly,

Bitwise AND

operation sets the corresponding bit to 1 if all the bits were 1, otherwise 0.

Bitwise XOR

operation sets the corresponding resulting bit to 1 if an odd number of bits were set to 1, otherwise 0.


---

## Samples

### Sample Input 1
```
2
```

### Sample Output 1
```
2 7
```
