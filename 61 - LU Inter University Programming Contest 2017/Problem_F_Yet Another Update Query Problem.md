# Yet Another Update Query Problem

**URL:** https://toph.co/p/yet-another-update-query-problem  

---

Given an array of n elements, you have to do Q operations. The operations can be of the following two types.

Operation

Description

Update(L,R,v)

You should add v to all Ai where L ≤ i ≤ R

Query(L,R,v)

You should output the frequency of the number v in the range from Lth to Rth index in the array.

The value of any element of the array will not be more than 200000 or less than 0 after any operation.

Input

In the first line, an integer

T

(1 ≤ T ≤ 5) denoting the number of test cases will be given. Each test case will contain the number

n

(1 ≤ n ≤ 100000) and

q

(1 ≤ q ≤ 100000) in the first line, the number of elements in the array and the total number of queries.The next line will contain n integers denoting the elements of the initial array. Then q lines will follow.

Each of the lines will contain 4 integers,

type

(1 ≤ type ≤ 2),

L

,

R

(1 ≤ L ≤ R ≤ n), and

v

(-100000 ≤ v ≤ 100000).

If type is 1, then this would mean an operation of the first type i.e an update operation. Otherwise, it would mean an operation of the second type i.e a query operation.

The initial array will contain non negative numbers less than or equal to 100000.

The value of any element of the array will not be more than 100000 or less than 0 after any operation.

Output

For each test case, print the case number in one line. Then print the result for each query of type 2 in different lines. Refer to the sample section for input format.

Example


---

## Samples

### Sample Input 1
```
1
5 5
1 2 3 4 5
2 3 4 3
1 3 4 -2
2 3 4 3
1 4 4 -1
2 3 4 1
```

### Sample Output 1
```
Case 1:
1
0
2
```
