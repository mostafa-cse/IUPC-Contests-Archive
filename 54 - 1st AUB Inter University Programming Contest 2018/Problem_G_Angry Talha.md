# Angry Talha

**URL:** https://toph.co/p/angry-talha  

---

Talha is a very good student and topper of his class. He is very good at teaching others too. One day, he is going to be a faculty for sure.

Generally, he takes classes of his juniors on algorithms. But alas, his students are very "Fakibaz". Although Talha tries his level best but they don't work hard at all. As a result, Talha has become very angry and told them, "I won't take your class anymore -_-".

Hearing this, his students started crying and told him to give them another chance. Talha told them that he will take another class today on string and give them a problem based on this topic. If they can solve it, only then Talha will continue taking their classes.

But Talha, being wicked as always, thought of teaching them a good lesson by giving them a very hard task. The task was like this.

You are given 3 strings

A

,

B

,

C

and an integer

K

. Find the longest common substring between

A

and

B

and then remove it from string

B

. (If there are more than one such string, then choose the lexicographically smallest one and if there are still ties, then take the one which comes first in

B

). Then take the remaining part of

B

and add it to the end of

C

. Assume that is the new string

D

.

From

D

, you have to find out:

The substring length of the longest palindrome.

Starting index of a substring having a length of

K

that can be permuted to make a palindrome. (If there are more than one, then take the one that comes first).

The number of distinct palindromes that can be made by permuting the characters of that substring.

Input

There will be four lines denoting string

A

,

B

,

C

and the integer

K

.

1 ≤ |A|, |B|, |C| ≤ 105

1 ≤ K ≤ 105

Note : |S| defines the length of string S.

A, B and C will contain only lower case letters and no white-space.

NOTE : Don't use "gets()" / "cin.getline()" for taking input. Instead use "scanf()" / "cin"

Output

In a line print the three outputs that is asked in the question.

As those numbers might be very big, print them modulo 1000000007 (109+7).

Example

Notes

Note :

For the sample case

A = "angryangry"

B = "angrytalha"

C = "aaa"

Longest common substring of A and B is "angry".

So, after removing it from B, only "talha" remains.

D = "aaatalha".

Now,

Longest palindrome is "aaa"

Starting index of a substring having length 5 that can be permuted into a palindrome is "aaata" and the starting index is 1 (it is the only such string).

Possible number of distinct permutations of "aaata" is

1

("aataa").


---

## Samples

### Sample Input 1
```
angryangry
angrytalha
aaa
5
```

### Sample Output 1
```
3 1 1
```
