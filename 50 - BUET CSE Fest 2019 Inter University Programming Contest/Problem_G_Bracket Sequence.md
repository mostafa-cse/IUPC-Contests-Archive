# Bracket Sequence

**URL:** https://toph.co/p/bracket-sequence  

---

You are given an N-dimensional array A. Each cell of this array contains either an opening bracket or a closing bracket. Let the dimension of the array is D1 * D2 * D3 * ... * DN. The index of the array A starts from (0, 0, ... , 0) to (D1 - 1, D2 - 1, D3 - 1, ... , DN - 1).

You want to walk in this N-dimensional space. You can go to any adjacent cell from your current cell. But you cannot return to some cell that you have already been before. You have to visit every cell of the array. The last cell you visit also has to be adjacent to the cell you started from. You can start from any cell. And another thing, if you write the brackets one after another in the order you visited the cells, it has to form a balanced bracket sequence.

As it is difficult to input an N-dimensional array, we will give you a string S consists of only opening and closing brackets. The length of the string will be D1 * D2 * D3 * ... * DN. You have to construct array A from this string.

A[i1][i2][i3]....[iN] = S[(i1 * D2 * D3 * ... * DN) + (i2 * D3 * D4 * ... * DN) + ... + iN).

Input

First line of input consists of T which is the number of test cases.

Each test case starts with an integer N. Next line contains N integers which is the dimensions of the array D1, D2, D3, ... , DN.

Next line contains the string S whose length is D1 * D2 * D3 * ... * DN.

Constraints

Sum of the lengths of S over all the test cases does not exceed 105.

Di > 1.

N > 1.

Output

For each test case, you have to output either 'YES' if there is such walk. And then you have to print the indexes of cells in the order of the walk. If there is no such walk you just have to print 'NO'.

Example

Notes

Notes

Two cells (i1, i2, i3, ... , iN) and (j1, j2, j3, ... , jN) are adjacent if | i1 - j1 | + | i2 - j2 | + ... + | iN - jN | = 1.

A bracket sequence is a string containing only characters "(" and ")". A balanced bracket sequence is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters "1" and "+" between the original characters of the sequence. For example, bracket sequences "()()" and "(())" are regular (the resulting expressions are: "(1)+(1)" and "((1+1)+1)" ), and ")(", "(" and ")" are not.


---

## Samples

### Sample Input 1
```
2
3
2 2 2
)(()(())
2
3 3
))()(())(
```

### Sample Output 1
```
YES
0 0 1
1 0 1
1 0 0
1 1 0
1 1 1
0 1 1
0 1 0
0 0 0
NO
```
