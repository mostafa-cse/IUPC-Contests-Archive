# Again LCS

**URL:** https://toph.co/p/again-lcs  

---

You are given two permutations of the numbers from

1-N

called

P1

and

P2

. You are also given two integers

C1

and

C2.

Let

S1

be a sequence formed by concatenating

P1 C1

times. Also let

S2

be a sequence formed by concatenating

P2 C2

times. Your task is very simple, find the longest common sub-sequence of

S1

and

S2

.

Input

The first line contains an integer

T (1 ≤ T ≤ 15)

, denoting the number of test cases. Each test case consists of

4

lines. The first line contains an integer

N (1 ≤ N ≤ 50,000)

. The second line contains the permutation

P1

separated by a single space. The third line contains the permutation

P2

separated by a single space. The fourth line contains two space separated integers

C1 (1 ≤ C1 ≤ 5)

and

C2 (1 ≤ C2 ≤ 5)

.

Output

For each test case, output the case number followed by the longest common sub-sequence as required. Please check the sample i/o for more clarity of the exact format.

Example


---

## Samples

### Sample Input 1
```
4
3
1 2 3
2 1 3
1 2
3
1 2 3
2 1 3
2 2
7
3 1 7 6 5 2 4
1 2 3 7 6 5 4
3 2
10
1 2 3 4 5 6 7 8 9 10
10 9 8 7 6 5 4 3 2 1
5 3
```

### Sample Output 1
```
Case 1: 3
Case 2: 4
Case 3: 12
Case 4: 7
```
