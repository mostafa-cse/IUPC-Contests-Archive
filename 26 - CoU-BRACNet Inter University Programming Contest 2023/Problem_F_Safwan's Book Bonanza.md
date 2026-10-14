# Safwan's Book Bonanza

**URL:** https://toph.co/p/safwan-s-book-bonanza  

---

A grand book fair is taking place in your city, showcasing a dazzling array of books and publications. Safwan is a passionate book lover going to this book fair with a goal to buy as many books as possible.

There are

$n$

unique books available at the fair, each with its own price and publication id. Also, there are

$m$

publications participating in the fair, each offering a special

discount

on the total amount of the books you bought from them. Suppose you bought total

$2$

books with prices

$20, 30$

from publication 1 and publication 1 is offering a discount amount of

$60$

. Then you can buy these

$2$

books for free. If the books price are

$30, 40$

, then you can buy these books spending

$30+40-60=10$

amount.

Safwan will be asked

$q$

queries. In each query, he will be given an

amount.

To maximize his reading pleasure, he will always try to purchase the maximum number of books with the given amount. Would you like to help him?

N. B.

You can’t buy the same book multiple times.

Input

The first line of the input contains three integers

$1 \leq n \leq{10^6}$

,

$1 \leq m \leq{10^6}$

,

$1 \leq q \leq 10^5$

. Note that,

$m$

is always less than or equal to

$n$

and there is at least one book of every publication.

Each of the next

$n$

lines consists of two integers

$\texttt{price}$

$(1 \leq \texttt{price} \leq 10^{12})$

and

$\texttt{publicationId}$

$(1 \leq \texttt{publicationId} \leq m)$

of

$i$

-th book.

Next line contains an array

$\texttt{discounts}$

of

$m$

integers

$\texttt{discounts}[1], \texttt{discounts}[2], …, \texttt{discounts}[m]$

where

$0 \leq \texttt{discounts}[i] \leq 10^{18}$

means

$i$

-th publisher will offer this discount if you buy one or more books from their collection.

Each of the next

$q$

lines contains an integer which denotes the amount

$(0 \leq \texttt{amount} \leq 10^{18})$

of that query.

Output

For each query, print maximum number of books Safwan can buy with the given amount of that query. See the sample input output for more clarification.

Example


---

## Samples

### Sample Input 1
```
5 2 3
5 1
5 1
6 1
7 2
12 2
6 0
23
35
50
```

### Sample Output 1
```
4
5
5
```
