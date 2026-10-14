# Productive Employees

**URL:** https://toph.co/p/productive-employees  

---

Congratulations on becoming the new boss of "Horizontal Company, branch: Sylhet"! But now you have a hard task in front of you, The central branch has sent you a list of

$M$

prospective employees to put in your office. However, just like it's name, the company's office is a long horizontal continuous segment

$[0, N]$

. Each employee has a specific coordinate

$X$

where he will work, along with a radius

$R$

of workspace. i.e. any point

$< R$

distance from X is used by that employee for work (points at exactly R distance are not used). Formally speaking, consider any coordinate

$Y$

(not necessarily integer), if

$|Y-X| < R$

then this point is used by the employee. Being an efficient boss, you want to select the maximum number of employees such that their workspaces don't intersect.

But there's another problem! This branch is relatively new, so the whole office is not really open yet. The central office will give you a segment

$[L, R]$

to work with. The workspaces of the selected employees should be strictly inside the given segment. The central office has sent you

$Q$

emails each containing a segment

$[L, R]$

. You need to tell them what is the maximum number of employees you can select for each such segment. Note that each segment is independent from other emailed segments.

Input

First line will contain number of test cases,

$T$

(

$1 \le T \le 10$

). Each test case will be an independent office (and staff). Each test case will begin with a line containing

$N$

(

$1 \le N \le 10^9$

) and

$M$

(

$1 \le M \le 10^5$

). Next

$M$

lines will contain two numbers,

$X$

(

$0 \le X \le N$

) and

$R$

(

$1 \le R < N$

), the employee's working coordinate and radius of work. Next line will contain

$Q$

(

$1 \le Q \le 10^5$

). Next

$Q$

lines will contain

$L$

and

$R$

(

$0 \le L < R \le N$

).

Output

For each test case, first output "Case #:" in a single line. Then for each of the emailed segments

$[L, R]$

in that case, output a line containing the maximum number of employees you can select for that segment.

Example


---

## Samples

### Sample Input 1
```
2
20 3
5 5
15 5
10 10
1
0 20
20 3
5 5
15 5
10 5
2
3 17
10 15
```

### Sample Output 1
```
Case 1:
2
Case 2:
1
0
```
