# Nothing’s more contagious than laughter

**URL:** https://toph.co/p/nothing-s-more-contagious-than-laughter  

---

Gotham, a city full of criminals. But there is one who is more than just a criminal. He brings pure madness and insanity upon the city and his legacy is

Death

!

It is another rough day for detective Jim Gordon! Joker escaped the Arkham Asylum this morning and gathered all the monsters created by Professor Hugo Strange aka The Philosopher in his place. Now he plans to destroy the whole city with his newly invented toxic gas. But somehow GCPD acknowledged that plan and Jim wants to stop him before he takes any steps.

Life of a police officer is pretty hard nowadays. They don’t get any free rides as they used to get in the past. To reach at the Joker’s place in time, Jim needs to use either public transport or pedestrian pathway which costs money! Jim doesn’t want to spend too much money so he needs your help to calculate the cheapest way to get there before Joker makes his first move.

In Gotham the transportation system is a bit different. There are N blocks numbered from

1 to N

in the city and they are connected with

N - 1

special bridges. A special bridge can have three types of bidirectional lanes.

Bus

Metro

Pedestrian Pathway

The definition of a route is a set of blocks connected by special bridge. Route can’t have a single block or be empty. Set of connected blocks means,

ith

block must be connected with

(i+1)th

block. For example if block A is connected with block B and block B is connected with block C then one possible route would be [A, B]. The others will be [B, C] and [A, B, C]. Here, [A, C] can’t be a route because A is not connected with C by a special bridge.

Route [A, B, C] can be represented as (A C) as both A and C are the endpoints of this route

.

Travel fare:

Bus:

Each Bus route will have a fare

F

for crossing each bridge in this route. For previous example, consider the route [A, B, C]. If the fare of this route is 5 then if you enter from A and leave at B the fare will be 5. If you leave at C the fare will be doubled to 10.

Metro:

Each metro route will have a fare

F (per unit distance)

. For the above example described in Bus section, let’s assume that the distance between A and B is 5 and the distance between B and C is 3. If the fare per unit distance is 1 then from A to B the fare will be 5 but from A to C it will be 8. You can’t jump off the bus or train unless you reached a Block.

Pedestrian pathway:

You may starting to wonder why should you pay when you walk! But this is Gotham and you can’t walk here peacefully. Walking between blocks is too risky. There can be smugglers, murderers and street fighters on the street. And you need to have lots of strength to survive. A bonus will be having a freeze gun! You can get a freeze gun in free of cost from any blocks. But the Helium solution cost money! What is the use of a freeze gun without Helium in it! Walking on the

ith

bridge will need

Hi

amount of Helium solution. You can buy Helium solution from the Wayne Enterprise store at any block. Cost of one unit Helium solution in

ith

block will be

Ci

. The Helium solution won’t last much longer. So, if you have any amount of spare Helium solution after reaching a block you must dump them immediately in the trash. If you want to walk again, you need to buy Helium again from that block.

You can also change Bus, Metro and use pathway at any block. You can safely assume that changing between routes or lanes is cost free. You can also assume that there will be no cycles, self loops and duplicate connections and it is always possible to go from one block to another if you have enough money. Now, Jim is at the police station and he needs know how much money should he take before start his journey to Joker’s place. What do you think? Can you help Jim and save millions of lives of Gotham?

There is one problem though. Joker has a special weapon which can destroy a route. So be careful!

Input

Input will start with a positive integer

T(T ≤ 10)

denoting the number of test cases. Each test case will start with a positive integer

N(2 ≤ N ≤ 105

), the number of blocks. The following line will contain

N

space separated integers where the

ith

integer

Ci(1 ≤ Ci ≤ 103

) denotes the cost of one unit Helium Solution at

ith

block. Each of the following

N - 1

lines will have four positive integer

A, B(1 ≤ A, B ≤ N and A ≠ B), L(1 ≤ L ≤ 103) and H(1 ≤ H ≤ 103)

where

A

and

B

are the block numbers connected with a special bridge,

L

is the length of the bridge and

H

is the amount of Helium solution needs to cross this bridge by walking. The following line will have a positive integer

R(1 ≤ R ≤ 105)

denoting the number of routes. Each of the following

R

lines will have four positive integers

T, S, E(1 ≤ S, E ≤ N and S ≠ E) and F(1 ≤ F ≤ 103)

where

T

is the route type,

S

and

E

are the block number of the two end points of the route and

F

is the amount of fare. There will be two types of routes:

T = 1 means Bus

T = 2 means Metro

Route from

S

to

E

(or vice versa) means all the connected blocks from

S

to

E

are included in this route. Also you can start your journey from any of the block that includes in this route.

Remember that pedestrian pathway will not be counted as a route because one can walk from any block to it’s all connected blocks!

The following line will have a positive integer

Q(1 ≤ Q ≤ 105)

denoting the number of queries. Each of the following

Q

lines will have two positive integers

T

and

K

where

T

is type of the query. There will be two types of queries:

T = 1 means destroy the

Kth(1 ≤ K ≤ R)

route(if it’s not destroyed yet!)

T = 2 means output the minimum cost from police station to Joker’s place(

Kth

block)

1 ≤ K ≤ N

.

You can safely assume that for each test case the summation of the size of all routes will be no more than 5×105. Here size of a route means the number of blocks it has. The police station will always be at block number

1

.

Output

For each test case the first line will be the case number in the format

“Case #t:”

without the quotes. Here

t

is the case number starting from

1

. Then for each query type

2

, output the minimum cost from police station to Joker’s place in separate line.

Example

Notes

Use faster I/O as the dataset can be huge

.


---

## Samples

### Sample Input 1
```
1
3
1 2 1
1 2 4 5
2 3 3 2
2
1 1 3 2
2 1 2 1
5
2 3
1 1
2 2
1 2
2 3
```

### Sample Output 1
```
Case #1:
4
4
9
```
