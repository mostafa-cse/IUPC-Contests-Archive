# Party Lights

**URL:** https://toph.co/p/party-lights  

---

The famous mafia leader of Byteland, Don Mukuvich, is hosting a party and he has decided to decorate the party hall with colorful lights. Why, you may ask? Well, because he can!

However, since he is not just any ordinary man, his choices of colors are extra-ordinary too. Instead of going for typical monochrome Red, Green or Blue colors, his lights can be of any color and each color is formed by a combination of Red, Green and Blue values, each ranging from 0 to 127. Why not 255? It's because he doesn't like bright lights. We identify these three values as the RGB color code for the composite color. For example, the color code for purple is (R: 127, G: 0, B: 127).

As you may have known, Don Mukuvich has a tremendous passion for sequences. He tries to put everything in a sequence. He performs his daily chores in a sequence, robs local banks in a sequence, hunts down rival mafia leaders sequentially, or, even arrange party lights in a sequence. He has been thinking about some interesting property to go with the sequence of lights.

The lights are arranged in a sequence, as expected. Don Mukuvich defines the color distance of two lights as the maximum difference between Red, or Green, or Blue color components. Now he defines the color deviation of a subsequence of lights as the maximum color distance between any two lights in that subsequence.

Since Don Mukuvich does not like too much deviation in colors, he wants to find out a subsequence of K lights from a given sequence of N lights with smallest possible color deviation rating. Sad for you though, he is now holding you at gun point, you must write a program for him to find his desired rating.

Input

First line of input contains an integer

$T$

(

$1 \le T \le 16$

), the number of test cases. For each test case, first line contains two integers

$N$

and

$K$

(

$2 \le K \le N \le 100000$

). Each of the next N lines contains three integers

$R$

,

$G$

,

$B$

(

$0 \le R, G, B \le 127$

) indicating the red, green and blue component value of a light color.

Output

For each case, print the minimum color deviation rating for a subsequence of

$K$

lights.

Example

Notes

Elements of a subsequence doesn’t have to be consecutive, but they must maintain the order as appeared in the original sequence.


---

## Samples

### Sample Input 1
```
2
5 3
6 6 4
6 2 7
3 1 3
4 1 5
6 2 6
2 2
1 3 2
2 6 4
```

### Sample Output 1
```
2
3
```
