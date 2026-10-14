# Fun With Fraction

**URL:** https://toph.co/p/fun-with-fraction  

---

Dulal is a school going kid. He is learning basic math right now. Today he has learned about division and fraction. His teacher has assigned few homeworks on it. In the assignment, the teacher will provide few pair of integers representing the numerator and denominator of a fraction and Dulal needs to print the fraction in string format. If the fractional part is repeating, he needs to enclose the repeating part in parentheses. Can you help Dulal to prepare his homework?

Input

In the first line, you will be given an integer

T

, denoting the number of test cases. For each test case, you will be given two integers

N

and

D

representing the numerator and denominator of a fraction.

Constraints:

1 <= T <= 1000

--2^63 <= N, D <= 2^63-1

D != 0

Output

For every test case, you just need to print a single line

“Case T: X”

where

T

is the test case number and

X

is the fraction in string format.

If the fraction has any recurring pattern, then place parentheses "()" around that pattern. If the fraction has more than 1000 digits after the decimal point ("."), you need to print first 1000 digits and then print three dots ("..."). See sample input/output for exact formatting.

Example

Notes

Note:

In case 6 of the sample i/o, the output is actually a single line.


---

## Samples

### Sample Input 1
```
6
0 1
1 1
-1 -2
1 -3
-1 4
39 5658511659156
```

### Sample Output 1
```
Case 1: 0
Case 2: 1
Case 3: 0.5
Case 4: -0.(3)
Case 5: -0.25
Case 6: 0.0000000000068922717402012170367657821843262438666727691824658742843345484766533747699824388637674342798861908737719107390623442956320812079962165421337678681324657870730271013154782248005942293545970230580526695355429298678865376427440705795905341598561645149845998286141204585501053234581987046747058760581314697499559381430987122491456195282062744537679534690541139095013673859990162278437665526167951680793346853082137988207542981725898975451905092527706817183334133785761962875443309887404942370476580649244828819167377225723922318207433089669920999629328911498108250130283086331920525699533669192864474330477498094423473962001769918404567502673212653988980466281605137408460290417204951931144554614187364614244540716281283118278738856893555574155724352538920341032371181476247285344632957570130767599971750849829680781687432376828254680320486774465794922060676802461375721770166169309266784633085154096920933102363045680883939462389663946765972798414359199511081181440448338165258529733502077663...
```
