# Tasks

**URL:** https://toph.co/p/tasks  

---

Zico is a fan of Artificial Intelligence (AI). So he is doing a course on AI and even likes the teacher who takes the AI course very much. During class, he always listens to the teacher and responds very fast. Once he thought of an idea to impress the teacher by making a robot. This robot can do a large variety of tasks. But some tasks are required to be done before some tasks while others are needed to be done after some tasks. Zico became confused how to create the algorithm that tells the robot what to do. He is desperate to impress the teacher so he asks your help as he knows you are an expert in algorithms. He has the list of tasks that needs to be done, can you help him?

He needs to know, what is the minimum time required to perform any task. Assume that each task is done in 1 unit time and the robot can do multiple tasks in 1 unit time (provided that all the previous tasks that need to be done are already done).

Input

Input contains an integer

$T$

(

$T ≤ 10$

)

, which is the number of test cases. The following

$T$

lines each contain:

A number

$n$

(

$1 ≤ n ≤ 1000$

)

, which is the total number of tasks that needs to be done. It is guaranteed that there will be no tasks a and b such that a needs to be done before b and b needs to be done before a. And at least one task can be done without doing any other tasks.

The following

$n$

lines contain the name of the tasks followed by the number

$m$

(

$0 ≤ m ≤ n$

)

and then m tasks which must be done before this task. Following line will contain an integer

$q$

(

$1 ≤ q ≤ 10^5$

)

, which is the number of queries followed by

$q$

task names. Tasks names will only contain lower case English letters and no whitespace. Their length will be less than 40.

Output

For each test case, output the case number. Then in a newline, print the minimum time required to perform each task of the query. Each query must be answered in separate lines. See the sample output for clarification about output format.

Example


---

## Samples

### Sample Input 1
```
2
3
sleep 1 eat
eat 1 run
run 0
2
sleep
run
5
breakfast 0
study 1 breakfast
play 1 breakfast
sleep 2 play study
lunch 1 study
4
study
lunch
play
sleep
```

### Sample Output 1
```
Case 1:
2
0
Case 2:
1
2
1
2
```
