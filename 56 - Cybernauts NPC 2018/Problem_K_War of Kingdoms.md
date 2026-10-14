# War of Kingdoms

**URL:** https://toph.co/p/war-of-kingdoms  

---

There is a country named WARLAND. It is a big country, so it is divided into

$N$

kingdoms. Each kingdom has a King and an army of

$W_i$

warlords &

$S_i$

soldiers. Each king also possesses

$M_i$

amount of wealth. It’s not possible that all the armies in the country are of equal strength. In a army each warlords and soldiers has their own power, and an army’s strength is measured using this formula:

${\Sigma}_{i=1}^{i=W} P_{w_i} + {\Sigma}_{j=1}^{j=S} (P_{s_j} \times M)^2$

where:

${P_w}_i$

is the power of

$i$

-th warlord,

${P_s}_j$

is the power of

$j$

-th soldier &

$M$

is the amount of wealth for a particular kingdom.

Sometimes, two kingdoms face each other in the battlefield. Can you guess who will win the war?

Of course that army whose army power is greater than other. Or the war can have no result for having equal power of the armies. But kingdoms don’t always face each other only for war. Sometimes they also meet to build friendship among them so that a kingdom can take help of other kingdom in the battlefield to increase their army’s power. When two kingdoms become friend, their army’s power will be calculated considering them as a single army, i.e: All the soldiers and warlords of these two army together will be considered as a single army and the wealth of the two kingdoms will be combined to support them. This friendship is also mutual. i.e: If kingdom

$A$

& kingdom

$B$

are friend, on the other hand kingdom

$B$

& kingdom

$C$

are friend, then kingdom

$A$

&

$C$

are also friend of each other.

There is also an wizard in the country who can do black magic. He only works for the person who pays him more. A king could take his help to do some black magic in the battlefield. So, when the wizard does magic, the opponent’s memory of last

$X$

days are gone for the time of the war. After the war ends, he drives their memory back.

Let's discuss a timeline history of Warland for three days. At day 1, there are three kingdom in Warland. On the 2nd day, kingdom 1 & kingdom 2 become friends and they are preparing for a war together against the kingdom 3. Just before the war begins, kingdom 3 hires the wizard and wants to face a war against kingdom 1. The wizard is instructed to erase the memory of kingdom 1’s king for the last 2 days. So, kingdom 1’s king will forget that kingdom 2 is their friend (1st and 2nd days memory are gone till the war ends) and as a result he will not invite kingdom 2 to join the battle.

Now, you will be given a description of timeline history of Warland for

$Q$

days. In each day one of the following two events happen:

Event type 1: Kingdom

$A$

and kingdom

$B$

become friends. If they are already friends of each other, just ignore this event.

Event type 2: Kingdom

$A$

and kingdom

$B$

will face a war. Kingdom

$A$

’s king has hired the wizard for the battle and told him to remove kingdom

$B$

’s king’s memory for the last

$X$

days (excluding today). If the value of

$X$

is 0, that means the wizard isn’t hired. For this type of event considering the situation, we have to find who will win the war. After the war ends, kingdom

$B$

’s kings memory will be back again. It’s also guaranteed that

$A$

and

$B$

were never friend before.

I am trying to solve this problem for a long long time, starting from the ancient time. Still couldn’t find the solution. That’s why I am asking you guys to help me.

Input

First line of the input file will contain the number of testcases

$T$

(

$1 \le T \le 5$

).

Each test cases contains several lines. First line of the test cases contains

$N$

(

$1 \le N \le 100000$

), the number of kingdom in Warland. Kingdoms are numbered from 1 to

$N$

. Next follows

$3N$

lines where each three lines describes a kingdom together, i.e: 1st, 2nd and 3rd lines of the

$3N$

lines describes kingdom 1. 4th, 5th & 6th line describes kingdom 2 and so on. In each description of the kingdom, 1st line contains three integer:

$W$

,

$S$

(

$1 \le W, S \le 100000$

) &

$M$

(

$1 \le M \le 10000$

). Where

$W$

means the number of warlords for this kingdom,

$S$

means the number of soldiers in the army and M is the amount of wealth possessed by the King of the kingdom. The 2nd line contains W integers:

${P_w}_1$

,

${P_w}_2$

, …,

${P_w}_W$

each describing the powers of the warlords. 3rd and the final line of the description contains

$S$

integers:

${P_s}_1$

,

${P_s}_2$

, …,

${P_s}_S$

describing the powers of the soldiers. After all the description of the kingdoms, there will be an integer:

$Q$

(

$1 \le Q \le 100000$

) representing the number of days in the timeline history and then

$Q$

lines follows describing one of the event in the following format:

1 A B

: this means its a description for event type 1 whose details is given above.

2 A B X

: this describes the event type 2 whose details is given above too.

Other constraints:

$1 \le {P_w}_i, {P_s}_j \le 10000$

$1 \le A, B \le N$

$0 \le X \le 100000$

The summation of number of all the warlords and soldiers together will not exceed 200000 for a single test case.

Output

For each test case, the first line should contain the test case number in the format: “Case: X” where

$X$

is the number of test case (without quote). Later, for each event of type 2, there should be a line containing the winner kingdom’s ID or “No one can win this war!” (without quotes) if the war has no result.

Example


---

## Samples

### Sample Input 1
```
1
3
1 2 10
10
5 3
1 1 20
5
3
1 1 15
7
5
4
2 1 2 0
2 1 2 1
1 1 3
2 1 2 0
```

### Sample Output 1
```
Case 1:
2
2
1
```
