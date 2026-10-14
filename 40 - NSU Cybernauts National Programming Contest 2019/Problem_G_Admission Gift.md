# Admission Gift

**URL:** https://toph.co/p/admission-gift  

---

During admission exams in the city of RR (Royal Royal city), the students of RR University of Engineering and Technology have decided to open a shop to help the newcomers. In this shop, if you ever buy an item of value

X

, you can get this item for free if you want to buy it again in the future. Moreover, the items in the shop can be combined. If you combine two items of values

A

and

B

, you will gain a new item of value

C

. The shop contains an unlimited amount of items of all values.

Now, seeing how brilliant you are, the students of the university want to play a game with you. They told you that they want you to make

N

number of items. They will give you

Vi

(value of the

i

-th item you have to make), and for each

Vi

, you can buy some items from their shop to make the item of

Vi

value. If you can make all of the

N

items by being charged at most

4

times and buying items from the shop at most

18000

times, you will get all of these items as gifts and you don't have to pay anything! Are you up for the task?

For example;

Imagine you were told to make the item of value 5 first. You can buy an item of value 5 from the shop and be done with it. You have been charged one time so far and have bought only one item so far.

Then you are told to make an item of value 7. You can just buy an item of value 7 from the shop. In that case, you have been charged twice so far (once for the item of value 5 and once for the item of value 7) and have bought two items so far.

For the third item, you are told to make an item of value 12. You can buy an item of value 5 and an item of value 7 from the shop. Since you have already bought items of value 5 and 7 before from the shop, you won't be charged again for these items. So, you have been charged twice so far and have bought four items so far.

If the game ends at this point, you have won! An example interaction of this scenario can be found in the output section.

Since this is an interactive problem,

don't forget to flush

your output while communicating with the driver program (the shop). You may use fflush(stdout) in C++, system.out.flush() in Java, stdout.flush() in Python to flush the output. If you use some other programming language, consult its documentation.

Input

Interaction Details

First, you should read a line containing a single integer

N

denoting the number of items you have to make.

The description of interaction for each of the

N

items follows next.

For each item, you should first read a line containing a single integer,

Vi

, value of the item you have to make.

Then you should print an integer

K

in a single line, the number of items you want to buy from the shop to make an item of value

Vi

.

In the next line, print

K

space-separated integers, the values of the items you are buying from the shop to make the item of value

Vi

. Since the given

Vi

is always a positive number, your

K

should always be a positive integer as well.

Now, read a line that represents the response from the shop.

The summation of the

K

space-separated integers must be equal to

Vi

; otherwise, you will get a

Failed...

response and the interaction will terminate.

If you have not been charged more than 4 times so far and have bought at most 18000 items from the shop so far, the line will say

Great!

as a response for the first

N-1

items.

For the

N

-th item, if you have not been charged more than 4 times so far and have bought at most 18000 items from the shop so far, the line will say

Congratulations!

meaning you have won.

If you have crossed the limit of being charged at most 4 times or buying at most 18000 items at any stage, you have lost and the response line of the shop will say

Failed...

and the interaction will terminate.

Don't forget to flush the output after printing each line!

Constraints:

1

$ \leq $

N, Vi

$ \leq $

1000

Output

A sample interaction based on the example given in problem statement may look like:

> 3
> 5
< 1
< 5
> Great!
> 7
< 1
< 7
> Great!
> 12
< 2
< 5 7
> Congratulations!

>

indicates what your program reads and

<

indicates what your program writes. These symbols are here to make it easy to understand. You do not have to print such symbols from your program.

Another example interaction can be like:

> 3
> 5
< 1
< 5
> Great!
> 7
< 3
< 4 2 1
> Great!
> 12
< 1
< 12
> Failed...

In this case, the solution failed and received the response

Failed...

because of being charged 5 times (for the values 5, 4, 2, 1, 12).

Another interaction example of success is:

> 3
> 5
< 1
< 5
> Great!
> 7
< 3
< 5 1 1
> Great!
> 12
< 1
< 12
> Congratulations!

In this case, the number of times you were charged is 3 (for the values of 5, 1 and 12) and the total number of items bought from the shop is 5 (5, 5, 1, 1, 12).

An interaction example of failure is

> 3
> 5
< 1
< 5
> Great!
> 7
< 2
< 5 1
> Failed...
[Interaction Terminated]

In this case, the items bought from the shop to make the 2nd item of value 7 do not sum up to 7 i.e. the 2nd item has not been successfully made, thus the failed response and after that, the interaction has terminated.


---
