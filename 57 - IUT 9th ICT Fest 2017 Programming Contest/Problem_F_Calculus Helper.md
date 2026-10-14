# Calculus Helper

**URL:** https://toph.co/p/calculus-helper  

---

Everybody knows that engineering students have to do lots of math. As a student of a renowned engineering university, Moin is no exception. He has to take one or two mathematics courses in every semester. For example, he is attending the MAT-110 course in this semester which includes calculus. The instructor taught them some methods of finding the derivative of a polynomial function. He also showed them how to calculate higher order derivatives by successively differentiating the same polynomial again and again. For example, derivative of the polynomial

(X^2 + 5*X + 6)

is

(2*X + 5)

and derivative of

(2*X + 5)

is

2

. Therefore, 2nd order derivative of

(X^2 + 5*X + 6)

is

2

. Similarly, 3rd order derivative of this function is

0

.

Calculus is very hard and it requires plenty of practices to become proficient in it. Therefore, the instructor gave a set of problems as exercise during the summer vacation. Moin has already solved all of them. But he can not check whether his solutions are correct or not as the instructor did not provide any answer sheet. Moin doesn’t want to wait all the vacation. So he came to you with the problems and his solutions. Please help him by generating a answer script for the given problem set.

Input

The professor has given

T

, number of test cases. Each test case is described by two lines. The first line of each problem contains a single integer

O

denoting the order of derivative to be computed. The second line contains the polynomial equation. This polynomial is a function of

X

which is described in the format

c1

X^p1 + c2

X^p2 + ... + ck*X^pk

where each

ci

is the coefficient and each

pi

is the power of variable

X

. The terms are given in decreasing order of

X

's power (

pi

) and will be unique. You can assume that

X

will be omitted (from the polynomial equation) if the power term (i.e.

pi

) is

0

. You can also assume that,

ci

or

pi

will be integer and they will be omitted from the polynomial equation (both in input and output) if they are less than two.

Constraints:

1 ≤ T ≤ 20

0 ≤ O ≤ 7

0 ≤ pi ≤ 10

1 ≤ ci ≤ 10

Maximum length of a polynomial equation will be at most

1000

.

Output

For each problem, print the problem number followed by the derivative of given order. You are supposed to print the terms in decreasing order of

X

's power (

i.e.

pi

). See sample input and output carefully for formatting details.

Example


---

## Samples

### Sample Input 1
```
4
1
X^2 + 5*X
2
X^3 + 6*X^2 + 10*X
0
X^5 + 3*X^3
2
10*X + 5
```

### Sample Output 1
```
Case 1: 2*X + 5
Case 2: 6*X + 12
Case 3: X^5 + 3*X^3
Case 4: 0
```
