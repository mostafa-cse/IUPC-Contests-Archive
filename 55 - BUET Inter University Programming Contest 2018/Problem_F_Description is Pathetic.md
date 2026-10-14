# Description is Pathetic

**URL:** https://toph.co/p/description-is-pathetic  

---

Do you know what is the hardest part of creating a problem? Thinking and writing the description. You have to think a lot how you should represent a story so that the contestants can easily understand the problem. A problem is read by at least 3 or 4 persons before the contest starts to make sure that there is no confusion in the problem statement. But, alas!!! We still get clarifications! So, what I decided for this problem is, there will be no story and the problem should be very straight forward. Let’s solve the following problem then:

You will be given an array of strings - A. Now you will have to implement two types of operations:

Insert: Append a new string X in array A

Query: You will be given two strings - P & S. You have to answer how many strings in A has both P as prefix and S as suffix together.

Input

The first line of each input file will contain two integers - N & M, where N denotes the number of strings in the array A at the initial state and M denotes the number of queries. Next N lines contain a string which is an element of array A. Next M lines can be one of following format of query:

1 X - This type of query describes the INSERT operation where X is a string

2 P S - This type of query describe the QUERY operation where P denotes the query prefix and S denotes the query suffix.

Costraints:

1 <= N, M <= 100000

1 <= |X|, |P|, |S|, |Ai| <= 100000

The summation of lengths of all the strings in a test case will not increase 1000000. Each string contains only lowercase alphabet.

Output

For each type of query 2 print the answer in seperate lines.

Example


---

## Samples

### Sample Input 1
```
3 5
a
bab
abcb
2 a a
2 ba ab
1 bacb
2 b b
2 ba ab
```

### Sample Output 1
```
1
1
2
1
```
