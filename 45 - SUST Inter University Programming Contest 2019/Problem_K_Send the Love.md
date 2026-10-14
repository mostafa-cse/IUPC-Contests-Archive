# Send the Love

**URL:** https://toph.co/p/send-the-love  

---

Yesterday Akhtaruzzaman Mridha (Akhter mia) was stealing mango from a tree near Asad Gate. And suddenly the branch he was sitting on, broke, and he fell. But luckily a strong girl named Nadia Tasnim was below the tree. She caught Akhter mia and saved him from breaking his neck. That was it for Akhter mia! Instant love! Next thing he could remember is he saying the girl “I Love You”. Somehow Nadia found that very cute and accepted his Love. Now they are a couple. Sweet eh?

Since his childhood, Akhter mia has dreamt of sending love emoji to his girlfriend. But after Nadia came into his life, something really frustrating started to happen. As Nadia likes to roam around in the city a lot, sometimes she goes out of network, which results in Akhter mia not being able to send her any love emoji. Akhter mia was very sad that he cried for twenty whole days. Then he decided to put those tears back into his eyes and do something about the situation.

Being a very smart individual, Akhtar mia developed an app along with networking hardware called Lovesphere. Lovesphere has a spherical coverage area. We call two Lovespheres connected if the two Lovespheres have an intersection between them. Also, connectivity is transitive (If Lovesphere

$A$

and

$B$

are connected, and Lovesphere

$B$

and

$C$

are connected. Then Lovesphere

$A$

and

$C$

are also connected).

If two individuals use his app from the same Lovesphere or from two connected Lovespheres, they can send love emoji to each other without any problem.

But as the city mayor had a crush on Nadia, so he wanted Akhter mia to fail. So he permitted him some weird coordinates in the sky, where Akhter mia can set up his Lovesphere(s).

The city they live in has a rectangular shape with corners at

$(0,0)$

,

$(x,0)$

,

$(x,y)$

,

$(0,y)$

. Akhter mia lives in his lab at

$(0,0)$

and never goes out. On the other hand, Nadia is always roaming around in the city. As none of them can fly, they always stay on the ground and inside the city.

Akhter mia got permission for setting up

$N$

Lovespheres. Now Akhter mia wants the radius of the coverage of all the Lovespheres to be same. Now he wants to know the minimum radius r he can set for all of the Lovespheres, such that, No matter wherever Nadia is, he can always send love emoji to her.

Input

The first line of the input will be two integers

$x$

,

$y$

(

$0 \le x, y \le 10^5$

), representing the corner of the rectangle opposite to the origin. Then next line will contain an integer

$N$

(

$1 \le N \le 10^3$

) representing the number of Lovespheres he was permitted by the mayor. Then each of the next

$N$

lines will have three integers

$x_i$

(

$0 \le x_i \le x$

),

$y_i$

(

$0 \le y_i \le y$

),

$h_i$

(

$0 \le h_i \le 10^5$

) representing the coordinates and the elevation where he is permitted to place Lovespheres.

Output

Print a single real number

$r$

(rounded to two digits after decimal) – the minimum radius he needs to set for all the Lovespheres.

Examples


---

## Samples

### Sample Input 1
```
2 2
2
0 1 1
2 1 1
```

### Sample Output 1
```
1.73
```

### Sample Input 2
```
2 2
2
0 0 1
2 2 1
```

### Sample Output 2
```
2.24
```
