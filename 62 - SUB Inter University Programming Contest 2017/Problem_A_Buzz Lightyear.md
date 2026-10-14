# Buzz Lightyear

**URL:** https://toph.co/p/buzz-lightyear  

---

Buzz Lightyear (character from famous movie ‘Toy Story’) is done with inter galactic battle and now in planet earth. His jetpacks are partly damaged in battle and needs help from ‘Sheriff Woody’. To reach Sheriff Woody, he must cross N buildings (located linearly in one direction from left to right) as Sheriff lives in rightmost (N+1)th building on a very top floor. Buzz Lightyear is afraid of stairs, so wants to reach the highest possible floor of Sheriffs building with his jetpacks. From each first N buildings, Buzz can collect fuel from it and use for his jetpack (only once) and make a jump which has two stages. If he choose to jump from i’th building and currently in t’th floor,

First his jetpack immediately fly him to t+u(i)’th floor of i+v(i)’th building,

Then he starts gliding downward (not vertically). During his gliding he may pass some buildings or not, before making any future jump (only from some building position but not in between) or touch the ground. While Buzz glides downward, his height decreases x(i) floor after passing each building (but never going beyond zero as the ground floor is at level zero).

While on the ground, Buzz can only walk from left to right and stop in front of any of the N buildings to make a jump. His target is to reach as high as possible on Sheriff's building. Now Buzz is on the ground and in front of first building (leftmost) and needs your help to calculate maximum floor he can reach at Sheriff's building.

For example, in the above image, N=12 and Sheriff lives on 13th building. Here, Buzz can jump from ground floor A of 1st building, then immediately fly to B’th floor of 3rd building, then glide down to C’th floor of 6th building then again jumping from here takes him to D’th floor of 9th building, thus finally reaching G’th floor of 13th building. But there is a better option where, he can walk to 2nd building and jump from P’th floor to Q’th floor of 8th building and glide down to R’th floor of G’th building.

Input

First line is the number of test cases T. Each case, starts with the number of building N. Then there are N lines where i’th of them describes i’th building with u(i), v(i), x(i) separated by space. Where, 1 <= T*N <= 1000000, 1 <= u(i),x(i) <= 100000, 0 <= v(i) <= 100000.

Output

For each test case, output case number followed by maximum floor of (N+1)th building where Buzz Lightyear can reach.

Example

Notes

Check sample IO for clarification.


---

## Samples

### Sample Input 1
```
2
5
3 6 8
9 1 6
3 0 10
3 2 8
7 3 4
5
6 4 7
9 2 2
10 3 10
10 0 3
6 3 6
```

### Sample Output 1
```
Case 1: 6
Case 2: 13
```
