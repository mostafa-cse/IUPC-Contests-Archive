# Flower Garden

**URL:** https://toph.co/p/flower-garden  

---

Trisha and her little sister Rafa loves gardening. They plant trees and water them everyday. When they get tired, they enjoy watching the flowers in the trees.

Now it's 7 PM and they must leave gardening and start studying. Trisha has made a plan to draw a tree in her exercise book. Rafa, the little one, decides to count the number of flowers that can be grown in that tree.

According to Wikipedia, "In graph theory, a tree is an undirected graph in which any two vertices are connected by exactly one path. In other words, any acyclic connected graph is a tree." The following graph is a tree with six vertices:

A flower is a sub-graph in a tree, with 3 petal nodes connected with a central root. In the picture above, if the root is the node 4, then the following 4 different flowers can be drawn in that tree:

Fascinated by the look of flowers, Rafa asks Trisha about how many ways flowers can be drawn in a given tree. Two ways are considered different, if there are different number of flowers in two configurations. If both configurations have the same number of flowers, then if there is at least one flower is drawn at a different place, then these two configurations are also different.

Trisha says she is not good at math. Help her find the answer.

Input

The first line contains a positive integer

$n$

(

$n ≤ 10^5$

), the number of nodes in a tree.

The next

$n - 1$

lines will contain two integers

$u$

and

$v$

(

$1 ≤ u, v ≤ n$

), each describing an edge in that tree. You can safely assume that the tree is connected.

Output

For each input, print one line, the number of ways flowers can be drawn in the given in that tree. Since the answer can be huge, print the answer modulo

$10^9$

.

Example


---

## Samples

### Sample Input 1
```
6
1 4
2 4
3 4
4 5
5 6
```

### Sample Output 1
```
4
```
