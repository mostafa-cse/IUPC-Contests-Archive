# Search Engine of Nicola

**URL:** https://toph.co/p/search-engine-of-nicola  

---

Being frustrated with captcha of popular search engine Koogle, The great programmer Nicola decided to make her own search engine. In her search engine, all information of the world can be considered as a string

$S$

where each topic of searching is a substring of

$S$

. There is a special feature in Nicola’s search engine: while typing, a user is notified with number of different possible topics based on what she has typed so far. In other words, when a user types a string

$X$

, the search engine shows

$|X|$

numbers one after another such that

$i^{th}$

(

$1\le i \le |X|$

) number shows the number of

unique

substrings of

$S$

which has

$X_{1 \dots i}$

(i.e. prefix of

$X$

with length

$i$

) as prefix. As a search engine, it has to handle plenty of such

$X$

(i.e. there are

$Q$

queries of

$X$

). This problem is very easy for Nicola but she is currently busy. Can you help her by solving it?

Input

First line of input contains the number of test cases,

$T$

(

$1 \le T \le 10$

).

Each test case begins with a string

$S$

(

$1 \le |S| \le 10^5$

) consisting of lowercase English Letters. In the next line, there is an integer

$Q$

(

$1 \le Q \le 10^5$

) denoting the number of query strings. Each of the next

$Q$

lines contains a query string

$X$

consisting of lowercase English letters (

$1 \le |X| \le 10^5$

).

Over all test cases,

$\sum |S| \le 3\times 10^5$

,

$\sum |X| \le 5 \times 10^5$

.

Output

For each query string

$X$

, output an array of integer of length

$|X|$

, where

$i^{th}$

(

$1 \le i \le |X|$

) number of the array corresponds to the number of substrings of

$S$

of current test case having

$X_{1 \dots i}$

as a prefix.

Example

Notes

For Query 1:

Substrings with prefix “a“: ”a” (Appeared multiple times but counted only once), ”ab”, “aba”, “abac”, “abacb”, “ac”, “acb”

Substrings with prefix “ab“: ”ab”, “aba”, “abac”, “abacb”

No substring with prefix “abc“


---

## Samples

### Sample Input 1
```
1
abacb
3
abc
ba
acb
```

### Sample Output 1
```
7 4 0 
4 3 
7 2 1
```
