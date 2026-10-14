# Biswa and Morse Code

**URL:** https://toph.co/p/biswa-and-morse-code  

---

Biswa wanted to know what the heck Morse Code is and here’s what he found out on the internet -

Morse code is a character encoding scheme used in telecommunication that encodes text characters as standardized sequences of two different signal durations called dots and dashes or dits and dahs. The International Morse Code encodes the 26 English letters A through Z, some non-English letters, the Arabic numerals and a small set of punctuation and procedural signals (prosigns). There is no distinction between upper and lower case letters. Each Morse code symbol is formed by a sequence of dots and dashes. The dot duration is the basic unit of time measurement in Morse code transmission. The duration of a dash is three times the duration of a dot. Each dot or dash within a character is followed by period of signal absence, called a space, equal to the dot duration. The letters of a word are separated by a space of duration equal to three dots, and the words are separated by a space equal to seven dots.

Time to hear about the cool project Biswa has been working on lately. It’s called - Online Love Guru. It’s an online platform where users ask their love related questions anonymously. The system generates the response to the questions of the users using some “Machine Learning” approach and send back to them. This online platform is now one of the most used one on planet earth and guess what, the aliens want to use this as well!

But he wants to do something interesting for the aliens. He wants to send them the answer to their queries using Morse Code. He now has a list of answers that can cover all possible questions. And he wants to transmit each answer in most efficient way. For each question, he’ll first send his Morse Code encoding for each character used in that answer and then transmit the answer using those Morse Code encodings. He firmly believes that it is potentially possible to find more efficient Morse Codes than the conventional ones for each of the answers in his list. The efficient Morse Codes will require less duration to transmit the answer.

Given the list of answers, can you write a program to generate the most efficient Morse Codes for each answers?

Constraints:

Each answer contains one or more words

Each word contains English letters (‘a’-’z’, ‘A’-’Z’) and numbers (‘0’ - ‘9’)

Each word contains no more than 20 characters

Each answer contains no more than 100 words

There is no distinction between upper and lower case letters

Efficient Morse Code should also be prepared using dots and dashes and will have non-zero length

All the letters and numbers will be present at least once in an answer

Input

First line of the input will specify the number of answers -

$N$

(

$1 ≤ N ≤ 100$

). Then there will be

$N$

subsequent lines with one answer each.

Output

Output should contain the proposed efficient Morse Codes for letters A to Z followed by the Morse Codes for numbers 0 to 9. If there’s multiple set of most efficient Morse Codes, you can output anyone from there.

Example


---

## Samples

### Sample Input 1
```
1
Pack my box with five dozen liquor jugs 0123456789
```

### Sample Output 1
```
-.-.
.--.
....-
-..-
.-
.-.-
..--
---
-
.....
-...
.-..
..-.
--.
.
...-
-.-
.--
....
-..
..
.-.
..-
--
...
-.
--.-
...--
-.--
.---
......
-....
.-...
..-..
--..
...-.
```
