# Left and Right

**URL:** https://toph.co/p/left-and-right  

---

You are given an array of

$n$

distinct integers. You will take index

$k$

as input and have to find out minimum number of swaps that you have to make so that all the numbers left to

$k$

will be less than the value at index

$k$

and all the numbers right to

$k$

will be greater than the value at index

$k$

.

Input

First you will take an integer

$n$

(

$1 \le n \le 100000$

) as input. Here,

$n$

denotes the total number of elements in the array. Then you will take

$n$

numbers as input to your array (

$1 \le array_i \le 10^9$

). Next, you will take an integer

$m$

(

$1 \le m \le 100000$

) as input. Here,

$m$

denotes the total number of queries. Finally, for each query, you will take the index

$k$

(

$1 \le k \le 100000$

; first index of the array is considered as 1 instead of 0) as input and compute the minimum number of swaps.

Output

For each query, you have to print the minimum number of swaps.

Examples


---

## Samples

### Sample Input 1
```
3
3 2 1
1
2
```

### Sample Output 1
```
1
```

### Sample Input 2
```
7
3 1 2 5 6 7 4
1
4
```

### Sample Output 2
```
1
```
