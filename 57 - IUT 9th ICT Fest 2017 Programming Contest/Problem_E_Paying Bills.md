# Paying Bills

**URL:** https://toph.co/p/paying-bills  

---

Mued is finally home for summer vacation after surviving yet another semester of the mighty CS Undergrad Program. Oh! So long he had waited for this moment. He is looking forward to fructify the plan of not leaving his room for next 6-7 days.

On one fine morning of the vacation, when the room temperature was just perfect to cover himself with a comfortable sheet and do a lie down marathon; his father gave him the most annoying job he could think of – paying bills!! He was given

$N$

coins of value

$C_1$

,

$C_2$

, …,

$C_N$

and was told to pay some pending bills on

$M$

different stores. Bill of

$i$

-th store is

$B_i$

.

“There is no point of wondering why I am only given coins”, he thought. Rather he decided to make some fun out of it. He liked the sweet sound of coins in his pocket. And he wanted to enjoy it on his way back home too. The best way to do this would be to pay all the bills using minimum number of coins and keep the rest in his pocket. The storekeepers won’t give him any change as expected. “Whatever, can’t be more cruel than my old man”, said he with a grin on his face.

Being a talented programmer himself, Mued can find out the minimum number of coins needed to pay all the bills. He doesn’t need your help. You are here just to play along.

Input

There will be

$T$

(

$0 < T ≤ 1000$

) test cases.

Each case starts with a positive integer

$N$

(

$0 < N ≤ 15$

) denoting the number of coins. Then comes the value of each coin

$C_i$

(

$1 ≤ C_i ≤ 1000$

). Next, there will be an integer

$M$

(

$M ≤ N$

) denoting the number of stores followed by the bill of each store

$B_i$

(

$1 ≤ B_i ≤ 1000$

).

Output

Print case number and the minimum number of coins needed. Print -1 if it is not possible to pay all the bills with given coins.

Example


---

## Samples

### Sample Input 1
```
2
6
1 2 3 4 5 6
2
9 3
6
1 2 3 4 5 6
3
4 4 4
```

### Sample Output 1
```
Case 1: 3
Case 2: -1
```
