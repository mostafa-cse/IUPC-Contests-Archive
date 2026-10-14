# Biswa and Red-Black Ants

**URL:** https://toph.co/p/biswa-and-red-black-ants  

---

Biswa has come to Antland for a trip. There are

N

holes in total in Antland. He can start visiting from any of the holes. In each hole, there is a magic number which is the number of the hole that Biswa should visit after the current hole.

K

of the holes are the hubs for red ants and the remaining holes are the hubs for black ants. One of the black ants' hole is also the headquarter of the black ants. There are some conditions while visiting the holes:

If Biswa starts his journey from any of the red ants' holes, he’s not allowed to visit the headquarter of black ants at any point of his journey.

if Biswa starts his journey from any of the black ants' holes, he must visit the headquarter of black ants at some point of his journey.

It is not allowed to visit any red ants' hole from the headquarter

Now your duty is to put the magic numbers in each of the holes. But before that you need to report the number of ways magic numbers can be assigned in each hole so that whichever hole Biswa starts from, all the above conditions are met.

Input

First line of the test case contains a positive integer

T (≤ 100)

denoting the number of test cases. In each test case, in first line there will be two positive integers

N (1 ≤ N ≤ 100000

) and

K (0 ≤ K < N)

. Then follows K more numbers

Ri (1 ≤ i ≤ K, 1 ≤ Ri ≤ N)

in the next line which are the hole numbers for red ants. In the final line there will be an integer

B (1 ≤ B ≤ N)

which is the headquarter and one of the hubs for the black ants.

Output

In each line print the remainder of the answer after dividing it by

1000000007 (109 + 7)

.

Example


---

## Samples

### Sample Input 1
```
2
3 1
1
2
11 10
1 2 3 4 5 6 7 8 9 11
10
```

### Sample Output 1
```
2
999999937
```
