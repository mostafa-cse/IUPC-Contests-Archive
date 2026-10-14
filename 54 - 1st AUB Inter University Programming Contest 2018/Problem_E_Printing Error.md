# Printing Error

**URL:** https://toph.co/p/printing-error  

---

We all know programming contest is fun. Every year teams all over the country participate in many contest. The biggest programming contest of the year, hosted by Asian University of Bangladesh (AUB), has just begun and the problem set is given to all the teams. Suddenly just right after the beginning of the contest, an announcement comes out having said that the problems in the set given are not arranged in numeric order and the same problem may be present more than once. This makes the task of solving the problems much harder, also you may end up solving the same problem more than once and thus ends up losing the contest. You, being one of the team members, decided to rearrange the problems in a suitable format, you need to spend several minutes sorting them before you begin.

To deal with this situations, you have decided to write a program that prints out the list of problems in a way that each and every member of your team can guess which problems to attempt first. You set the following rules:

The numbers should be in order from lowest to highest

There should be no duplicates

Consecutive problem numbers if present should be grouped into a single segment, represented by a starting number, followed by a hyphen and end with the ending number.

The number should be grouped into as few segments as possible.

Rest problems should be separated by a comma followed by a space.

Input

The first line will contain a single, positive integer

$S$

representing the number of problem set given. For each set, there will be two lines. The first line will contain a single integer

$P$

(

$1 ≤ P ≤ 10^5$

) representing the number of problems in the set. Next following line will contain

$P$

integers

$P_i$

(

$1 \le P_i \le 10^5$

) representing the problem numbers.

Output

For each set, output a single line, starting with “Set #S: X” where

$S$

is the set number in the input and

$X$

is equal to the grouped version of the given integers following the above rules. Print a blank line after each set of problems.

Example


---

## Samples

### Sample Input 1
```
2
6
1 2 1 3 5 6
2
1 10
```

### Sample Output 1
```
Set #1: 1-3, 5-6

Set #2: 1, 10
```
