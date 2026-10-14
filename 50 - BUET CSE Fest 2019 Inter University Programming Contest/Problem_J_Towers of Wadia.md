# Towers of Wadia

**URL:** https://toph.co/p/towers-of-wadia  

---

Admiral General Aladin has

$n$

watchtowers on a desert of People's Republic of Wadia. One of those watchtowers is the headquarter there. On a few days back, something

aladin

(bad) happened. A fighter plane from a neighbouring country bombarded on the watchtowers and some towers were destroyed. No one wants to talk about it and let the Admiral General know about it for some obvious reasons. So, you, the head of security of the country, didn’t really get to know which towers were destroyed. However, as an

aladin

(good) citizen, you want to figure out the expected area covered by all the remaining towers. Area covered by some watchtowers is the area of the convex hull covering those watchtowers.

You know that in total

$k$

towers were destroyed. You also know that the indestructible headquarter wasn’t destroyed and fortunately, it’s still

inside

the convex hull (not on the edge of the convex hull) formed by the remaining watchtowers.

Input

The first line of the input will be

$n$

(

$4 ≤ n ≤ 100$

), the number of watchtowers before the

aladin

(bad) incident happened. The next line will have two space separated integers

$x_0$

and

$y_0$

, the position of the headquarter. Each of the next n-1 lines will contain two space separated integers which are the positions of the other watchtowers. The next line contains a number

$k$

(

$0 ≤ k ≤ 10$

).

Absolute value of all the coordinates will be no more than 1000.

It is guaranteed that it will be possible to find at least one set of

$n-k$

towers so that the convex hull formed by those points will have the headquarter

inside

it. Also, no three towers will be on the same line.

Output

Print one line, the expected area of the convex hull formed by the remaining watchtowers. Error less than

$10^{-6}$

will be ignored.

Example


---

## Samples

### Sample Input 1
```
5
1 1
0 0
0 3
3 0
3 2
1
```

### Sample Output 1
```
4.500000
```
