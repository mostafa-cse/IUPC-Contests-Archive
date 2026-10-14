# Remember the Name...

**URL:** https://toph.co/p/remember-the-name  

---

There's a famous song written by Mike Shinoda, which has these lines:

This is 10% luck, 20% skill, 15% concentrated power of will, 5% pleasure, 50% pain, and a 100% reason to remember the name...

This problem is about luck and skill. You are moderating a competition. There are N competitors. And, there are Q new competitors yet to come. Each of them is very competitive. They follow the exact same procedure. Each of these contestants first comes to you, asks you exactly how many competitors are compatible with him/her (let's denote this number as comp(qi) for the i-th new competitor), and then joins the competition.

But there's a little problem with the new competitors. If the number of compatible competitors exceeds the tolerance factor (let Ti denote it) of a new competitor, then he/she thinks that there are too many compatible competitors and he/she doesn't join the competition.

Each competitor has a luck factor Li and a skill factor Si. The number comp(qi) denotes the number of compatible competitors (who has already joined the competition before the i-th new competitor) with the i-th new competitor.

Let's say the luck factor and skill factor of a competitor is L and S, respectively. Then he/she will be compatible with the i-th new competitor if:

(L - Li)2 + (S - Si)2 ≤ Xi2

... where Xi is the satisfaction factor of the i-th new competitor.

Your job is to answer every new competitor that how many compatible competitors with them there are already and whether it's within the tolerance limit or not.

Input

The first line will contain two integers

N

and

Q

(1 ≤ N, Q ≤ 105), the number of preexisting competitors and the number of new competitors to join the competition. The next two lines both will contain N integers, the first one will contain the luck factors and the second line will contain the skill factors. The i-th integer of both lines denotes the i-th competitor.

The next Q lines will contain four integers

Li

,

Si

,

Xi

(1 ≤ Li, Si, Xi ≤ 105) and

Ti

(1 ≤ Ti ≤ 103) each. The i-th line denotes the luck factor, skill factor, satisfaction factor and tolerance factor of the i-th new competitor, respectively.

Output

You will print Q lines that contain one integer each, where the i-th integer denotes the number of compatible competitors with the i-th new competitor.

If the number of compatible competitors exceeds the tolerance factor for that competitor, print "Too Many!!!" without the quotes.

Example


---

## Samples

### Sample Input 1
```
7 6
0 2 2 0 1 0 0
0 0 2 2 1 0 0
1 0 1 7
0 1 2 6
0 0 2 7
2 2 2 6
1 1 5 10
1 1 5 10
```

### Sample Output 1
```
5
6
Too Many!!!
4
10
Too Many!!!
```
