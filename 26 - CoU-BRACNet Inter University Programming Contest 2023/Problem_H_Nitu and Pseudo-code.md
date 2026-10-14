# Nitu and Pseudo-code

**URL:** https://toph.co/p/nitu-and-pseudo-code  

---

Last night, Nitu came across the following pseudo-code. She understood that this method would take two integer values and a list of integers as input. She decided to implement this method in her preferred programming language and tried calling it with various sets of values. However, she encountered performance issues with her implementation for certain input values, as it did not execute within the expected timeframe. Can you assist her in implementing this pseudo-code?

1

FUNCTION CountLuckyNumbers(l, r, forbidden_list)

2

# Initialize a counter for lucky numbers

3

count_lucky_numbers = 0

4

5

# Loop through the range from l to r (inclusive)

6

FOR i FROM l TO r

7

# Convert the current number to a string

8

current_number = CONVERT_TO_STRING(i)

9

10

# Initialize a flag to determine if the number is allowed

11

is_allowed = TRUE

12

13

# Check if the current number contains any of the forbidden numbers

14

FOR EACH forbidden IN forbidden_list

15

# Convert the forbidden number to a string for comparison

16

forbidden_string = CONVERT_TO_STRING(forbidden)

17

18

# If the current number contains the forbidden number as a substring,

19

# Set the flag to false and exit the loop

20

IF current_number CONTAINS forbidden_string

21

is_allowed = FALSE

22

BREAK

23

END IF

24

END FOR

25

26

# If the current number is allowed, increment the lucky number count

27

IF is_allowed

28

INCREMENT count_lucky_numbers BY 1

29

END IF

30

END FOR

31

32

# Return the count of lucky numbers

33

RETURN count_lucky_numbers

34

END FUNCTION

Input

The input begins with an integer,

$T$

$(1 \leq T \leq 100)$

indicating the number of test cases.

For each test case:

The first line contains an integer,

$N$

$(1 \leq N \leq 100)$

which represents the size of the forbidden list.

The subsequent

$N$

lines contain integers, each representing an element in the forbidden list. Each of these elements falls within the range

$1$

to

$10^{18}$

.

Finally, there is a line containing two integers,

$l$

and

$r$

where both

$l$

and

$r$

are within the range of

$1$

to

$10^{18}$

.

Output

For each test case, please provide a single line of output in the following format:

$\texttt{Case \#}X\texttt{: }Y$

.

Here,

$X$

represents the test case number, and

$Y$

represents the result returned by the pseudocode.

Example


---

## Samples

### Sample Input 1
```
1
2
3 6
1 10
```

### Sample Output 1
```
Case #1: 8
```
