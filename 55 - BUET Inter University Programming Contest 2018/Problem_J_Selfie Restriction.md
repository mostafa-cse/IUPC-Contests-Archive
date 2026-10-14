# Selfie Restriction

**URL:** https://toph.co/p/selfie-restriction  

---

Do you know the boy named Amlan? The only dream of his life is taking selfies. He takes selfies even in contests. Hence there are new rules in programming contests. These rules are like “You can take at most

x

selfies in

y

minutes”. If you break such rule and take a selfie, your team will get a penalty. That doesn’t stop Amlan from taking selfies. His teammates are angry but you know, he is a brilliant contestant. They cannot just replace him. Being this much helpless, they just want to know the total amount of penalty they will receive for Amlan’s selfies. You will be given all the rules and the times at which Amlan takes the selfies. You need to help his team to calculate the total penalty. To their great relief, the judges decided to delete all the records of Amlan’s selfies when his team receives some penalty. The contest runs for 300 minutes.

Input

The first line of the input contains

T

, the number of test cases. Each test case begins with two numbers

N

, and

M

.

N

is the total number of rules.

M

is the number of selfies Amlan took. Each of next

N

lines contains three space integers

x y z

that indicate the rule “One can take at most

x

selfies in

y

minutes. Breaking this rule will cause a penalty of amount

z

.” The next line contains

M

integers,

s1, s2, … , sm

in non-decreasing order, which are the times (in minutes) of Amlan’s selfies.

1<= T <=10

1 <= N, M <= 10000

1 <= x <= 10000

1 <= y <= 300

1 <= z <= 10000

1 <= si <= 300, for 1 <= i <= M

Output

For each test case, print only one integer in a separate line which is the total amount of penalty for the test case.

Example

Notes

Test case 1:

There are two rules:

You can take at most 1 selfie in 1 minute. Breaking this rule will cost a penalty of **10**.

You can take at most 1 selfie in 2 minutes. Breaking this rule will cost a penalty of **20**.

When Amlan took the second selfie at the first minute, he broke both of the rules and his teams received a total penalty of

30

. Good thing is, all the records have been deleted with the penalty. So, when he took the selfie at the 2nd minute, he didn’t break any rule at all.

Test case 2:

There is only one rule:

You can take at most 1 selfie in 2 minutes. Breaking this rule will cost a penalty of **25**.<br>

When Amlan took the 4th selfie, he broke the rule.

Test case 3:

Although all 8 selfies are taken in minute 1. But they are taken sequentially. So after taking first 2 then penalty 10 is added. Then next 2 will add penalty 10 and so on. So there will be total 40 penalty.


---

## Samples

### Sample Input 1
```
3
2 3
1 1 10
1 2 20
1 1 2
1 4
1 2 25
1 3 5 6
1 8
1 1 10
1 1 1 1 1 1 1 1
```

### Sample Output 1
```
30
25
40
```
