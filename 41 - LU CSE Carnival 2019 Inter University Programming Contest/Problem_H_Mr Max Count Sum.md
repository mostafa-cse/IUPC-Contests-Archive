# Mr Max Count Sum

**URL:** https://toph.co/p/mr-max-count-sum  

---

Mr Max

,

Mr Sum

and

Mr Count

are three neighbours. They have a common enemy, an old man living in the building opposite to them who disturbs everyone with his loud music every morning. So they have decided to break into his house and destroy the music player. One day they went inside his house while he was sleeping and found a mysterious box. When they opened the box, they saw a paper with a function written on it. As they read it out loud, it changed their lives forever. Now, you are also given that function. Let's see if you can change your life as well.

Given an array A containing N elements. Find the output of the given function for all different K [1 to N] using the life changing function.

function solveMeIfYouCan(A, K)
    mr_sum = 0
    len = element count in A

    For L = 1 to len
        For R = L to len 
            mr_max = A[L]
            mr_count = 0
            
            For i = L to R
                mr_max = max(mr_max, A[i])
            end For     
     
            For i = L to R
                If mr_max equals A[i] 
                    mr_count = mr_count + 1
                end If
            end For

            If K equals mr_count
                mr_sum = mr_sum + 1
            end If
        end For
    end For

  return mr_sum
end function

Note: Array indexing starts from 1.

Input

The first line contains the integer N - number of elements in A. Next line contains

N

integers denoting the elements of array

A

.

1 ≤ N ≤ 105

1 ≤ A[i] ≤ 109

Output

Print a single line containing N space separated numbers, denoting the answer of the given function for all possible K (1 to N).

Example


---

## Samples

### Sample Input 1
```
5
1 2 2 1 2
```

### Sample Output 1
```
8 5 2 0 0
```
