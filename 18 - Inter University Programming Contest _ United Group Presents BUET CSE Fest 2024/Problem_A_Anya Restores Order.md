# Anya Restores Order

**URL:** https://toph.co/p/anya-restores-order  

---

Anya doesn’t like disorderliness, everything she has needs to be in order and complete. Today, she went to a store and bought some powerballs also called lottery balls. The balls are small in size and have a number written on it. Anya asked the storekeeper to give her a complete package of balls with consecutive numbers from

$1$

to

$B$

meaning she wanted

$B$

balls each with a unique number and no numbers missing between them. Then, she asked for them to be packed into tubes, each containing the same number of balls, arranged in sequential order. A complete and organized package!

The store keeper packed the balls and delivered them to Anya. When she opened the packages, she was speechless! It’s all wrong! Not only the packages are unevenly filled with different numbers of balls, the balls are not in sequential order too! To make things worse there are some balls missing and there were even some that probably belonged to other orders. What a disaster!

Despite the mess, she is determined to restore order. She decides to take two tubes of balls and transfer all of the balls into another one and discard the empty one. As she merges the tubes, she will occasionally ask you to help her find any missing balls that should be numbered lower than the highest-numbered ball in the tube. If there are multiple missing balls you report the smallest one. If there are no missing balls, then report that to her by saying

$complete$

! Please note that due to the same packaging error, there may be multiple balls of the same number in a tube (that shopkeeper will pay for this).

Help Anya to attain her order.

You are given

$N$

array indicating the tubes. Each array

$A_i$

has arbitrary size

$M_i$

contains some positive integers

$A_{ij}$

representing the balls. You will be given

$Q$

queries. There will be two type of queries

$1\ i\ j$

Append array

$A_j$

after array

$A_i$

and delete the array

$A_j$

.

It is guaranteed that there is an array with id

$i$

and

$j$

at the time of this query.

$2\ i$

Output the missing number ball of the array

$A_i$

according to the description. It is guaranteed that there is an array with id

$i$

at the time of this query.

Input

The first line of input will have a positive integer

$T$

, the number of independent test cases.

Each case will begin with two positive integer

$N,Q$

, the number of arrays and the number of queries. Then the next

$N$

lines each will start with

$M_i$

indicating the size of the array followed by

$M_i$

integers

$A_{ij}$

indicating the elements of the array.

Next

$Q$

lines indicates queries each of them in the form of mentioned previously

$1\le T\le 10^5$

$1\le N\le 10^5$

$1\le M_i\le 10^5$

$1\le A_{ij}\le 10^9$

Sum of

$M_i$

over all tests cases

$\le 10^6$

Sum of

$Q$

over all tests cases

$\le 2\times10^6$

Each query will start with a integer

$1\le t\le 2$

For

$t=1$

it will follow

$i\ j$

,

$1\le i,j\le \textbf{n}$

For

$t=2$

it will follow

$i$

,

$1\le i\le \textbf{n}$

Output

For each query of type 2, output the answer in a new line

Example


---

## Samples

### Sample Input 1
```
1
4 7
4 2 4 1 2
3 5 3 7
2 6 8
5 3 1 5 1 10
2 1
1 1 2
2 1
1 3 1
2 3
1 4 3
2 4
```

### Sample Output 1
```
3
6
complete
9
```
