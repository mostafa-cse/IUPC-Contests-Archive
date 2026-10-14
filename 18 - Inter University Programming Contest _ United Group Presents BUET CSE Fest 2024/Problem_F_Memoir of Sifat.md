# Memoir of Sifat

**URL:** https://toph.co/p/memoir-of-sifat  

---

This is an interactive problem.

Sifat has got a binary string of length

$N$

and he wants to play with you. He will keep the string hidden, but not the integer

$N$

. To play with him, you will serially ask him some queries. In each query, you will ask him with a binary string of your choice and he will reply whether your given string is a subsequence of the hidden string.

Sifat will not accept more than

$1024$

queries, however he is always honest.

A subsequence of a string is a string which can be obtained by removing several (possibly zero) characters from the original string without changing the order of characters.

Input

In the first line of input, Sifat will provide you an integer

$N$

$(1 \le N \le 1000)$

.

Then you start the interaction with your queries.

For each interaction, you should print a line consisting of your query binary string

$S$

. Length of

$S$

must not exceed

$N$

and it must be

non-empty

. Each query will be replied with a single line.

If

$S$

exactly matches with the hidden string, Sifat will reply with “

Correct

”.

Otherwise, if

$S$

is a subsequence of the hidden string, Sifat will reply with “

Yes

”.

Otherwise, Sifat will reply with “

No

”.

Your program should get the “Correct” reply within

$1024$

queries.

You must terminate your program immediately once you get the “Correct” reply. Otherwise you may not get the accepted verdict.

If you keep asking more than

$1024$

queries, you may get “Wrong answer”/”CPU Limit Exceeded”/”Runtime Error”. Similarly, if your interaction is malformed, you may get “Wrong answer”/”CPU Limit Exceeded”/”Runtime Error”.

After outputting each line, don't forget to flush the output.

For example:

fflush(stdout) in C/C++;

System.out.flush() in Java;

sys.stdout.flush() in Python;

flush(output) in Pascal;

Output

There is no more explicit output apart from the interaction in this problem.

Notes

Sample interaction: The hidden string in this case is

$0110$

.

Line starting with

$>$

denotes Sifat’s line, line starting with

$<$

denotes your provided line.

$> 4$

$< 010$

$> Yes$

$< 0101$

$> No$

$< 011$

$> Yes$

$< 0110$

$> Correct$


---
