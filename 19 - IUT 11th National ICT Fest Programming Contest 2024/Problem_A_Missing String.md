# Missing String

**URL:** https://toph.co/p/missing-string  

---

This is an

Interactive Problem

.

The judge has a secret binary string

$S$

of length

$n(1 \leq n \leq 1000)$

.

You can do several queries on the string.

To do a query, print “?

$Q$

”. Here

$Q$

is any binary string of length

$m(1 \leq m \leq 2 \times n)$

.

The judge replies to your query with an integer, the number of substrings of

$S$

that are lexicographically smaller than

$Q$

.

Find the secret string by asking no more than

$2 \times n$

queries.

When you have figured out the secret string, print “!

$S$

” in a line and move on to the next test case.

Input

The first line contains a single integer

$T(1 \leq T \leq 100)$

— the number of test cases.

Each test case starts with reading the integer

$n$

, the length of the secret string in that test case. The sum of

$n$

in all the test cases does not exceed

$2000$

.

Interaction Details

For each query, print the query in a line and flush the output. The query should be in the format mentioned above.

After each query, read an integer: the response from the judge.

$-1$

as a response from the judge means you did an invalid query. If you do any invalid query, your submission will fail with an arbitrary incorrect verdict.

After confirming the secret string in a test case, move on to the next test case if there is any, terminate your program otherwise.

To flush the output stream, you may use:

fflush(stdout)

in C/C++

stdout.flush()

in Python

Output

A sample interaction is given below for a test with two test cases, the first string is “001” and the second string is “11”.

>> 2
>> 3
<< ? 0
>> 0
<< ? 1
>> 5
<< ! 001
>> 2
<< ? 0
>> 0
<< ? 1
>> 0
<< ! 11

Another sample with a single test case and the secret string being “01”.

>> 1
>> 2
<< ? 0101
>> 2
<< ? 101011
>> -1

Here

>>

indicates what your program reads and

<<

indicates what your program writes. These symbols are here to make it easy to understand. You do not have to print such symbols from your program.

Notes

Notes

Binary strings are strings consisting of characters 0 and/or 1.

Substrings of a string are collections of one or more consecutive characters of that string in the same order they appear in the original string.

String A is said to be lexicographically smaller than string B if either string A is a prefix of string B or the first index where characters in the strings mismatch, character in string A has a lower ASCII value.


---
