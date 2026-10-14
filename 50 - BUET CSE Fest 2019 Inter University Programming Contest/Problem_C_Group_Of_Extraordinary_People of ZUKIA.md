# Group_Of_Extraordinary_People of ZUKIA

**URL:** https://toph.co/p/group-of-extraordinary-people-of-zukia  

---

I am sure all of you are familiar with a specific group of people. For your own safety and so that this problem sees the light in the contest they shall be referred to as ‘Group of Extra Ordinary People’ of ZUKIA. Unfortunately ZUKIA was always been an underdog in this field. They were always out shined by their counterparts from other Institutions around the country.But in recent years they are moving up the ladders. In this problem you are going to help the ambitious extraordinary people from ZUKIA.

What is the one and only aspiration in the life of such an extraordinary person? Its a seat in the high tables - to become a leading figure who will be respected by fellow extraordinary people and will have authority over the ordinary people. And then if they manage to save some extra time, buy motorcycles from gifts - or rather they would call offerings - from the ordinary people. Now in order to move up in the world they need to devote their life and body to the current existing leaders during events and in private meetings held in ZUKIA. You are given an instance of such an event.

There is a list of N people from the group of extraordinary people given to you. Each person has an unique id from [1...N] and the current ‘Extraordinary Value’ in range [1...1e9]. You are organizing an event for them with people from this list. In order to do that you will choose persons with id number [L...R] and then those persons who will go to the said event. In the event they will always form a line according to their rank. For your convenience you may think that they will create a non-increasing line from the highest valued person to the lowest valued person. In this line each person will get a satisfaction index according to what he thinks he has achieved in his otherwise insignificant life. As they want to be deflowered by their superiors they want their immediate neighbors to be as high valued as possible and that gives them a satisfaction value.

Your job is, given a lot of queries of range, find the total satisfaction for each of the queries. The way it works is that suppose you are given a range from [L..R]. Then after rearranging according to ‘Extraordinary Value’ let their id be B(0), B(1), … B(R-L).

Concretely, for the ith person on the list, left Happiness = abs(A(B(i)) - A(B(i-1))),

and right Happiness = abs(A(B(i)) - A(B(i+1)))

And satisfaction of ith person = max( Left Happiness, Right Happiness)

For leftmost person in the line, Left Happiness = 0, and For rightmost person in the line, Right Happiness = 0.

Your job is, given a lot of queries of range, find the total satisfaction for each of the queries. Total satisfaction of a single query is defined as the sum of the satisfaction of all the people in the query.

Input

First line will contain the number of test cases T.

Then there will be two numbers N and Q denoting the number of total people and the number of queries.

Then there will be N numbers: i’th of which represents the ‘Extraordinary Value’ of person i in the organization.

Then there are Q queries. Each of the query is in the form of two numbers L and R. For each of these queries you have to output the total satisfaction index in the case that people from [L...R] are sent to the event.

1 <= T <= 5

1 <= N, Q <= 100000

1 <= Ai <= 1000000000

1 <= L <= R <= N

Output

For each case print a line “Case #:”. Then in the next Q lines print the answers to the queries. I’th line should contain answer for i’th query.

See the sample input output for clarification.

Example

Notes

For the first query in the sample, the values are [9, 1, 3].

After sorting according to their extra-ordinary value [9, 3, 1].

1st person's satisfaction = abs(9 - 3) = 6

2nd person's satisfaction = max(abs(3 - 9), abs(3 -1)) = 6

3rd person's satisfaction = abs(1 - 3) = 2.

So total satisfaction for this query = 6 + 6 + 2 = 14.


---

## Samples

### Sample Input 1
```
1
5 5
9 1 3 10 6
1 3
2 5
1 5
5 5
3 5
```

### Sample Output 1
```
Case 1:
14
13
12
0
11
```
