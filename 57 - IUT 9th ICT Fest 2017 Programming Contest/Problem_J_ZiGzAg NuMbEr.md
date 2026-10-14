# ZiGzAg NuMbEr

**URL:** https://toph.co/p/zigzag-number  

---

A number is called a Zig-zag number if the differences between consecutive digits alternate between positive and negative. A Zig-zag number has the following properties.

It has at least 3 digits.

Differences between consecutive digits alternate between positive and negative where first difference can be either positive or negative.

It has no leading 0 (zero).

For example, 174925 is a Zig-zag number because the differences between consecutive digits (6, -3, 5, -7, 3) are alternating between positive and negative. 154, 190, 101, 909 and 13254 are some Zig-zag numbers while 123, 900 and 4556 are not.

You are given two integers

L

and

R

. You need to find all the Zig-zag numbers within the range

L

and

R

inclusive, sort them in ascending order with respect to their Digit Sum and answer the

Kth

Zig-zag number in the sorted sequence.

Digit Sum

of a number is the sum of all its digits.

Digit Sum

of (40528) = 4+0+5+2+8 = 19.

Let,

x

and

y

are two Zig-zag numbers within the range

L

and

R

inclusive. In sorted sequence of Zig-zag numbers,

x

will appear before

y

if

any

of the followings satisfies:

Digit Sum of (x) < Digit Sum of (y)

Digit Sum of (x) = Digit Sum of (y)

and

x < y

.

Let,

L

= 120,

R

= 140 and

K

= 6.

From 120 to 140 there are 6 Zig-zag numbers. They are 120, 121, 130, 131, 132 and 140 and their digit sums are 3, 4, 4, 5, 6 and 5 respectively. If we sort them according to the given procedure, we will get the following sequence: 120, 121, 130, 131, 140 and 132. So, 6th Zig-zag number in the sorted sequence is 132.

Input

The input begins with a single positive integer

T (≤100000)

on a line by itself indicating the number of the cases. Each of the next

T

lines contains three space separated integers

L

,

R

and

K

(1 ≤ L ≤ R ≤ 10^18, 1 ≤ K ≤ 10^18)

.

Output

For each test case, print the test case number followed by

Kth

Zig-zag number in the sorted sequence. If there is no such Zig-zag number, print

-1

. You should follow the exact format as the sample output.

Example

Notes

Explanation

Case 1:

There are 8 Zig-zag numbers from 153 to 165. If we sort them according to the given procedure, we get the following sequence: 160, 161, 153, 162, 154, 163, 164 and 165.

Case 2:

There are less than 30 Zig-zag numbers in the given range.

Warning

The input file is huge, please use faster I/O methods.


---

## Samples

### Sample Input 1
```
3
153 165 3
100 165 30
1 142 11
```

### Sample Output 1
```
Case 1: 153
Case 2: -1
Case 3: 132
```
