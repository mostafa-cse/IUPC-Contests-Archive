# Pop! Shop

**URL:** https://toph.co/p/pop-shop  

---

In a bustling medieval town, Arwa stumbled upon a lively carnival, its tents and banners fluttering in the breeze. Amidst the crowd’s chatter and laughter, she spotted a peculiar stall adorned with colorful balloons and mysterious prizes. Curiosity piqued, she approached the stall, where a wizened carnival master awaited. “Welcome, fair maiden, to the Pop! Shop” he proclaimed, gesturing towards a row of

$N$

balloons, each bearing its own enigmatic value,

$v_i$

.

“In this grand spectacle, ye shall wield special darts, each endowed with magical properties.“, the carnival master explained, “With these darts, ye can perform daring feats to pop the balloons and earn points.” He continued, “Be wary maiden, you can leave a balloon untouched, but each balloon can be popped only once. And the more points ye amass, the grander the reward!”. With a twinkle in her eye, Arwa listened intently as the carnival master detailed the ways she could wield her dart:

The Single Shot:

Arwa could aim her dart at a single balloon, popping it to earn its value

$v_i$

;

The Double Strike:

By targetting two adjacent balloons simultaneously - the

$i$

-th and

$(i+1)$

-th balloons - Arwa’s magical dart, when thrown, would unleash double darts popping the two balloons, earning the product of their values

$v_i \times v_{i+1}$

;

The Spectacular Sweep:

Should Arwa choose, she could aim her magical dart in a way that hits two different ballons

$i$

and

$j > i +1$

, earning the value

$v_i \times v_j$

. But she needs to keep two things in mind when using this move:

Sweep on balloons

$i$

and

$j$

can be performed only if all balloons between them, from

$(i + 1)$

to

$(j - 1)$

, had been popped earlier.

In case she decides to perform multiple sweeps, their ranges cannot be disjoint. Given Sweep 2 (involving balloons

$i_2$

and

$j_2$

) is performed after Sweep 1 (involving balloons

$i_1$

and

$j_1$

), Arwa needs to maintain

$i_1 > i_2$

and

$j_1 < j_2$

. This should be followed for all subsequent cases of sweeps.

Eager to embark on this daring adventure, Arwa faced the challenge: given the number of balloons and their associated values, she sought to devise a strategy to maximize her score. With determination in her heart, Arwa pondered her options, ready to seize the opportunity and claim the greatest prize the carnival had to offer.

Input

The first line of the input contains a single integer

$N (1 \leq N \leq 5000)$

denoting the number of balloons.

The following line contains

$N$

space-separated integers,

$v_i (-10^7 \leq v_i \leq 10^7)$

indicating the value associated with each balloon.

Output

Print a single integer denoting the maximum score.

Examples


---

## Samples

### Sample Input 1
```
3
4 5 3
```

### Sample Output 1
```
23
```

### Sample Input 2
```
7
9 5 15 20 13 17 30
```

### Sample Output 2
```
932
```
