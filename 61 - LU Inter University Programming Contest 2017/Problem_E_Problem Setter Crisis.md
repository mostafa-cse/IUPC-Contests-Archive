# Problem Setter Crisis

**URL:** https://toph.co/p/problem-setter-crisis  

---

Competitive Programming is very popular in Leading University. There are many great achievements of Leading University in Programming Contest, such as 2 teams in top 20 in ICPC 2013 Dhaka Regional, 15th in NCPC 2016, 10th among 117 teams in NGPC 2017 and etc. Leading University also organizes Intra LU programming contest on each semester.

Now Leading University Computer Club is going to arrange Inter university programming contest, soon! Teams from junior and senior division are going to participate in this contest. But the organizer are facing problem on preparing the problem set for the contest. Local problem setters are not willing to set any problems withing this short time because of their tight schedule.

Mr Arif Ahmed a prominent problem setter proposes a solution for this matter, that is to hire N globally recognized problem setters to set the problems before the deadline. Each of the N problem setter has different skill to set a problem, thus the time each takes to set a problem may be different from the others. Each of the N problem setter takes Si seconds to set a problem with Di difficulty level (for i from 1 to N).

However, LUIUPC will be held at the S-th second. Not to mention that the organizers has given only 1 computer for the problem setters to set the problems, so the problem setters has to work alternately. It is allowed to ignore the time it takes to upload the problems, write the solutions, prepare the server and paying the problem setters. Since the organizers hardly managed to hire prominent problem setters from all over the Bangladesh, to ensure a healthy competition among the teams they want the quantity of problems to be maximum and moderate. First they want to maximize the number of problems, then maximize the difficulty level if and only if possible.

As an example, Let us suppose currently there are 3 problem setters available to set problems, where each of them could finish in S = {1, 5, 8} seconds and the difficulty level are D = {4, 5, 8} respectively and LUIUPC will be held on the 8th second. In such situation the most optimal solution is to hire the first and second problem setter which takes 1 + 5 = 6 seconds and achieve a total of 2 problems and among them highest difficulty level is 5.

Input

The first line of the input contains a number

K

(K ≥ 1), which is the number of input data sets in the file.

This is followed by K data sets of the following form:

The first line of each data set contains two integers

N

(1 ≤ N ≤ 1000),

S

(1≤ S ≤ 1018). N is the number of available problems setters and S is the time when LUIUPC will be held.

This is followed by N lines, each describing one problem i with two integers

si

(1 ≤ si ≤ 1000) and

di

(1 ≤ di ≤ 1018). si is the time i-th problem setter takes to set a problem and di is the difficulty level of that problem.

Output

For each test case, Print "Case i: M N" where i is the test case number, M is the maximum problem could be chosen and N is the highest difficulty level among the chosen problems. If no problem could be produced before LUIUPC starts, Print “RIP LUIUPC”.

Example


---

## Samples

### Sample Input 1
```
3
3 8
1 4
5 5
8 8
3 9
3 10
3 20
3 30
2 10
11 20
15 1
```

### Sample Output 1
```
Case 1: 2 5
Case 2: 3 30
Case 3: RIP LUIUPC
```
