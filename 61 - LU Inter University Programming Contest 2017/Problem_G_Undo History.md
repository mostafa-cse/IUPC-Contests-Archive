# Undo History

**URL:** https://toph.co/p/undo-history  

---

Robin is using a peculiar text editor to write a sequence of lines of text. The editor consists of three parts: a results window, a text buffer and an undo history. More details about the three parts follow.

The results window contains a sequence of strings: the lines of text you already wrote. Initially, the results window is empty.

The text buffer contains a string: the line you are writing at the moment. Initially, the string in the text buffer is empty.

The undo history contains a sequence of strings: all the past states of the text buffer. Initially, the undo history contains a single element: an empty string.

You are given a sequence of lines. Robin would like to print the contents of these lines into the results window. (At the end, the sequence of strings stored in the results window must be precisely equal to the lines. Order of elements matters.) Additionally, Robin would like to do so as quickly as possible. He is able to take the following actions:

Robin may type a lowercase letter. The letter is appended to the text buffer. The new text buffer is then added as a new element of the undo history. (For example, if the text buffer currently contains "do", then pressing 'g' changes the text buffer to "dog" and then stores "dog" into the undo history.)

Robin may press Enter. When he does so, the current content of the text buffer is printed to the results window as a new line, after the lines that were printed earlier. The text buffer remains unmodified. (For example, if the text buffer contains "dog" and Robin presses Enter, "dog" will be appended to the results window, and the results buffer still contains "dog".)

Robin may use two mouse clicks to restore any entry from the undo history to the text buffer. This operation does not modify the undo history.

Return the minimum total number of button presses (keyboard and mouse) that Robin needs to print all the given lines into the results window.

Input

Input starts with a positive integer T, denoting the number of test cases (T < 200). Each test case starts with an integer n, the number of strings in that case (1 <= n <= 100). This line is followed by n lines, each containing a string of no more than 50 characters. Each element of a string will contain only lowercase letters (‘a’ – ‘z’).

Output

Print the minimum number of operations required for the given task. See the sample outputs for the exact format of the output.

Example

Notes

Explanation

Case 1:

Type 't'. The text buffer now contains "t", and the undo history now contains "" and "t".

Type 'o'. The text buffer now contains "to", and the undo history now contains "", "t", and "to".

Using six more keypresses, type the letters in "morrow". The text buffer now contains "tomorrow" and the undo history contains all prefixes of "tomorrow". The results window is still empty.

Press Enter. The results window now contains one string: "tomorrow".

Click the mouse twice to restore "to" from undo history.

Using another three keypresses, type the letters in "day".

Press Enter. The results window now contains "tomorrow" and "today", in this order, and we are done.

The total number of button presses was 8 (typing "tomorrow") + 1 (Enter) + 2 (mouse) + 3 (typing "day") + 1 (Enter) = 15.

Case 2:

After typing "a" and pressing enter, we need to restore the empty string (which is always present at the top of the undo buffer) before typing "b".

Case 3:

There are times when it is not necessary to use the undo history at all.


---

## Samples

### Sample Input 1
```
5
2
tomorrow
today
2
a
b
4
a
ab
abac
abacus
3
absolutely
abs
absolute
5
pyramid
sphinx
sphere
python
serpent
```

### Sample Output 1
```
Case #1: 15
Case #2: 6
Case #3: 10
Case #4: 17
Case #5: 39
```
