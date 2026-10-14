# Mag the Mighty Kaidul

**URL:** https://toph.co/p/mag-the-mighty-kaidul  

---

The winter is about to come. Mag the Mighty Kaidul is waiting for it for days. It is his favorite season when he passes his time in his triangular love of Facebook, Quora and Lungi. As he wants no disturbance during this period, he is going to recheck his personal DNS servers which are situated on the wall.

Instead of bricks, the wall is actually made of routers and servers. The wall is made of L levels. In each level there are N partitions there. In each partition there is a either a server or router. DNS servers are all situated in the topmost level. In the partitions of every other level there are only routers. There is same number of connecting wires between every two devices (router or DNS Server) situated in the partitions of two adjacent levels.

Kaidul will be sending HTTP requests from his personal computer to the routers of the bottommost level. Requests will then travel level by level and reach the DNS servers on the topmost level. He wants to stay unique and doesn’t want his HTTP requests to travel in the same path already traveled by another request because otherwise he can be traced by White Hackers. (Two paths are said to be different if there is at least one connecting wire which is not present in both of the paths)

Now Kaidul wonders how many different unique HTTP requests he can make which ends up in one of the DNS servers. Are you up for helping Kaidul just to score a problem?

Input

The first line of the test case will contain the number of levels

$L$

(

$2 ≤ L ≤ 100000$

) and the number of bricks in each level

$N$

(

$1 ≤ N ≤ 100$

).

The following N lines will contain N numbers each. The

$j$

-th number (

$1 ≤ j ≤ N$

) on

$i$

-th line (

$1 ≤ i ≤ N$

),

$a_ij$

(

$0 ≤ a_ij ≤ 100$

) represents the number of connecting wires between device pair

$(i, j)$

of two adjacent levels.

Output

You have to print the number of unique paths that can be used for sending the HTTP requests. As this numbers can be pretty large you have print the remainder of this number after dividing by 1717171769.

Example


---

## Samples

### Sample Input 1
```
2 2
2 2
1 2
```

### Sample Output 1
```
7
```
