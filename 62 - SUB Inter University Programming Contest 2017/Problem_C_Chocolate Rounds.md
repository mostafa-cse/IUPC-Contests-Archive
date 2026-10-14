# Chocolate Rounds

**URL:** https://toph.co/p/chocolate-rounds  

---

In a magical Victoryland, there is a princes named “Rowshan” who loves chocolate bar a lot and don’t like to share the bars with anybody. She is so much fond of chocolate bars that even if anyone presents her with thousands of chocolate bars she would eat all of the bars to her heart’s content. However, she follows a simple rule to enjoy each bar uniquely. Even though she takes several rounds to finish all of the chocolates but the rule is same for all of the rounds. In first round, she numbers the bars serially starting from 1. Then she starts eating from the first bar. Although, in every round she never eats any bar whose position number is the multiple of the position number of any eaten bar except the first one of that round. For example, if there are 6 bars then she would eat 1, 2, 3 & 5 numbered bars in her first round as bar numbered 4 and 6 are the multiple of the 2nd bar. After each round, she numbers the remaining bars from the beginning (e.g.: from 1) and repeats the rounds according to the rule.

Recently, her brother “Raheel” have decided to visit her with a lot of chocolates and have decided to come up with an idea to share the chocolates by any means. Consequently, “Raheel” has asked her sister to stop following this process so that he may eat few chocolates. As a response, “Rowshan” has promised her brother to share the chocolates if and only if he could guess the number of rounds she would need to finish all of the chocolates. As a result, after searching a lot, “Raheel” comes to YOU! Now, you have to determine the number of rounds that “Rowshan” would need for any given number of chocolates.

Raheel cites an example for you:

If there are 6 chocolates numbered as 1, 2, 3, 4, 5 and 6 initially then,

In the 1st Round she will eat bar number: 1, 2, 3, 5

Whereas, In the 2nd Round she will eat: 1, 2 (As remaining bar numbered 4 and 6 of the first round became number 1 and 2 in the second round).

Now, could you please help “Raheel” to determine the number of rounds that “Rowshan” would need for a given number of chocolates to eat?

Input

In the first line of the input, there will be an integer number N (1 < n <= 1234567) denoting the number of test cases. Then n lines follow where each of them is a non negative integer number C denoting the number of chocolates that “Rowshan” has. C can be as long as 10^7.

Output

For each test case you have to print the number of rounds that “Rowshan” needs to finish all of the chocolates. The output should be in this format “Case N: X” without the quotation mark where X denotes the number of rounds and N denotes the number of test case.

Example

Notes

You should use faster I/O methods.


---

## Samples

### Sample Input 1
```
3
2
6
25
```

### Sample Output 1
```
Case 1: 1
Case 2: 2
Case 3: 4
```
