# Amicable Numbers

**URL:** https://toph.co/p/amicable-numbers  

---

From Wikipedia:

“Amicable numbers are two different numbers so related that the sum of the proper divisors of each is equal to the other number. (A proper divisor of a number is a positive factor of that number other than the number itself. For example, the proper divisors of 6 are 1, 2, and 3.) A pair of amicable numbers constitutes an aliquot sequence of period 2. A related concept is that of a perfect number, which is a number that equals the sum of its own proper divisors, in other words a number which forms an aliquot sequence of period 1. Numbers that are members of an aliquot sequence with period greater than 2 are known as sociable numbers.

The smallest pair of amicable numbers is (220, 284). They are amicable because the proper divisors of 220 are 1, 2, 4, 5, 10, 11, 20, 22, 44, 55 and 110, of which the sum is 284; and the proper divisors of 284 are 1, 2, 4, 71 and 142, of which the sum is 220.”

In this problem, you have to find the amicable numbers in a range

[A, B]

.

Input

First line will contain an integer

T (T < 100)

, number of test cases. Each case will contain two integers

A

and

B (0 <= A, B <= 10,000,000 and A <= B)

.

Output

For each case, print the case number and then list the amicable pairs on each line sorted by the first number. For each pair, write the smaller number first. An amicable pair falls inside the input range iff, both numbers are between

[A, B]

. See sample for more clarification.

Example


---

## Samples

### Sample Input 1
```
2
0 2000
230 2000
```

### Sample Output 1
```
Case 1:
220 284
1184 1210
Case 2:
1184 1210
```
