# So Much Difference

**URL:** https://toph.co/p/so-much-difference  

---

Difference starts with a 'D'. This is the root of all dissimilarities and arguments and fights. Figuring out differences is just like figuring out your life. Sometimes they confuse you but in the end it is all worth it. If you can't find out the difference between things, or solve the difference between people, your life is as meaningless as you are. But before you can solve the difference between things you must find it out. That's why you have made a function that can figure out the difference between everything.

You are given a Tree. And some paths on that tree, you need to use your function to figure out the difference between those paths.

function Distance(x1, y1, x2, y2)  
    Array1 = []
    Array2 = []

    For A1 = nodes on the unique path from x1 to y1 
        Array1.push(V[A1])   
    end For
    
    For A2 = nodes on the unique path from x2 to y2 
        Array2.push(V[A2])   
    end For

    NewArray1 = sort the elements inside Array1
    NewArray2 = sort the elements inside Array2

    len1 = element count in Array1
    len2 = element count in Array2
    mid1 = ceiling(len1 / 2)
    mid2 = ceiling(len2 / 2)
    maxFreq = 0

    For P = elements in Array1
        cnt = 0
        For Q = elements in Array1
            if P equals Q
                cnt = cnt + 1
            end if 
        end For
       maxFreq = Maximum(maxFreq, cnt)         
    end For
    //|A| denotes the absolute value of A
    difference = |NewArray1[mid1] - NewArray2[mid2]|

    return (maxFreq * difference)
end function

Note: All the Array index starts from 1

Input

The first line contains an integer

N

number of nodes in the tree.

Then there will be a single line containing

N

integers

V[1], V[2], V[3], ... V[N]

.

V[i]

is the value on the

ith

node.

Following

(N - 1)

lines will contain two integers

u

and

v

, means there is a edge from

u

to

v

. Edges are bidirectional.

Then there will be Q queries. Each line will contain four integers

x1

,

y1

,

x2

,

y2

.

1 ≤ N ≤ 105

1 ≤ u, v, x1, y1, x2, y2 ≤ N

1 ≤ Q ≤ 105

-108 ≤ V[i] ≤ 108

Output

For each query output the answer of the Distance function in a single line. For better understanding check the samples.

Example

Notes

Note: All the Array index starts from 1.


---

## Samples

### Sample Input 1
```
8
1 2 3 4 5 6 7 8
1 2
2 3
3 4
4 5
5 6
6 7
7 8
5
1 2 1 7
2 8 4 8
1 5 5 8
1 8 2 5
8 8 3 7
```

### Sample Output 1
```
3
1
3
1
3
```
