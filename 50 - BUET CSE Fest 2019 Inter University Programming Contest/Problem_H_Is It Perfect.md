# Is It Perfect

**URL:** https://toph.co/p/is-it-perfect  

---

Bob has an initial array

D

of length

n

. Alice is a good friend of Bob. So Bob challenges Alice to finish the following task with this array D.

A Sequence G is called

PERFECT

if elements of G are

distinct

and one of the two following properties hold :

If product of elements of G is a

perfect-square

then number of elements of G should be

even

.

If product of elements of is not a

perfect-square

then number of elements of G should be

odd

.

Alice's task is to find out the number of different ways to construct non-empty

PERFECT

sub-sequences of D. Alice is not an expert programmer. So now he wants your help. Can you find it?

A sub-sequence is a sequence that can be derived from another sequence by deleting some or no elements without changing the order of the remaining elements.

Two ways are considered different if sets of indexes of elements chosen by these ways are different. You have to find the answer

modulo

993344777

.

Input

First line contains one integer n (1 ≤ n ≤ 10^6) — the number of elements in the array.

Second line contains n integers - the elements of the array D where 1≤ D[i] ≤ 60 for 1 ≤ i ≤ n .

Output

Print one integer — the number of different ways modulo

993344777

.

Examples

Notes

For the first test case, you can make three sub-sequences :

you can choose only 2

you can choose only 8

you can choose both 2 and 8 because 2 * 8 = 16 is a perfect-square


---

## Samples

### Sample Input 1
```
2
2 8
```

### Sample Output 1
```
3
```

### Sample Input 2
```
3
3 2 7
```

### Sample Output 2
```
4
```
