# Maximum Sum

**URL:** https://toph.co/p/maximum-sum  

---

Little Jimmy loves to play with numbers. One day he was playing with a number sequence. In his game, he picked an array of integers and computed the sum of all the numbers in that array.

Then after playing for couple of hours, he got bored and wanted more challenge. Then he came up with the following game.

The rules for the game is as follows:

First he is given an array of N integers (now the game starts).

In each step, he picked a non-empty contiguous subarray and multiply the sum of elements of the sub-array with the size of the subarray. This product is added to his score. After that he removed the whole subarray from the array. The subarray must be picked sequentially. That is, xth element can't be picked before picking (x-1)th element.

He continued doing step 2 until the array became empty.

Can you determine the maximum score he can obtain?

Input

First take a number

T

(1 ≤ T ≤ 1000) as input, which indicates the total number of testcases. Now for each case, take a number

N

(1 ≤ N ≤ 1000) which indicates total number of elements in the array. Now take N numbers (each between -10000 and 10000, inclusive) as input and compute the maximum score that can be obtained for the new game.

Output

For each case, print the maximum score in a new line.

Example


---

## Samples

### Sample Input 1
```
2
3
1 2 3
2
1 2
```

### Sample Output 1
```
18
6
```
