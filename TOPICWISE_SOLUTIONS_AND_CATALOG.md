# IUPC & National Contests: Master Topic-Wise Problem Catalog & Solution Guide

> **Source:** Contests archive from [therealbcs.com/iupc](https://therealbcs.com/iupc) (62 Contests, 558+ Problems, 2017–2026)

## Overview

This document classifies the problems from the national competitive programming contests (IUPC, NCPC, ICPC Dhaka Regional & Preliminaries) into core competitive programming topics. For each topic, it provides essential theoretical insights, recurring problem patterns in Bangladeshi onsite contests, in-depth solution walkthroughs, and a complete problem directory.

### Topic Distribution Summary

| Topic | Total Problems | Key Techniques |
|---|---|---|
| **Data Structures & Range Queries** | **23** | Segment Trees (Point/Range updates with Lazy Propagation), Fenwic... |
| **Dynamic Programming** | **10** | 1D/2D DP, Tree DP, Bitmask DP, Digit DP, Subsequence / String DP,... |
| **Graph Theory** | **115** | Trees, Shortest Paths (Dijkstra, 0-1 BFS), Minimum Spanning Tree ... |
| **Binary Search & Two Pointers** | **0** | Algorithms & Problem Solving... |
| **Number Theory & Mathematics** | **93** | Prime Sieve, Modular Arithmetic, Modular Inverse, GCD/LCM, Extend... |
| **Combinatorics & Probability** | **57** | Permutations, Combinations, Stars & Bars, Linearity of Expectatio... |
| **Strings** | **77** | String Hashing (Single/Double), KMP Prefix Function, Z-Algorithm,... |
| **Geometry** | **34** | Points, Vectors, Cross Product, Dot Product, Convex Hull, Shoelac... |
| **Game Theory** | **57** | Impartial Games, Nim, Sprague-Grundy theorem, Minimax, Symmetric ... |
| **Greedy & Sorting** | **31** | Greedy Choice Property, Sorting with Custom Comparators, Priority... |
| **Constructive & Ad-Hoc / Implementation** | **61** | Bitwise XOR/AND/OR logic, Parity arguments, Simulation, Chessboar... |

---

# Data Structures & Range Queries (23 Problems)

**Focus Areas:** Segment Trees (Point/Range updates with Lazy Propagation), Fenwick Tree (BIT), Monotonic Queue/Stack, Persistent Data Structures, Trie, Coordinate Compression.

### Key Algorithmic Patterns in IUPC Contests

- Coordinate compression followed by Fenwick Tree for inversion count and rank queries.
- Segment Tree with Lazy Propagation for range addition/multiplication and range sum/min/max queries.
- Trie for prefix matching and maximum XOR subarray / pair.
- Offline queries with Mo's Algorithm or Sweep-line + BIT.

### In-Depth Problem Solutions

#### Problem A: Anya Restores Order (`18 - Inter University BUET CSE Fest 2024`)

- **Problem Statement:** Maintain tubes of balls, support appending tube j to tube i, deleting tube j, and finding the smallest missing number strictly lower than the maximum ball in tube i.
- **Core Observation:** A tube is "complete" up to maximum M if all numbers 1..M exist without gaps. We only need the smallest missing value.
- **Solution Approach:** Maintain a balanced BST / Segment Tree or frequency map with Disjoint Set Union (DSU) over contiguous numbers for each tube. When merging tubes, use Small-to-Large merging (merging smaller set into larger set) to achieve O(N log^2 N) overall time.
- **Data Structures:** `DSU, Small-to-Large Merging, std::set / Fenwick Tree`
- **Complexity:** `Time: O(N \log^2 N + Q \log N), Space: O(N)`

#### Problem D: Max SMEX (`23 - CUET Inter University Programming Contest CodeStorm 1.0`)

- **Problem Statement:** Compute the maximum SMEX (Smallest Missing Even eXcluded) over dynamic subarray queries.
- **Core Observation:** Even numbers partitioned into intervals. SMEX is the first even integer 2k that does not appear in the subset.
- **Solution Approach:** Maintain presence of even numbers using a Segment Tree where leaves store whether 2k is present. Finding SMEX is finding the leftmost zero-leaf in the segment tree in O(log N).
- **Data Structures:** `Segment Tree with binary search on tree`
- **Complexity:** `Time: O(Q \log N), Space: O(N)`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **Kill Two Birds with One Stone** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 2 | **K Floors Down** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 3 | **Pattern Purifier** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 4 | **The AND, The OR, and The XOR** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 5 | **A Slice of Pi** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 6 | **Survival of the Fated** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 7 | **Pascal’s Tree** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 8 | **Prime Triangles** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 9 | **Peak Reduction** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 10 | **The Power of the Sun** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 11 | **The Great Withering** | 08 - CUET IUPC 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/08 - CUET IUPC 2025/Problemset.pdf) |
| 12 | **Delete, Deduct, and Destroy** | 10 - ICPC DHAKA 2025 ONLINE PRELIMINARY | [Statements.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/10 - ICPC DHAKA 2025 ONLINE PRELIMINARY/Statements.pdf) |
| 13 | **Your Next Line Is, “What A Cool Problem!”** | 10 - ICPC DHAKA 2025 ONLINE PRELIMINARY | [Statements.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/10 - ICPC DHAKA 2025 ONLINE PRELIMINARY/Statements.pdf) |
| 14 | **Least Compatible Ancestor** | 10 - ICPC DHAKA 2025 ONLINE PRELIMINARY | [Statements.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/10 - ICPC DHAKA 2025 ONLINE PRELIMINARY/Statements.pdf) |
| 15 | **Magical Flower Garden** | 10 - ICPC DHAKA 2025 ONLINE PRELIMINARY | [Statements.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/10 - ICPC DHAKA 2025 ONLINE PRELIMINARY/Statements.pdf) |
| 16 | **The Perfect View** | 10 - ICPC DHAKA 2025 ONLINE PRELIMINARY | [Statements.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/10 - ICPC DHAKA 2025 ONLINE PRELIMINARY/Statements.pdf) |
| 17 | **Over Counting** | 10 - ICPC DHAKA 2025 ONLINE PRELIMINARY | [Statements.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/10 - ICPC DHAKA 2025 ONLINE PRELIMINARY/Statements.pdf) |
| 18 | **The Matrix** | 10 - ICPC DHAKA 2025 ONLINE PRELIMINARY | [Statements.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/10 - ICPC DHAKA 2025 ONLINE PRELIMINARY/Statements.pdf) |
| 19 | **Chemical Reaction** | 10 - ICPC DHAKA 2025 ONLINE PRELIMINARY | [Statements.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/10 - ICPC DHAKA 2025 ONLINE PRELIMINARY/Statements.pdf) |
| 20 | **Efficient Construction on Mars** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_I_Efficient Construction on Mars.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_I_Efficient Construction on Mars.md) |
| 21 | **Life Is Dark and Full of Error** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_H_Life Is Dark and Full of Error.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_H_Life Is Dark and Full of Error.md) |
| 22 | **Party Lights** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_K_Party Lights.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_K_Party Lights.md) |
| 23 | **Cut the Rope** | 60 - SUST Inter University Programming Contest 2017 | [Problem_F_Cut the Rope.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_F_Cut the Rope.md) |

---

# Dynamic Programming (10 Problems)

**Focus Areas:** 1D/2D DP, Tree DP, Bitmask DP, Digit DP, Subsequence / String DP, Convex Hull Trick & Divide and Conquer Optimizations.

### Key Algorithmic Patterns in IUPC Contests

- State definition identifying minimal parameters representing subproblem.
- Bitmask DP for N <= 20 Hamiltonian or assignment problems.
- Digit DP for counting numbers in range [L, R] satisfying digit constraints.
- Subtree DP aggregating values from children to parent.

### In-Depth Problem Solutions

#### Problem B: Peculiar Partitioning II (`27 - BUET Inter University Programming Contest 2023`)

- **Problem Statement:** Partition an array into two non-empty subsequences to maximize the combined score.
- **Core Observation:** The score function depends only on prefixes and transitions between states in both subsequences.
- **Solution Approach:** Define DP[i][mask]: maximum score considering first i elements where mask encodes the relevant state of the two partitions. Transitions evaluate placing element i into partition 1 or partition 2.
- **Data Structures:** `2D DP table`
- **Complexity:** `Time: O(N \cdot 2^K), Space: O(N \cdot 2^K)`

#### Problem A: Again LCS (`50 - BUET CSE Fest 2019 Inter University Programming Contest`)

- **Problem Statement:** Find the Longest Common Subsequence of multiple strings under character frequency constraints.
- **Core Observation:** Standard 2-string LCS is O(N^2). When alphabet is small or string count is moderate, compress transitions using next-occurrence pointers.
- **Solution Approach:** Precompute next_pos[c][i] for each character c in each string. Use memoized search DP(pos1, pos2, ...) over valid tuple states.
- **Data Structures:** `Next occurrence table, Memoization table`
- **Complexity:** `Time: O(|\Sigma| \cdot \text{States}), Space: O(\text{States})`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **Picturesque Skyline** | 21 - NCPC Preliminary JU 2023 | [Problemset_and_Editorial.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/21 - NCPC Preliminary JU 2023/Problemset_and_Editorial.pdf) |
| 2 | **Easy String** | 21 - NCPC Preliminary JU 2023 | [Problemset_and_Editorial.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/21 - NCPC Preliminary JU 2023/Problemset_and_Editorial.pdf) |
| 3 | **Make A Beautiful Array** | 21 - NCPC Preliminary JU 2023 | [Problemset_and_Editorial.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/21 - NCPC Preliminary JU 2023/Problemset_and_Editorial.pdf) |
| 4 | **Battle of Boberland** | 21 - NCPC Preliminary JU 2023 | [Problemset_and_Editorial.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/21 - NCPC Preliminary JU 2023/Problemset_and_Editorial.pdf) |
| 5 | **Platonic number in a tree** | 21 - NCPC Preliminary JU 2023 | [Problemset_and_Editorial.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/21 - NCPC Preliminary JU 2023/Problemset_and_Editorial.pdf) |
| 6 | **Aragorn is back** | 21 - NCPC Preliminary JU 2023 | [Problemset_and_Editorial.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/21 - NCPC Preliminary JU 2023/Problemset_and_Editorial.pdf) |
| 7 | **Game of Removing** | 21 - NCPC Preliminary JU 2023 | [Problemset_and_Editorial.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/21 - NCPC Preliminary JU 2023/Problemset_and_Editorial.pdf) |
| 8 | **Calendar (Please No More)** | 21 - NCPC Preliminary JU 2023 | [Problemset_and_Editorial.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/21 - NCPC Preliminary JU 2023/Problemset_and_Editorial.pdf) |
| 9 | **Make More Money** | 33 - BUET Inter University Programming Contest 2022 | [Problem_E_Make More Money.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_E_Make More Money.md) |
| 10 | **Counting Triplets** | 60 - SUST Inter University Programming Contest 2017 | [Problem_H_Counting Triplets.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_H_Counting Triplets.md) |

---

# Graph Theory (115 Problems)

**Focus Areas:** Trees, Shortest Paths (Dijkstra, 0-1 BFS), Minimum Spanning Tree (Kruskal, Prim), LCA, Disjoint Set Union (DSU), Network Flows, Bridges, and Articulation Points.

### Key Algorithmic Patterns in IUPC Contests

- Tree diameter and centroid decomposition for distance queries.
- Lowest Common Ancestor (Binary Lifting) for path aggregations.
- DSU with rollback or small-to-large merging for dynamic connectivity.
- Multi-source BFS / Dijkstra on state graphs $(u, \text{mask})$ or $(u, \text{rem})$.

### In-Depth Problem Solutions

#### Problem C: Stay in Your Lane (`01 - IUT IUPC 2026`)

- **Problem Statement:** Navigating a directed road network with capacity and speed limits across lanes.
- **Core Observation:** The problem reduces to finding the minimum bottleneck cost path in a directed graph where lanes can transition at specific junctions.
- **Solution Approach:** Model each lane at each road segment as a node $(u, l)$. Add directed edges for straight movements and switching costs for lane changes. Run Dijkstra with a priority queue prioritizing minimum total transit time.
- **Data Structures:** `Priority Queue (Min-Heap), Adjacency List`
- **Complexity:** `Time: O((V \cdot L + E \cdot L) \log(V \cdot L)), Space: O(V \cdot L + E \cdot L)`

#### Problem E: Min-XOR MST (`04 - NSU IUPC 2026`)

- **Problem Statement:** Constructing a Minimum Spanning Tree where edge weights are determined by XOR values between vertex values.
- **Core Observation:** Boruvka's algorithm combined with a Binary Trie allows finding the minimum XOR neighbor for each component in O(log(MAX_VAL)).
- **Solution Approach:** Insert all vertex values into a Binary Trie. Recursively split the trie into left (bit 0) and right (bit 1) subtrees. At each branch, connect the two sets by finding the pair with minimum XOR using trie query. Total edges added = N - 1.
- **Data Structures:** `Binary Trie, DSU`
- **Complexity:** `Time: O(N \log N \log(\text{MAX})), Space: O(N \log(\text{MAX}))`

#### Problem J: Treasure Hunt Battle of Agincourt (`18 - Inter University BUET CSE Fest 2024`)

- **Problem Statement:** Find the optimal path on a weighted grid avoiding traps while collecting treasures with energy constraints.
- **Core Observation:** Energy constraints restrict the number of steps, creating a directed acyclic state graph (DAG) parameterized by (x, y, energy).
- **Solution Approach:** 0-1 BFS or Dijkstra on state graph (r, c, energy). If energy is small, standard DP over DAG can compute the reachable maximum treasure value.
- **Data Structures:** `Queue / Min-Heap`
- **Complexity:** `Time: O(R \cdot C \cdot K), Space: O(R \cdot C \cdot K)`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **K-Color Union** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 2 | **Nonmetal Alchemist** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 3 | **Self Citation** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 4 | **Floatovoltaics** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 5 | **Min-XOR MST** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 6 | **Fool’s Gold** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 7 | **Dynamic Ranklist** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 8 | **Capital Logistics** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 9 | **The Man, The Math, The Legend!** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 10 | **Resonance Frog** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 11 | **Diagonal Shortcuts** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 12 | **Onion Peeling** | 04 - NSU IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/04 - NSU IUPC 2026/Problemset.pdf) |
| 13 | **Mission Hexa** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 14 | **Boulevard of Broken Cars** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 15 | **Gas Reservoir** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 16 | **Save the Wonderland** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 17 | **Love Marriage** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 18 | **Morning Walk** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 19 | **Nonogram** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 20 | **Optimal Balancing Strategy** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 21 | **Two Strings Attached** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 22 | **C-Style String Length** | 07 - ICPC Asia Dhaka Regional 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/07 - ICPC Asia Dhaka Regional 2025/Problemset.pdf) |
| 23 | **Edgy Graph** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 24 | **Red Dead Redemption 2** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 25 | **Binomial XOR** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 26 | **Symmetric Swap** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 27 | **The Perfect Spider Web** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 28 | **Divisible Perfection** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 29 | **MEX-imum Beauty** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 30 | **Substring Symphony** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 31 | **Statue on a Permutation** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 32 | **Sublime Replacement** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 33 | **Math Madness** | 11 - Uttara University Inter-University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/11 - Uttara University Inter-University Programming Contest 2025/Problemset.pdf) |
| 34 | **Pair Pressure** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 35 | **The Last Bit of Us** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 36 | **Triangle Trap** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 37 | **An Interesting Problem** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 38 | **Polynomial K Paths** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 39 | **Distinct of Distincts** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 40 | **To Inﬁnity and Beyond** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 41 | **Litmus Test** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 42 | **XOR This OR That** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 43 | **LCM Factorization** | 12 - Betopia Group Presents DUET Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/12 - Betopia Group Presents DUET Inter University Programming Contest 2025/Problemset.pdf) |
| 44 | **Are** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 45 | **Yet** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 46 | **Cut** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 47 | **CatGPT** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 48 | **Quasi-binary** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 49 | **Flowers** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 50 | **Library** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 51 | **Hand** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 52 | **In** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 53 | **The** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 54 | **Packet** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 55 | **Unhappy** | 16 - ICPC Dhaka Regional Site 2024 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/16 - ICPC Dhaka Regional Site 2024/Problemset.pdf) |
| 56 | **Graffiti** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_D_Graffiti.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_D_Graffiti.md) |
| 57 | **Will Power** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_L_Will Power.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_L_Will Power.md) |
| 58 | **Meena, Raju and Mango Tree** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_C_Meena, Raju and Mango Tree.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_C_Meena, Raju and Mango Tree.md) |
| 59 | **Pop! Shop** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_D_Pop! Shop.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_D_Pop! Shop.md) |
| 60 | **Thanos LLC.** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_K_Thanos LLC..md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_K_Thanos LLC..md) |
| 61 | **Gona** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 62 | **ASCII** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 63 | **Bears** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 64 | **Pyramid** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 65 | **Crazy** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 66 | **Uncle** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 67 | **Pess** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 68 | **Island** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 69 | **Qwiksort** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 70 | **Point** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 71 | **Strategies** | 24 - ICPC Dhaka Regional Site 2023 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/24 - ICPC Dhaka Regional Site 2023/Problemset.pdf) |
| 72 | **Queries, Queries Everywhere** | 26 - CoU-BRACNet Inter University Programming Contest 2023 | [Problem_E_Queries, Queries Everywhere.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/26 - CoU-BRACNet Inter University Programming Contest 2023/Problem_E_Queries, Queries Everywhere.md) |
| 73 | **Tree Flip** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 74 | **Binary Sort** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 75 | **Network** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 76 | **Aspect Ratio** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 77 | **Overtake** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 78 | **2x2 Flip** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 79 | **Jump If You Can** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 80 | **Product Manager** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 81 | **Creating Triangles** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 82 | **Sort It** | 28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/28 - ICPC ASIA DHAKA REGIONAL CONTEST 2022/Problemset.pdf) |
| 83 | **Holy Tree** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_C_Holy Tree.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_C_Holy Tree.md) |
| 84 | **Alice, Bob and Tree** | 32 - ICPC Dhaka Regional Preliminary 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/32 - ICPC Dhaka Regional Preliminary 2021/Problemset.pdf) |
| 85 | **Red Blue Graph** | 33 - BUET Inter University Programming Contest 2022 | [Problem_G_Red Blue Graph.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_G_Red Blue Graph.md) |
| 86 | **Superman and the Buildings of Dahaka** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_B_Superman and the Buildings of Dahaka.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_B_Superman and the Buildings of Dahaka.md) |
| 87 | **Stephen, Bob, and Tomato's Canvas** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_A_Stephen, Bob, and Tomato's Canvas.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_A_Stephen, Bob, and Tomato's Canvas.md) |
| 88 | **Goku's Tree** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_F_Goku's Tree.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_F_Goku's Tree.md) |
| 89 | **Snake's Neck** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_L_Snake's Neck.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_L_Snake's Neck.md) |
| 90 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 91 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 92 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 93 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 94 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 95 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 96 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 97 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 98 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 99 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 100 | **Input: Standard Input** | 43 - RUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/43 - RUET IUPC 2019/Problemset.pdf) |
| 101 | **So Much Difference** | 45 - SUST Inter University Programming Contest 2019 | [Problem_D_So Much Difference.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_D_So Much Difference.md) |
| 102 | **MaxFlow (II)** | 45 - SUST Inter University Programming Contest 2019 | [Problem_F_MaxFlow (II).md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_F_MaxFlow (II).md) |
| 103 | **Game in a Binary Grid** | 45 - SUST Inter University Programming Contest 2019 | [Problem_L_Game in a Binary Grid.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_L_Game in a Binary Grid.md) |
| 104 | **Weird Graph** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_B_Weird Graph.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_B_Weird Graph.md) |
| 105 | **Explosion** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_F_Explosion.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_F_Explosion.md) |
| 106 | **Traffic Jam That Never Ends** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_K_Traffic Jam That Never Ends.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_K_Traffic Jam That Never Ends.md) |
| 107 | **Biswa and Restaurant Business** | 55 - BUET Inter University Programming Contest 2018 | [Problem_G_Biswa and Restaurant Business.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_G_Biswa and Restaurant Business.md) |
| 108 | **Problematic Problem Setters** | 56 - Cybernauts NPC 2018 | [Problem_D_Problematic Problem Setters.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_D_Problematic Problem Setters.md) |
| 109 | **Lighthouse 2** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_D_Lighthouse 2.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_D_Lighthouse 2.md) |
| 110 | **Lighthouse** | 60 - SUST Inter University Programming Contest 2017 | [Problem_B_Lighthouse.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_B_Lighthouse.md) |
| 111 | **Mag the Mighty Kaidul** | 60 - SUST Inter University Programming Contest 2017 | [Problem_E_Mag the Mighty Kaidul.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_E_Mag the Mighty Kaidul.md) |
| 112 | **How Many Ways?** | 60 - SUST Inter University Programming Contest 2017 | [Problem_L_How Many Ways_.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_L_How Many Ways_.md) |
| 113 | **Flower Garden** | 61 - LU Inter University Programming Contest 2017 | [Problem_B_Flower Garden.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_B_Flower Garden.md) |
| 114 | **Orchid Division** | 61 - LU Inter University Programming Contest 2017 | [Problem_J_Orchid Division.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_J_Orchid Division.md) |
| 115 | **Weapon Supplier** | 62 - SUB Inter University Programming Contest 2017 | [Problem_H_Weapon Supplier.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_H_Weapon Supplier.md) |

---

# Binary Search & Two Pointers (0 Problems)

**Focus Areas:** 

### Key Algorithmic Patterns in IUPC Contests

- Standard patterns apply.

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|

---

# Number Theory & Mathematics (93 Problems)

**Focus Areas:** Prime Sieve, Modular Arithmetic, Modular Inverse, GCD/LCM, Extended Euclidean, Euler Totient Function, Diophantine equations, Matrix Exponentiation.

### Key Algorithmic Patterns in IUPC Contests

- Linear Sieve (O(N)) precomputing smallest prime factors (SPF) for fast O(log N) factorization.
- Fermat's Little Theorem (a^(p-2) mod p) for modular inverse when modulo is prime.
- Chinese Remainder Theorem (CRT) for non-coprime or modular systems.
- Matrix exponentiation for linear recurrences in O(K^3 log N).

### In-Depth Problem Solutions

#### Problem F: Fraction Again! (`01 - IUT IUPC 2026`)

- **Problem Statement:** Simplify complex sums of fractions under modulo 998244353 and compute exact irreducible forms.
- **Core Observation:** Division under modulo requires multiplying by the modular inverse. Compute gcd to check irreducibility when exact representation is needed.
- **Solution Approach:** Precompute factorials and inverse factorials. Evaluate numerator and denominator mod P using Extended Euclidean algorithm.
- **Data Structures:** `Precomputed arrays`
- **Complexity:** `Time: O(N + \log P), Space: O(N)`

#### Problem A: Almost Perfect Prime Factor! (`25 - ICPC Dhaka Regional Preliminary Contest 2023`)

- **Problem Statement:** Determine if an integer N has prime factors that satisfy an almost-perfect balance condition.
- **Core Observation:** Prime factor powers can be identified by trial division up to sqrt(N) and Miller-Rabin test for remainder.
- **Solution Approach:** Factorize N into p_1^a1 * p_2^a2... Check if the exponents and sum of divisors condition match the predicate.
- **Data Structures:** `Sieve of Eratosthenes`
- **Complexity:** `Time: O(\sqrt{N}), Space: O(1)`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **Ask With Caution** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 2 | **Binary to Palindrome** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 3 | **Stay in Y our Lane** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 4 | **Outsmarting** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 5 | **Wonderful View** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 6 | **Fraction Again!** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 7 | **Sandfall** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 8 | **Hilly Array** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 9 | **Not T oday** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 10 | **Mode Zero** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 11 | **Peak-a-boo** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 12 | **T erminal** | 01 - IUT IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/01 - IUT IUPC 2026/Problemset.pdf) |
| 13 | **A Name of One’s Own** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 14 | **Singularity** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 15 | **Level Up** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 16 | **Skill Issue** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 17 | **T angled** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 18 | **Ebb and Flow** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 19 | **An Odd Problem** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 20 | **Echoes of Erasure** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 21 | **The Paintress** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 22 | **Know Y our Place** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 23 | **Relatively Speaking** | 03 - DUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/03 - DUET IUPC 2026/Problemset.pdf) |
| 24 | **Quantum Corridor** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 25 | **Easy Composite** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 26 | **Path of Crows** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 27 | **Dual Star** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 28 | **Chorki** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 29 | **Mandatory XOR Problem** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 30 | **Genome Evolution** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 31 | **Pothchola** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 32 | **Cosmic Bit Flip** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 33 | **Prefix Reversal** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 34 | **Lottery** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 35 | **Sapure** | 06 - BUET IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/06 - BUET IUPC 2026/Problemset.pdf) |
| 36 | **GCD and LCM in Perfect Sync** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 37 | **Prime - Prime - Prime** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_J_Prime - Prime - Prime.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_J_Prime - Prime - Prime.md) |
| 38 | **Where is the Ghost** | 26 - CoU-BRACNet Inter University Programming Contest 2023 | [Problem_A_Where is the Ghost.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/26 - CoU-BRACNet Inter University Programming Contest 2023/Problem_A_Where is the Ghost.md) |
| 39 | **A Lazy Statement** | 26 - CoU-BRACNet Inter University Programming Contest 2023 | [Problem_B_A Lazy Statement.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/26 - CoU-BRACNet Inter University Programming Contest 2023/Problem_B_A Lazy Statement.md) |
| 40 | **The Clash of Tactical Titans: Klopp vs. Ten Hag** | 26 - CoU-BRACNet Inter University Programming Contest 2023 | [Problem_G_The Clash of Tactical Titans_ Klopp vs. Ten Hag.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/26 - CoU-BRACNet Inter University Programming Contest 2023/Problem_G_The Clash of Tactical Titans_ Klopp vs. Ten Hag.md) |
| 41 | **A Game with Grandma** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 42 | **Transform the Array** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 43 | **Omago Virus** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 44 | **Omicron Juice 2023** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 45 | **Cyclic Palindrome** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 46 | **Proximity Card Data Statistics** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 47 | **Portals and Roads** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 48 | **Mr. Dumb the Police in charge** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 49 | **Image Cropping** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 50 | **Product Quality Analyst** | 29 - ICPC Dhaka Regional Preliminary Contest 2022 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/29 - ICPC Dhaka Regional Preliminary Contest 2022/Problemset.pdf) |
| 51 | **Make GCD Great Again!** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 52 | **Clash of Coprimes** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 53 | **Peculiar Partitioning** | 33 - BUET Inter University Programming Contest 2022 | [Problem_C_Peculiar Partitioning.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_C_Peculiar Partitioning.md) |
| 54 | **Colded LCM** | 33 - BUET Inter University Programming Contest 2022 | [Problem_I_Colded LCM.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_I_Colded LCM.md) |
| 55 | **Greatest GCD Ever** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 56 | **My Small Number** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_C_My Small Number.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_C_My Small Number.md) |
| 57 | **Hange and Her Gear** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_E_Hange and Her Gear.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_E_Hange and Her Gear.md) |
| 58 | **Input: Standard Input** | 44 - DUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/44 - DUET IUPC 2019/Problemset.pdf) |
| 59 | **Input: Standard Input** | 44 - DUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/44 - DUET IUPC 2019/Problemset.pdf) |
| 60 | **Input: Standard Input** | 44 - DUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/44 - DUET IUPC 2019/Problemset.pdf) |
| 61 | **Input: Standard Input** | 44 - DUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/44 - DUET IUPC 2019/Problemset.pdf) |
| 62 | **Input: Standard Input** | 44 - DUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/44 - DUET IUPC 2019/Problemset.pdf) |
| 63 | **Input: Standard Input** | 44 - DUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/44 - DUET IUPC 2019/Problemset.pdf) |
| 64 | **Input: Standard Input** | 44 - DUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/44 - DUET IUPC 2019/Problemset.pdf) |
| 65 | **Input: Standard Input** | 44 - DUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/44 - DUET IUPC 2019/Problemset.pdf) |
| 66 | **Input: Standard Input** | 44 - DUET IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/44 - DUET IUPC 2019/Problemset.pdf) |
| 67 | **Play the Lottery** | 45 - SUST Inter University Programming Contest 2019 | [Problem_B_Play the Lottery.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_B_Play the Lottery.md) |
| 68 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 69 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 70 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 71 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 72 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 73 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 74 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 75 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 76 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 77 | **Input: Standard Input** | 46 - BUP IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/46 - BUP IUPC 2019/Problemset.pdf) |
| 78 | **All the Cuts** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_D_All the Cuts.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_D_All the Cuts.md) |
| 79 | **Is It Perfect** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_H_Is It Perfect.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_H_Is It Perfect.md) |
| 80 | **Maruo and the Sequence** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_I_Maruo and the Sequence.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_I_Maruo and the Sequence.md) |
| 81 | **Prime Friendly Numbers
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 82 | **Subset with GCD K
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 83 | **Bouquet For My Valentine** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_J_Bouquet For My Valentine.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_J_Bouquet For My Valentine.md) |
| 84 | **Find the primes?** | 55 - BUET Inter University Programming Contest 2018 | [Problem_A_Find the primes_.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_A_Find the primes_.md) |
| 85 | **Level Up** | 55 - BUET Inter University Programming Contest 2018 | [Problem_C_Level Up.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_C_Level Up.md) |
| 86 | **Sequence Query** | 55 - BUET Inter University Programming Contest 2018 | [Problem_M_Sequence Query.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_M_Sequence Query.md) |
| 87 | **Amicable Numbers** | 56 - Cybernauts NPC 2018 | [Problem_A_Amicable Numbers.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_A_Amicable Numbers.md) |
| 88 | **Just Primes II (Hard)** | 56 - Cybernauts NPC 2018 | [Problem_H_Just Primes II (Hard).md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_H_Just Primes II (Hard).md) |
| 89 | **Just Primes II (Easy)** | 56 - Cybernauts NPC 2018 | [Problem_J_Just Primes II (Easy).md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_J_Just Primes II (Easy).md) |
| 90 | **That's Odd!** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_A_That's Odd!.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_A_That's Odd!.md) |
| 91 | **Breaking Math** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_B_Breaking Math.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_B_Breaking Math.md) |
| 92 | **This Is Too Hard ☹** | 61 - LU Inter University Programming Contest 2017 | [Problem_H_This Is Too Hard ☹.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_H_This Is Too Hard ☹.md) |
| 93 | **This Is Too Hard ☹** | 61 - LU Inter University Programming Contest 2017 | [Problem_H_This is Too Hard.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_H_This is Too Hard.md) |

---

# Combinatorics & Probability (57 Problems)

**Focus Areas:** Permutations, Combinations, Stars & Bars, Linearity of Expectation, Inclusion-Exclusion, Catalan Numbers.

### Key Algorithmic Patterns in IUPC Contests

- Linearity of Expectation: E[X + Y] = E[X] + E[Y] holds even when X and Y are dependent.
- Stars and Bars: Number of non-negative integer solutions to x1 + ... + xk = N is C(N + k - 1, k - 1).
- Derangements and Inclusion-Exclusion for counting arrangements with no fixed points.

### In-Depth Problem Solutions

#### Problem F: How Many Valid Collections? (`05 - NDUB IUPC 2026`)

- **Problem Statement:** Count collections of distinct items satisfying specific subset non-intersection conditions mod 10^9+7.
- **Core Observation:** Direct counting double counts overlapping collections. Apply Principle of Inclusion-Exclusion (PIE).
- **Solution Approach:** Compute sum over all intersection sizes k of (-1)^k * C(N, k) * (ways given k violations). Use precomputed factorials.
- **Data Structures:** `Factorial and inverse factorial arrays`
- **Complexity:** `Time: O(N), Space: O(N)`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **Mad Max** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 2 | **Difference Engine** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 3 | **Parallel Lives** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 4 | **Double Blind** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 5 | **A Distinct Problem** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 6 | **Shortest Paths** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 7 | **Fairy Lights** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 8 | **Standoff** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 9 | **Spot the Difference** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 10 | **Prefix Split** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 11 | **Prime Coloring** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 12 | **Appending LIS** | 02 - SUST IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/02 - SUST IUPC 2026/Problemset.pdf) |
| 13 | **86** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 14 | **All Y our Base** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 15 | **Chander Gari** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 16 | **Function Ordering** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 17 | **Helping Knuth** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 18 | **How Many Valid Collections?** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 19 | **Last Day Harvest** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 20 | **Mango Mania** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 21 | **Perils and Patrols** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 22 | **Stable Gears** | 05 - NDUB IUPC 2026 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/05 - NDUB IUPC 2026/Problemset.pdf) |
| 23 | **Interval and Expected Value** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 24 | **T ree Path Price Queries** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 25 | **Max Person** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 26 | **The New CEO of CloseAI** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 27 | **T oggle the Streetlights** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 28 | **Time Well Spent** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 29 | **Awkward Nodes** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 30 | **Guess the Number** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 31 | **Fruit Ninja** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 32 | **Insert Force** | 09 - Metropolitan University Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/09 - Metropolitan University Inter University Programming Contest 2025/Problemset.pdf) |
| 33 | **Max-Min Madness** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 34 | **The Absolute MEX Challenge** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 35 | **Palindromic Palindrome Partition** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 36 | **Strong T ree** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 37 | **Aloy and the Forbidden Code** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 38 | **Rotating Painter** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 39 | **Flip to Zero** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 40 | **The Art of Rearrangement** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 41 | **No Duplicates** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 42 | **Primal Brackets** | 13 - MTB Presents AUST Inter University Programming Contest 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/13 - MTB Presents AUST Inter University Programming Contest 2025/Problemset.pdf) |
| 43 | **Array Permutation** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 44 | **Omae Wa Mou Shindeiru** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_J_Omae Wa Mou Shindeiru.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_J_Omae Wa Mou Shindeiru.md) |
| 45 | **Again LCS** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_A_Again LCS.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_A_Again LCS.md) |
| 46 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 47 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 48 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 49 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 50 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 51 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 52 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 53 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 54 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 55 | **Input: Standard Input** | 51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/51 - 2018 ACM-ICPC, Asia Dhaka Regional Contest/Problemset.pdf) |
| 56 | **Kitorp and His Wife** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_I_Kitorp and His Wife.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_I_Kitorp and His Wife.md) |
| 57 | **Walking Down The Road** | 61 - LU Inter University Programming Contest 2017 | [Problem_A_Walking Down The Road.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_A_Walking Down The Road.md) |

---

# Strings (77 Problems)

**Focus Areas:** String Hashing (Single/Double), KMP Prefix Function, Z-Algorithm, Trie, Suffix Automaton, Palindrome Algorithms (Manacher).

### Key Algorithmic Patterns in IUPC Contests

- Polynomial rolling hash with two primes to compare substrings in O(1).
- KMP pi-array for finding periods, borders, and pattern occurrences.
- Manacher's algorithm to find all palindromic substrings in O(N).
- Trie for fast bitwise XOR search and dictionary prefix matching.

### In-Depth Problem Solutions

#### Problem B: Binary to Palindrome (`01 - IUT IUPC 2026`)

- **Problem Statement:** Transform a binary string into a palindrome using minimum bit flips or cyclic shifts.
- **Core Observation:** A palindrome requires S[i] == S[N - 1 - i]. Cyclic shifts change the pairing of indices.
- **Solution Approach:** For each cyclic shift k (0 <= k < N), compute mismatch count using FFT or rolling hash with prefix sums in O(N) or O(N log N). Take minimum over all shifts.
- **Data Structures:** `Double Rolling Hash / Prefix mismatch array`
- **Complexity:** `Time: O(N), Space: O(N)`

#### Problem A: Missing String (`19 - IUT 11th National ICT Fest Programming Contest 2024`)

- **Problem Statement:** Find the shortest lexicographically smallest string that does not appear as a substring in a given text.
- **Core Observation:** By pigeonhole principle, if text has length N, the missing string has length at most ceil(log_|Sigma|(N)) + 1.
- **Solution Approach:** For lengths L = 1, 2, 3... collect all substrings of length L in a hash set. The first length where set size < |Sigma|^L contains the missing string.
- **Data Structures:** `Hash Set / Trie`
- **Complexity:** `Time: O(N \cdot L), Space: O(N)`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **Memoir of Sifat** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_F_Memoir of Sifat.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_F_Memoir of Sifat.md) |
| 2 | **Power of a string** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_G_Power of a string.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_G_Power of a string.md) |
| 3 | **Search Engine of Nicola** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_H_Search Engine of Nicola.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_H_Search Engine of Nicola.md) |
| 4 | **Missing String** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_A_Missing String.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_A_Missing String.md) |
| 5 | **Number of Anagrams** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_B_Number of Anagrams.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_B_Number of Anagrams.md) |
| 6 | **Name Game** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_H_Name Game.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_H_Name Game.md) |
| 7 | **Anagram** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 8 | **Election** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 9 | **Equal** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 10 | **Function!** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 11 | **Good** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 12 | **Hate** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 13 | **Palindromic** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 14 | **Picturesque** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 15 | **Rik** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 16 | **Sort** | 20 - NCPC Onsite 2023 Hosted by JU | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/20 - NCPC Onsite 2023 Hosted by JU/Problemset.pdf) |
| 17 | **Nitu and Her Lucky String** | 26 - CoU-BRACNet Inter University Programming Contest 2023 | [Problem_C_Nitu and Her Lucky String.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/26 - CoU-BRACNet Inter University Programming Contest 2023/Problem_C_Nitu and Her Lucky String.md) |
| 18 | **Nitu and Pseudo-code** | 26 - CoU-BRACNet Inter University Programming Contest 2023 | [Problem_H_Nitu and Pseudo-code.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/26 - CoU-BRACNet Inter University Programming Contest 2023/Problem_H_Nitu and Pseudo-code.md) |
| 19 | **The Assignment** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_B_The Assignment.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_B_The Assignment.md) |
| 20 | **Spreadsheet v1** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_G_Spreadsheet v1.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_G_Spreadsheet v1.md) |
| 21 | **The Revenge Of Anti Hash** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 22 | **Password Shuffling** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 23 | **Chip’s Challenge** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 24 | **Constructing Strings** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 25 | **The Lieutenant's Exam** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 26 | **Fair Set** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 27 | **Creating Assignment** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 28 | **XOR** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 29 | **Hitmen** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 30 | **Ant on the Conic** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 31 | **Fare Thee Well, My Friend** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 32 | **Object Detection** | 36 - ICPC Asia Dhaka Regional Contest 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/36 - ICPC Asia Dhaka Regional Contest 2020/Problemset.pdf) |
| 33 | **Find the Word** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 34 | **Search The Files** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 35 | **Bracket Colouring** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 36 | **Water in Tree** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 37 | **K-Divisors** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 38 | **Jumping Frog Redefined** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 39 | **Age of Perceptrons** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 40 | **The Nostalgia of a Deja Vu** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 41 | **Save Mozzarella!** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 42 | **Evil Judges** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 43 | **Respectfully Giving Away** | 38 - MIST-National Collegiate Programming Contest, 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/38 - MIST-National Collegiate Programming Contest, 2020/Problemset.pdf) |
| 44 | **Simple As a Substring!** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_E_Simple As a Substring!.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_E_Simple As a Substring!.md) |
| 45 | **Palindrome Query I** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_J_Palindrome Query I.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_J_Palindrome Query I.md) |
| 46 | **Living on a Prayer** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_C_Living on a Prayer.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_C_Living on a Prayer.md) |
| 47 | **String Factory** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_G_String Factory.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_G_String Factory.md) |
| 48 | **Cook a Dish** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_I_Cook a Dish.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_I_Cook a Dish.md) |
| 49 | **Almost Pattern Matching II** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 50 | **The Social Network** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 51 | **ICGeSi Standings** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 52 | **ICPC Standings** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 53 | **Palindrome Again? Arghh!** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 54 | **Elevators** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 55 | **Pairs Forming GCD** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 56 | **Have You Heard of Cricket?** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 57 | **Almost Forgot to Welcome** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 58 | **Good Things Come to Those** | 42 - 2019 ICPC Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/42 - 2019 ICPC Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 59 | **Festival of SUST** | 45 - SUST Inter University Programming Contest 2019 | [Problem_A_Festival of SUST.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_A_Festival of SUST.md) |
| 60 | **APM** | 45 - SUST Inter University Programming Contest 2019 | [Problem_G_APM.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_G_APM.md) |
| 61 | **Bracket Sequence** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_G_Bracket Sequence.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_G_Bracket Sequence.md) |
| 62 | **A Problem for String Lovers** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_K_A Problem for String Lovers.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_K_A Problem for String Lovers.md) |
| 63 | **Find the Substrings
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 64 | **Angry Talha** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_G_Angry Talha.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_G_Angry Talha.md) |
| 65 | **Description is Pathetic** | 55 - BUET Inter University Programming Contest 2018 | [Problem_F_Description is Pathetic.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_F_Description is Pathetic.md) |
| 66 | **Secret Sorting Order** | 56 - Cybernauts NPC 2018 | [Problem_E_Secret Sorting Order.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_E_Secret Sorting Order.md) |
| 67 | **Crossword Puzzles** | 60 - SUST Inter University Programming Contest 2017 | [Problem_A_Crossword Puzzles.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_A_Crossword Puzzles.md) |
| 68 | **Chikongunia** | 60 - SUST Inter University Programming Contest 2017 | [Problem_C_Chikongunia.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_C_Chikongunia.md) |
| 69 | **Fibonacci Word Failure Function Sum** | 60 - SUST Inter University Programming Contest 2017 | [Problem_I_Fibonacci Word Failure Function Sum.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_I_Fibonacci Word Failure Function Sum.md) |
| 70 | **Palindromist** | 60 - SUST Inter University Programming Contest 2017 | [Problem_K_Palindromist.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_K_Palindromist.md) |
| 71 | **Very Dirty String** | 61 - LU Inter University Programming Contest 2017 | [Problem_D_Very Dirty String.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_D_Very Dirty String.md) |
| 72 | **Undo History** | 61 - LU Inter University Programming Contest 2017 | [Problem_G_Undo History.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_G_Undo History.md) |
| 73 | **Eloa’s Secret** | 62 - SUB Inter University Programming Contest 2017 | [Problem_D_Eloa’s Secret.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_D_Eloa’s Secret.md) |
| 74 | **Fun With Fraction** | 62 - SUB Inter University Programming Contest 2017 | [Problem_F_Fun With Fraction.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_F_Fun With Fraction.md) |
| 75 | **Beautiful String** | 62 - SUB Inter University Programming Contest 2017 | [Problem_I_Beautiful String.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_I_Beautiful String.md) |
| 76 | **Match the Color** | 62 - SUB Inter University Programming Contest 2017 | [Problem_K_Match the Color.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_K_Match the Color.md) |
| 77 | **Office Para** | 62 - SUB Inter University Programming Contest 2017 | [Problem_L_Office Para.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_L_Office Para.md) |

---

# Geometry (34 Problems)

**Focus Areas:** Points, Vectors, Cross Product, Dot Product, Convex Hull, Shoelace formula, Line Intersection, Point in Polygon.

### Key Algorithmic Patterns in IUPC Contests

- Cross product (x1*y2 - x2*y1) determines orientation (clockwise, counterclockwise, collinear).
- Monotone Chain / Graham Scan for Convex Hull in O(N log N).
- Shoelace formula for polygon area.
- Point-in-convex-polygon using binary search on angles from pivot in O(log N).

### In-Depth Problem Solutions

#### Problem D: Floatovoltaics (`04 - NSU IUPC 2026`)

- **Problem Statement:** Maximize solar panel placement area on an irregular reservoir without overlapping restricted shoreline zones.
- **Core Observation:** Panel placement area is polygon clipping and finding the maximum inscribed rectangle or circle in a polygon.
- **Solution Approach:** Represent reservoir boundaries as a polygon. Clip against forbidden zones using Sutherland-Hodgman algorithm. Compute area via Shoelace formula.
- **Data Structures:** `Point2D, Polygon structs`
- **Complexity:** `Time: O(N \log N), Space: O(N)`

#### Problem F: Cut the Rope (`60 - SUST Inter University Programming Contest 2017`)

- **Problem Statement:** Determine if a straight line cut intersects a set of circular and polygonal obstacles.
- **Core Observation:** A line ax + by + c = 0 intersects a circle of radius R at (x0, y0) iff perpendicular distance <= R.
- **Solution Approach:** Calculate perpendicular distance from line to all circle centers. For polygons, test line-segment intersection against all edges.
- **Data Structures:** `Geometry primitives`
- **Complexity:** `Time: O(N), Space: O(1)`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **Ultra-Secured Lab** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_K_Ultra-Secured Lab.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_K_Ultra-Secured Lab.md) |
| 2 | **Ri, the Miner** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_F_Ri, the Miner.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_F_Ri, the Miner.md) |
| 3 | **Doctor Strange in the Circleverse** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_I_Doctor Strange in the Circleverse.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_I_Doctor Strange in the Circleverse.md) |
| 4 | **Profitable Home** | 26 - CoU-BRACNet Inter University Programming Contest 2023 | [Problem_D_Profitable Home.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/26 - CoU-BRACNet Inter University Programming Contest 2023/Problem_D_Profitable Home.md) |
| 5 | **CONSEPHULL** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_D_CONSEPHULL.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_D_CONSEPHULL.md) |
| 6 | **Diagonal Traversal** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_E_Diagonal Traversal.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_E_Diagonal Traversal.md) |
| 7 | **Clock Fantasy** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_H_Clock Fantasy.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_H_Clock Fantasy.md) |
| 8 | **Chop Chop** | 33 - BUET Inter University Programming Contest 2022 | [Problem_A_Chop Chop.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_A_Chop Chop.md) |
| 9 | **The One With Infinite Squares** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 10 | **Kings Vs Rooks** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 11 | **Almost A Palindrome?** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 12 | **Winning Arrangements** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 13 | **Alice, Bob and the Array** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 14 | **Co Primes** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 15 | **Strange Typewriter** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 16 | **Recursion, Lambda and** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 17 | **Lattice Triangle** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 18 | **COVID - 19** | 37 - ICPC Dhaka Regional Preliminary 2020 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/37 - ICPC Dhaka Regional Preliminary 2020/Problemset.pdf) |
| 19 | **I Scream, You Scream!** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_F_I Scream, You Scream!.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_F_I Scream, You Scream!.md) |
| 20 | **Faisal and His Playgrounds** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_L_Faisal and His Playgrounds.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_L_Faisal and His Playgrounds.md) |
| 21 | **Productive Employees** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_B_Productive Employees.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_B_Productive Employees.md) |
| 22 | **Irregular Is Tough, Regular Is Easy!** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_D_Irregular Is Tough, Regular Is Easy!.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_D_Irregular Is Tough, Regular Is Easy!.md) |
| 23 | **Five Brothers' Kingdom** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_K_Five Brothers' Kingdom.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_K_Five Brothers' Kingdom.md) |
| 24 | **Childhood Game** | 45 - SUST Inter University Programming Contest 2019 | [Problem_C_Childhood Game.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_C_Childhood Game.md) |
| 25 | **Send the Love** | 45 - SUST Inter University Programming Contest 2019 | [Problem_K_Send the Love.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_K_Send the Love.md) |
| 26 | **Towers of Wadia** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_J_Towers of Wadia.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_J_Towers of Wadia.md) |
| 27 | **Modified Linear Regression** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_L_Modified Linear Regression.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_L_Modified Linear Regression.md) |
| 28 | **Doom of Mosquitoes** | 55 - BUET Inter University Programming Contest 2018 | [Problem_B_Doom of Mosquitoes.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_B_Doom of Mosquitoes.md) |
| 29 | **Broken Roads and Hearts** | 55 - BUET Inter University Programming Contest 2018 | [Problem_I_Broken Roads and Hearts.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_I_Broken Roads and Hearts.md) |
| 30 | **Bikpik Colony** | 56 - Cybernauts NPC 2018 | [Problem_C_Bikpik Colony.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_C_Bikpik Colony.md) |
| 31 | **Ha Ha Ha** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_H_Ha Ha Ha.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_H_Ha Ha Ha.md) |
| 32 | **Problem Number Nine and Three Quarter** | 60 - SUST Inter University Programming Contest 2017 | [Problem_D_Problem Number Nine and Three Quarter.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_D_Problem Number Nine and Three Quarter.md) |
| 33 | **Uncle M** | 62 - SUB Inter University Programming Contest 2017 | [Problem_E_Uncle M.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_E_Uncle M.md) |
| 34 | **Hyperloop** | 62 - SUB Inter University Programming Contest 2017 | [Problem_J_Hyperloop.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_J_Hyperloop.md) |

---

# Game Theory (57 Problems)

**Focus Areas:** Impartial Games, Nim, Sprague-Grundy theorem, Minimax, Symmetric Strategies, Invariant Analysis.

### Key Algorithmic Patterns in IUPC Contests

- XOR sum of pile sizes in Nim: non-zero means winning position for first player.
- Calculate Grundy value G(u) = mex({G(v) : u -> v}). Game composite is XOR of Grundy values.
- Look for symmetry: if second player can always mirror first player's moves, second player wins.

### In-Depth Problem Solutions

#### Problem A: Game of Tic-Tac-Toe, Again (`40 - NSU Cybernauts National Programming Contest 2019`)

- **Problem Statement:** Analyze multi-dimensional or modified Tic-Tac-Toe game states to determine the winner under optimal play.
- **Core Observation:** The board size is small enough that game states can be recursively evaluated with memoization (Minimax).
- **Solution Approach:** Represent board as base-3 integer or string. Use minimax(state, player) with alpha-beta pruning. If state visited, return cached result.
- **Data Structures:** `Memoization table / Transposition table`
- **Complexity:** `Time: O(3^9), Space: O(3^9)`

#### Problem E: Interesting Game (`18 - Inter University BUET CSE Fest 2024`)

- **Problem Statement:** Players remove elements from an array according to divisibility rules; last player to move wins.
- **Core Observation:** Each element corresponds to an independent game state governed by its prime factorization.
- **Solution Approach:** Compute Grundy values for individual prime powers. The overall game state is the XOR sum of Grundy values of all numbers.
- **Data Structures:** `Sieve, Grundy array`
- **Complexity:** `Time: O(MAX \log \log MAX), Space: O(MAX)`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **A Boring Number Game** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 2 | **Bijgonit** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 3 | **Magnetic Bond Optimization** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 4 | **Daripalla** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 5 | **Escape Plan II** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 6 | **Flowers II** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 7 | **Glitch in the Multiverse** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 8 | **Array Apocalypse** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 9 | **Let’s Learn Multiplication Table** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 10 | **T5** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 11 | **Total Distance Over All Trees** | 14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/14 - UIU INTER-UNIVERSITY PROGRAMMING CONTEST 2025/Problemset.pdf) |
| 12 | **Baskets and Stones** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 13 | **Boat-Flix** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_B_Boat-Flix.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_B_Boat-Flix.md) |
| 14 | **Interesting Game** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_E_Interesting Game.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_E_Interesting Game.md) |
| 15 | **Tiebreaker the Heartbreaker** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_I_Tiebreaker the Heartbreaker.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_I_Tiebreaker the Heartbreaker.md) |
| 16 | **Efficient Tour** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_G_Efficient Tour.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_G_Efficient Tour.md) |
| 17 | **Fuel Finance** | 19 - IUT 11th National ICT Fest Programming Contest 2024 | [Problem_L_Fuel Finance.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/19 - IUT 11th National ICT Fest Programming Contest 2024/Problem_L_Fuel Finance.md) |
| 18 | **Alice and Bob's Laziness** | 26 - CoU-BRACNet Inter University Programming Contest 2023 | [Problem_I_Alice and Bob's Laziness.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/26 - CoU-BRACNet Inter University Programming Contest 2023/Problem_I_Alice and Bob's Laziness.md) |
| 19 | **Yet Another Frog Jumping Problem** | 33 - BUET Inter University Programming Contest 2022 | [Problem_D_Yet Another Frog Jumping Problem.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_D_Yet Another Frog Jumping Problem.md) |
| 20 | **Tomar Mobile E Games Ache?** | 33 - BUET Inter University Programming Contest 2022 | [Problem_H_Tomar Mobile E Games Ache_.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_H_Tomar Mobile E Games Ache_.md) |
| 21 | **Shine on You Crazy Diamond** | 33 - BUET Inter University Programming Contest 2022 | [Problem_J_Shine on You Crazy Diamond.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_J_Shine on You Crazy Diamond.md) |
| 22 | **Lord of the Curses** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 23 | **I know Recursions!** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 24 | **Colored Development** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 25 | **R X** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 26 | **Trees Are Beautiful** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 27 | **What happens if you sum?** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 28 | **Where are Nordomas Kit?** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 29 | **Droplets** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 30 | **Round Tables** | 39 - 2019 ICPC Dhaka Regional Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/39 - 2019 ICPC Dhaka Regional Contest/Problemset.pdf) |
| 31 | **Game of Tic-Tac-Toe, Again** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_A_Game of Tic-Tac-Toe, Again.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_A_Game of Tic-Tac-Toe, Again.md) |
| 32 | **Fashion Show** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_D_Fashion Show.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_D_Fashion Show.md) |
| 33 | **Unfair Robot Race** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_I_Unfair Robot Race.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_I_Unfair Robot Race.md) |
| 34 | **Fantastic Food** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_K_Fantastic Food.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_K_Fantastic Food.md) |
| 35 | **Mr Max Count Sum** | 41 - LU CSE Carnival 2019 Inter University Programming Contest | [Problem_H_Mr Max Count Sum.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/41 - LU CSE Carnival 2019 Inter University Programming Contest/Problem_H_Mr Max Count Sum.md) |
| 36 | **T5 Racing** | 45 - SUST Inter University Programming Contest 2019 | [Problem_H_T5 Racing.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_H_T5 Racing.md) |
| 37 | **Welcome
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 38 | **Boring Chess
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 39 | **Odd is real
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 40 | **The End
 
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 41 | **Colorful Balls
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 42 | **Vugol Search
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 43 | **Yet Another Longest Path Problem
 
Input** | 52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/52 - 2018 ACM-ICPC, Asia Dhaka Regional Preliminary Contest/Problemset.pdf) |
| 44 | **Left and Right** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_A_Left and Right.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_A_Left and Right.md) |
| 45 | **Game of Tic-Tac-Toe** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_B_Game of Tic-Tac-Toe.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_B_Game of Tic-Tac-Toe.md) |
| 46 | **Tasks** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_D_Tasks.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_D_Tasks.md) |
| 47 | **Towers of Doom** | 55 - BUET Inter University Programming Contest 2018 | [Problem_L_Towers of Doom.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_L_Towers of Doom.md) |
| 48 | **Be Efficient!!** | 56 - Cybernauts NPC 2018 | [Problem_F_Be Efficient!!.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_F_Be Efficient!!.md) |
| 49 | **Alice Loves to Play Games** | 56 - Cybernauts NPC 2018 | [Problem_G_Alice Loves to Play Games.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_G_Alice Loves to Play Games.md) |
| 50 | **Paying Bills** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_E_Paying Bills.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_E_Paying Bills.md) |
| 51 | **Stone Hopping** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_G_Stone Hopping.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_G_Stone Hopping.md) |
| 52 | **Not Linkin Park!** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_I_Not Linkin Park!.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_I_Not Linkin Park!.md) |
| 53 | **Battle of Endor** | 60 - SUST Inter University Programming Contest 2017 | [Problem_G_Battle of Endor.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_G_Battle of Endor.md) |
| 54 | **Putting Guards** | 60 - SUST Inter University Programming Contest 2017 | [Problem_J_Putting Guards.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/60 - SUST Inter University Programming Contest 2017/Problem_J_Putting Guards.md) |
| 55 | **Frog and Points** | 61 - LU Inter University Programming Contest 2017 | [Problem_I_Frog and Points.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_I_Frog and Points.md) |
| 56 | **A Simple Game** | 62 - SUB Inter University Programming Contest 2017 | [Problem_B_A Simple Game.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_B_A Simple Game.md) |
| 57 | **Cache Cash** | 62 - SUB Inter University Programming Contest 2017 | [Problem_G_Cache Cash.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_G_Cache Cash.md) |

---

# Greedy & Sorting (31 Problems)

**Focus Areas:** Greedy Choice Property, Sorting with Custom Comparators, Priority Queues, Interval Scheduling.

### Key Algorithmic Patterns in IUPC Contests

- Exchange argument: prove that swapping any two elements in non-greedy order cannot improve the objective.
- Sort by end time for interval scheduling.
- Two pointers on sorted arrays to find pairs satisfying sum/difference constraints in O(N).

### In-Depth Problem Solutions

#### Problem B: Boat-Flix (`18 - Inter University BUET CSE Fest 2024`)

- **Problem Statement:** Optimal scheduling of movie watch parties on boats with capacity and time overlaps.
- **Core Observation:** Greedy interval scheduling: sorting by end times maximizes the number of non-overlapping events.
- **Solution Approach:** Sort all intervals by finish time. Maintain available boat release times in a multiset or min-heap. For each event, allocate to the boat that finished most recently.
- **Data Structures:** `std::multiset / std::priority_queue`
- **Complexity:** `Time: O(N \log N), Space: O(N)`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **Big Tang Theory** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_F_Big Tang Theory.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_F_Big Tang Theory.md) |
| 2 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 3 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 4 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 5 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 6 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 7 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 8 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 9 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 10 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 11 | **Input: Standard Input** | 47 - SUB IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/47 - SUB IUPC 2019/Problemset.pdf) |
| 12 | **Input: Standard Input** | 48 - MIST Inter University Programming Contest 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/48 - MIST Inter University Programming Contest 2019/Problemset.pdf) |
| 13 | **Input: Standard Input** | 48 - MIST Inter University Programming Contest 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/48 - MIST Inter University Programming Contest 2019/Problemset.pdf) |
| 14 | **Input: Standard Input** | 48 - MIST Inter University Programming Contest 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/48 - MIST Inter University Programming Contest 2019/Problemset.pdf) |
| 15 | **Input: Standard Input** | 48 - MIST Inter University Programming Contest 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/48 - MIST Inter University Programming Contest 2019/Problemset.pdf) |
| 16 | **Input: Standard Input** | 48 - MIST Inter University Programming Contest 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/48 - MIST Inter University Programming Contest 2019/Problemset.pdf) |
| 17 | **Input: Standard Input** | 48 - MIST Inter University Programming Contest 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/48 - MIST Inter University Programming Contest 2019/Problemset.pdf) |
| 18 | **Input: Standard Input** | 48 - MIST Inter University Programming Contest 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/48 - MIST Inter University Programming Contest 2019/Problemset.pdf) |
| 19 | **Input: Standard Input** | 48 - MIST Inter University Programming Contest 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/48 - MIST Inter University Programming Contest 2019/Problemset.pdf) |
| 20 | **Input: Standard Input** | 48 - MIST Inter University Programming Contest 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/48 - MIST Inter University Programming Contest 2019/Problemset.pdf) |
| 21 | **Input: Standard Input** | 49 - MIST IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/49 - MIST IUPC 2019/Problemset.pdf) |
| 22 | **Input: Standard Input** | 49 - MIST IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/49 - MIST IUPC 2019/Problemset.pdf) |
| 23 | **Input: Standard Input** | 49 - MIST IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/49 - MIST IUPC 2019/Problemset.pdf) |
| 24 | **Input: Standard Input** | 49 - MIST IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/49 - MIST IUPC 2019/Problemset.pdf) |
| 25 | **Input: Standard Input** | 49 - MIST IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/49 - MIST IUPC 2019/Problemset.pdf) |
| 26 | **Input: Standard Input** | 49 - MIST IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/49 - MIST IUPC 2019/Problemset.pdf) |
| 27 | **Input: Standard Input** | 49 - MIST IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/49 - MIST IUPC 2019/Problemset.pdf) |
| 28 | **Input: Standard Input** | 49 - MIST IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/49 - MIST IUPC 2019/Problemset.pdf) |
| 29 | **Input: Standard Input** | 49 - MIST IUPC 2019 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/49 - MIST IUPC 2019/Problemset.pdf) |
| 30 | **A Feast for the Fans** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_H_A Feast for the Fans.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_H_A Feast for the Fans.md) |
| 31 | **Problem Setter Crisis** | 61 - LU Inter University Programming Contest 2017 | [Problem_E_Problem Setter Crisis.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_E_Problem Setter Crisis.md) |

---

# Constructive & Ad-Hoc / Implementation (61 Problems)

**Focus Areas:** Bitwise XOR/AND/OR logic, Parity arguments, Simulation, Chessboard/Grid invariants, Invariant Maintenance.

### Key Algorithmic Patterns in IUPC Contests

- Bitwise independence: analyze each bit position (0 to 30 or 60) independently.
- Invariants: find a quantity (sum mod 2, inversion count mod 2) that remains unchanged under operations.
- Constructive bases: use powers of 2 or tree traversal to build valid solutions.

### In-Depth Problem Solutions

#### Problem A: Adhoc King (`17 - ICPC PRELIMINARY DHAKA SITE 2024`)

- **Problem Statement:** Construct an array satisfying pairwise GCD and XOR conditions or determine if impossible.
- **Core Observation:** Pair adjacent elements as (2k, 2k+1) whose XOR is 1 and GCD is 1.
- **Solution Approach:** Use consecutive odd-even pairings to satisfy parity and coprime conditions constructively.
- **Data Structures:** `Direct array construction`
- **Complexity:** `Time: O(N), Space: O(N)`

#### Problem A: That's Odd! (`57 - IUT 9th ICT Fest 2017 Programming Contest`)

- **Problem Statement:** Sum all odd numbers from a list of given integers.
- **Core Observation:** Check bit 0 (x & 1) or x % 2 != 0.
- **Solution Approach:** Iterate through array, add to accumulator if odd.
- **Data Structures:** `Accumulator`
- **Complexity:** `Time: O(N), Space: O(1)`

### Complete Problem Directory

| # | Problem Title | Contest | File Location |
|---|---|---|---|
| 1 | **Perpendicular Parking** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 2 | **Effective Rendering** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 3 | **Dysbinaria** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 4 | **Escape Plan** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 5 | **Funny Fairy Tale** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 6 | **The Scientist** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 7 | **Ticket Dilemma** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 8 | **Travel on the grid II** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 9 | **Earthquake** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 10 | **The Beast** | 15 - MIAKI PRESENTS KUET IUPC ONSITE 2025 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/15 - MIAKI PRESENTS KUET IUPC ONSITE 2025/Problemset.pdf) |
| 11 | **Anya Restores Order** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_A_Anya Restores Order.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_A_Anya Restores Order.md) |
| 12 | **Dual Wield** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_C_Dual Wield.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_C_Dual Wield.md) |
| 13 | **Treasure Hunt: Battle Of Agincourt** | 18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024 | [Problem_J_Treasure Hunt_ Battle Of Agincourt.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/18 - Inter University Programming Contest _ United Group Presents BUET CSE Fest 2024/Problem_J_Treasure Hunt_ Battle Of Agincourt.md) |
| 14 | **Demon Slayer** | 23 - CUET Inter University Programming Contest CodeStorm 1.0 | [Problem_E_Demon Slayer.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/23 - CUET Inter University Programming Contest CodeStorm 1.0/Problem_E_Demon Slayer.md) |
| 15 | **Safwan's Book Bonanza** | 26 - CoU-BRACNet Inter University Programming Contest 2023 | [Problem_F_Safwan's Book Bonanza.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/26 - CoU-BRACNet Inter University Programming Contest 2023/Problem_F_Safwan's Book Bonanza.md) |
| 16 | **StackLang** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_A_StackLang.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_A_StackLang.md) |
| 17 | **Order of Digits** | 30 - Cefalo SUST Inter University Programming Contest 2023 | [Problem_J_Order of Digits.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/30 - Cefalo SUST Inter University Programming Contest 2023/Problem_J_Order of Digits.md) |
| 18 | **Beautiful Blocks Again!** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 19 | **Black Bishop** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 20 | **Codovid Virus** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 21 | **Der Stern** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 22 | **Calendars** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 23 | **Flip** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 24 | **Vishon Xor** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 25 | **Keep Calm, Keep padding** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 26 | **ICPC Standing** | 31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/31 - ICPC ASIA DHAKA REGIONAL CONTEST 2021/Problemset.pdf) |
| 27 | **Omicron Juice** | 32 - ICPC Dhaka Regional Preliminary 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/32 - ICPC Dhaka Regional Preliminary 2021/Problemset.pdf) |
| 28 | **Omicron Juice Again** | 32 - ICPC Dhaka Regional Preliminary 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/32 - ICPC Dhaka Regional Preliminary 2021/Problemset.pdf) |
| 29 | **Bitonic Beaver** | 32 - ICPC Dhaka Regional Preliminary 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/32 - ICPC Dhaka Regional Preliminary 2021/Problemset.pdf) |
| 30 | **Lazy Squirrel** | 32 - ICPC Dhaka Regional Preliminary 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/32 - ICPC Dhaka Regional Preliminary 2021/Problemset.pdf) |
| 31 | **Pairdrome** | 32 - ICPC Dhaka Regional Preliminary 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/32 - ICPC Dhaka Regional Preliminary 2021/Problemset.pdf) |
| 32 | **A Lonely Queen** | 32 - ICPC Dhaka Regional Preliminary 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/32 - ICPC Dhaka Regional Preliminary 2021/Problemset.pdf) |
| 33 | **Update Query Problem** | 32 - ICPC Dhaka Regional Preliminary 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/32 - ICPC Dhaka Regional Preliminary 2021/Problemset.pdf) |
| 34 | **Hovercraft** | 32 - ICPC Dhaka Regional Preliminary 2021 | [Problemset.pdf](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/32 - ICPC Dhaka Regional Preliminary 2021/Problemset.pdf) |
| 35 | **Up You Go** | 33 - BUET Inter University Programming Contest 2022 | [Problem_B_Up You Go.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_B_Up You Go.md) |
| 36 | **Choco Fun** | 33 - BUET Inter University Programming Contest 2022 | [Problem_F_Choco Fun.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/33 - BUET Inter University Programming Contest 2022/Problem_F_Choco Fun.md) |
| 37 | **Admission Gift** | 40 - NSU Cybernauts National Programming Contest 2019 | [Problem_G_Admission Gift.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/40 - NSU Cybernauts National Programming Contest 2019/Problem_G_Admission Gift.md) |
| 38 | **Remember the Name...** | 45 - SUST Inter University Programming Contest 2019 | [Problem_E_Remember the Name....md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_E_Remember the Name....md) |
| 39 | **Biswa and Morse Code** | 45 - SUST Inter University Programming Contest 2019 | [Problem_I_Biswa and Morse Code.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_I_Biswa and Morse Code.md) |
| 40 | **Jumping Frog (II)** | 45 - SUST Inter University Programming Contest 2019 | [Problem_J_Jumping Frog (II).md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/45 - SUST Inter University Programming Contest 2019/Problem_J_Jumping Frog (II).md) |
| 41 | **Group_Of_Extraordinary_People of ZUKIA** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_C_Group_Of_Extraordinary_People of ZUKIA.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_C_Group_Of_Extraordinary_People of ZUKIA.md) |
| 42 | **A Unique Array** | 50 - BUET CSE Fest 2019 Inter University Programming Contest | [Problem_E_A Unique Array.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/50 - BUET CSE Fest 2019 Inter University Programming Contest/Problem_E_A Unique Array.md) |
| 43 | **Maximum Direction in a Matrix** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_C_Maximum Direction in a Matrix.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_C_Maximum Direction in a Matrix.md) |
| 44 | **Printing Error** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_E_Printing Error.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_E_Printing Error.md) |
| 45 | **Chocolates** | 54 - 1st AUB Inter University Programming Contest 2018 | [Problem_F_Chocolates.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/54 - 1st AUB Inter University Programming Contest 2018/Problem_F_Chocolates.md) |
| 46 | **Little Dwayne** | 55 - BUET Inter University Programming Contest 2018 | [Problem_D_Little Dwayne.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_D_Little Dwayne.md) |
| 47 | **Unbelievable Array** | 55 - BUET Inter University Programming Contest 2018 | [Problem_E_Unbelievable Array.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_E_Unbelievable Array.md) |
| 48 | **Nothing’s more contagious than laughter** | 55 - BUET Inter University Programming Contest 2018 | [Problem_H_Nothing’s more contagious than laughter.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_H_Nothing’s more contagious than laughter.md) |
| 49 | **Selfie Restriction** | 55 - BUET Inter University Programming Contest 2018 | [Problem_J_Selfie Restriction.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_J_Selfie Restriction.md) |
| 50 | **Noora Number** | 55 - BUET Inter University Programming Contest 2018 | [Problem_K_Noora Number.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/55 - BUET Inter University Programming Contest 2018/Problem_K_Noora Number.md) |
| 51 | **Light The Candle** | 56 - Cybernauts NPC 2018 | [Problem_B_Light The Candle.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_B_Light The Candle.md) |
| 52 | **Water Project of Black Iceland** | 56 - Cybernauts NPC 2018 | [Problem_I_Water Project of Black Iceland.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_I_Water Project of Black Iceland.md) |
| 53 | **War of Kingdoms** | 56 - Cybernauts NPC 2018 | [Problem_K_War of Kingdoms.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_K_War of Kingdoms.md) |
| 54 | **Biswa and Red-Black Ants** | 56 - Cybernauts NPC 2018 | [Problem_L_Biswa and Red-Black Ants.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/56 - Cybernauts NPC 2018/Problem_L_Biswa and Red-Black Ants.md) |
| 55 | **Shhh! Don't Tell!** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_C_Shhh! Don't Tell!.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_C_Shhh! Don't Tell!.md) |
| 56 | **Calculus Helper** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_F_Calculus Helper.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_F_Calculus Helper.md) |
| 57 | **ZiGzAg NuMbEr** | 57 - IUT 9th ICT Fest 2017 Programming Contest | [Problem_J_ZiGzAg NuMbEr.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/57 - IUT 9th ICT Fest 2017 Programming Contest/Problem_J_ZiGzAg NuMbEr.md) |
| 58 | **Maximum Sum** | 61 - LU Inter University Programming Contest 2017 | [Problem_C_Maximum Sum.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_C_Maximum Sum.md) |
| 59 | **Yet Another Update Query Problem** | 61 - LU Inter University Programming Contest 2017 | [Problem_F_Yet Another Update Query Problem.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/61 - LU Inter University Programming Contest 2017/Problem_F_Yet Another Update Query Problem.md) |
| 60 | **Buzz Lightyear** | 62 - SUB Inter University Programming Contest 2017 | [Problem_A_Buzz Lightyear.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_A_Buzz Lightyear.md) |
| 61 | **Chocolate Rounds** | 62 - SUB Inter University Programming Contest 2017 | [Problem_C_Chocolate Rounds.md](file:///c:/Users/m0stafakamal/Desktop/IUPC_Contests/62 - SUB Inter University Programming Contest 2017/Problem_C_Chocolate Rounds.md) |

---
