# Living on a Prayer

**URL:** https://toph.co/p/living-on-a-prayer  

---

Tommy is an unlucky guy who used to work on the docks. He and his wife Gina are not financially stable, so life is very tough for them. And since there is a strike that has made the docks become closed, Tommy has no work to do and has started spending more time at home. Gina tries to keep Tommy busy at home so that Tommy doesn't feel upset. For that purpose, each day, Gina gives Tommy a string S and asks him to find the K-th palindromic sub-string of that string.

Tommy is too upset to play the game, but he doesn't want to break Gina's heart either, as they have got to hold on to what they've got, no matter how hard life's been. So Tommy came to you, a brilliant problem solver. Your task is to find Tommy's answers for each day, so that Gina's heart doesn't break.

Input

Input starts with an integer

$T$

(

$1 ≤ T ≤ 100$

), the number of days you have to help Tommy.

Each of the following

$T$

lines contains a string

$S$

(

$1 ≤ \text{Length of S} ≤ 10^4$

) and an integer

$K$

(

$1 ≤ K ≤ 10^8$

) separated by space, Gina's question for that day.

All strings in the input consist of uppercase English alphabets only (A to Z).

Output

For each day, print the

$K$

-th lexicographically smallest palindromic substring of string

$S$

in a single line.

If such a substring does not exist, print

$-1$

instead of the substring.

Example

Notes

A substring is a contiguous sequence of characters within a string. For example, "bc" is a substring of the string "abcda". Two substrings are considered different if they either start at or end at different positions in the string, even if their contents are the same.


---

## Samples

### Sample Input 1
```
6
BDROCKS 3 
AA 1
AA 2
AA 3
AA 4
ABACABA 7
```

### Sample Output 1
```
D
A
A
AA
-1
ABACABA
```
