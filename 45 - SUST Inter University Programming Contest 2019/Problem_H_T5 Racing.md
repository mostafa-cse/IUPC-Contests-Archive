# T5 Racing

**URL:** https://toph.co/p/t5-racing  

---

It is high time for the annual T5 racing and your team is planning to win the race. In T5 racing the drivers need to complete at most

$X$

laps (lap means a portion of a trip). However, the racing track is different from F5 racing. The T5 racing track has

$N$

checkpoints and each checkpoint

$i$

has score point

$P_i$

associated with it. Checkpoints are connected by some bidirectional racing roads and there is no cycle in the T5 racing track.

For example, there are four checkpoints in the picture and three racing roads connecting them. The rules of the T5 racing are very simple. At any point of time, if a driver is at checkpoint 2, he/she can move to any of the directly connected checkpoint 1 or 3 to complete one lap. The race will start at checkpoint 1 and the drivers can finish the race at any checkpoint. Two drivers can take two different paths to finished the race as long as they complete at most

$X$

laps.

A driver can add score point

$P_i$

to his/her to her scorecard when he/she enters checkpoint

$i$

for the first time. Drivers can enter the same checkpoint multiple time during the race but they will get the score only the first time. The highest score scorer will win the race and there can be multiple winners.

Since you are the greatest T5 hacker on this Galaxy, and you already know the racing track map for the next race. Now you have to tell what is the maximum score your team driver needs to win the race.

Input

Input starts with an integer

$T$

(

$0 < T ≤ 100$

), denoting the number of test cases. Each case starts with two integers

$N$

(

$1 ≤ N  ≤ 100$

) and

$X$

(

$1 ≤ X ≤ 200$

) as mentioned above. Next line contains

$N$

integers separated by space and the

$i$

-th integer of this line represents the score point

$P_i$

(

$0 ≤ P_i ≤ 10^5$

) of the

$i$

-th checkpoint. Next

$N -1$

lines will contain two integers

$i$

and

$j$

, meaning that there is a racing road between checkpoint

$i$

and

$j$

.

Output

For each case, print the case number and the maximum score point your team driver needs to win the race in a line.

Example


---

## Samples

### Sample Input 1
```
1
4 2
1 4 2 3
1 2
1 3
3 4
```

### Sample Output 1
```
Case 1: 6
```
