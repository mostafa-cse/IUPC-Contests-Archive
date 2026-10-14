# 🏆 Bangladesh National Programming Contests Archive (IUPC / ICPC / NCPC)

[![GitHub repo](https://img.shields.io/badge/GitHub-IUPC--Contests--Archive-blue?logo=github)](https://github.com/mostafa-cse/IUPC-Contests-Archive)
[![Contests](https://img.shields.io/badge/Contests-62-brightgreen)](#-archived-contests)
[![Problems](https://img.shields.io/badge/Problems-550%2B-orange)](#-topic-wise-problem-breakdown)
[![Years](https://img.shields.io/badge/Years-2017--2026-blueviolet)](#)

A comprehensive, organized archive of **62 Inter University Programming Contests (IUPC)**, **National Collegiate Programming Contests (NCPC)**, and **ICPC Asia Dhaka Regional Contests** held across Bangladesh from **2017 to 2026**.

Sourced from [therealbcs.com/iupc](https://therealbcs.com/iupc) and verified against official platform archives (Toph, Codeforces Gym, BapsOJ, GitHub).

---

## 📖 Master Topic-Wise Solutions & Categorization

> 📘 **Full Guide:** Read the [**Topic-Wise Problem Catalog & Solution Blueprints**](./TOPICWISE_SOLUTIONS_AND_CATEGORIZATION.md) for deep-dive algorithmic approaches, mathematical invariants, data structures, and $\mathcal{O}(\dots)$ complexity analysis for all 550+ problems.

### 📊 Problem Distribution by Topic

| # | Topic | Count | Core Techniques & Algorithms |
|---|---|:---:|---|
| 1 | 🕸️ **Graph Theory & Trees** | **136** | Dijkstra on State Graph, 0-1 BFS, Tree LCA (Binary Lifting), Kruskal (MST), DSU, Bipartite Matching, Flow, Bridges & SCC |
| 2 | 🔢 **Number Theory & Math** | **88** | Linear Sieve, Prime Factorization, GCD/LCM, Modular Inverse, Diophantine equations, Euler Totient, FFT |
| 3 | 🔤 **Strings & Pattern Matching** | **88** | Double Polynomial Rolling Hash, KMP (Prefix Function), Z-Algorithm, Trie, Manacher, Suffix Automaton |
| 4 | ♟️ **Game Theory** | **60** | Nim Game, Sprague-Grundy Theorem, XOR-Sum (Nim-Sum), Minimax, Invariant Symmetry |
| 5 | 🎲 **Combinatorics & Probability** | **59** | Factorials Precomputation, $\binom{n}{r} \pmod P$, Linearity of Expectation, Inclusion-Exclusion, Catalan numbers |
| 6 | 🧩 **Constructive, Bitwise & Ad-Hoc** | **50** | Bitwise XOR/AND/OR Basis, Parity Invariants, Grid Simulation, Case Analysis |
| 7 | 📐 **Computational Geometry** | **34** | 2D Vector Cross Product, Convex Hull (Monotone Chain), Shoelace Formula, Segment Intersection |
| 8 | ⚖️ **Greedy, Two Pointers & Binary Search** | **31** | Greedy Exchange Argument, Two Pointers, Monotonic Sliding Window, Binary Search on Answer |
| 9 | 🌲 **Data Structures & Range Queries** | **9** | Segment Tree with Lazy Propagation, Fenwick Tree (BIT), Monotonic Stack/Queue, Sparse Table |
| 10| 🧠 **Dynamic Programming (DP)** | **3** | Subtree/Tree DP, Bitmask DP ($\mathcal{O}(3^N)$), Digit DP, Knapsack & Matrix Exponentiation DP |

---

## 🗂️ Folder Structure

Each contest has its own dedicated folder containing:
1. `Contest_Info.md` - Contest metadata (Date, Type, Contest Link, Standings Link, Editorial Link, Practice Link).
2. `Problemset.pdf` / `Statements.pdf` - Complete official problemset booklet for PDF-based contests.
3. Individual `Problem_<Letter>_<Title>.md` files - Formatted problem statements with LaTeX math formulas ($\LaTeX$) and sample inputs/outputs for Toph contests.

```
IUPC_Contests/
├── TOPICWISE_SOLUTIONS_AND_CATEGORIZATION.md   <-- Master Topic Guide
├── 01 - IUT IUPC 2026/
│   ├── Contest_Info.md
│   └── Problemset.pdf
├── ...
├── 18 - Inter University BUET CSE Fest 2024/
│   ├── Contest_Info.md
│   ├── Problem_A_Anya Restores Order.md
│   ├── Problem_B_Boat-Flix.md
│   └── ...
└── 62 - SUB Inter University Programming Contest 2017/
    ├── Contest_Info.md
    └── Problem_A_Buzz Lightyear.md
```

---

## 📋 Archived Contests

| # | Contest Title | Platform / Problem Format |
|:---:|---|:---:|
| 01 | IUT IUPC 2026 | Codeforces Gym / PDF |
| 02 | SUST IUPC 2026 | Codeforces Gym / PDF |
| 03 | DUET IUPC 2026 | Codeforces Gym / PDF |
| 04 | NSU IUPC 2026 | Codeforces Gym / PDF |
| 05 | NDUB IUPC 2026 | Codeforces Gym / PDF |
| 06 | BUET IUPC 2026 | Codeforces Gym / PDF |
| 07 | ICPC Asia Dhaka Regional 2025 | Codeforces Gym / PDF |
| 08 | CUET IUPC 2025 | Google Drive / PDF |
| 09 | Metropolitan University IUPC 2025 | Codeforces Gym / PDF |
| 10 | ICPC DHAKA 2025 ONLINE PRELIMINARY | GitHub Archive / PDF |
| 11 | Uttara University IUPC 2025 | Google Drive / PDF |
| 12 | DUET IUPC 2025 | Google Drive / PDF |
| 13 | AUST IUPC 2025 | Codeforces Gym / PDF |
| 14 | UIU IUPC 2025 | GitHub / PDF |
| 15 | KUET IUPC ONSITE 2025 | Google Drive / PDF |
| 16 | ICPC Dhaka Regional Site 2024 | GitHub Archive / PDF |
| 17 | ICPC PRELIMINARY DHAKA SITE 2024 | GitHub Archive / PDF |
| 18 | BUET CSE Fest 2024 IUPC | Toph (12 Problems MD) |
| 19 | IUT 11th National ICT Fest 2024 | Toph (11 Problems MD) |
| 20 | NCPC Onsite 2023 Hosted by JU | Google Docs Export / PDF |
| 21 | NCPC Preliminary JU 2023 | Google Drive / PDF |
| 22 | SUST CSE Carnival 2024 IUPC | Toph / Contest Metadata |
| 23 | CUET IUPC CodeStorm 1.0 | GitHub Archive / PDF + Toph |
| 24 | ICPC Dhaka Regional Site 2023 | Google Drive / PDF |
| 25 | ICPC Dhaka Regional Preliminary 2023 | Notion / 8 Problems MD |
| 26 | CoU-BRACNet IUPC 2023 | Toph (9 Problems MD) |
| 27 | BUET IUPC 2023 | GitHub / PDF |
| 28 | ICPC ASIA DHAKA REGIONAL 2022 | Google Drive / PDF |
| 29 | ICPC Dhaka Regional Preliminary 2022 | Google Drive / PDF |
| 30 | Cefalo SUST IUPC 2023 | Toph (10 Problems MD) |
| 31 | ICPC ASIA DHAKA REGIONAL 2021 | Google Drive / PDF |
| 32 | ICPC Dhaka Regional Preliminary 2021 | Google Drive / PDF |
| 33 | BUET IUPC 2022 | Toph (10 Problems MD) |
| 34 | AUST IUPC 2022 | Google Drive / PDF |
| 35 | RUET IUPC 2022 | Google Drive / PDF |
| 36 | ICPC Asia Dhaka Regional 2020 | Google Drive / PDF |
| 37 | ICPC Dhaka Regional Preliminary 2020 | Google Drive / PDF |
| 38 | MIST-NCPC 2020 | Google Drive / PDF |
| 39 | 2019 ICPC Dhaka Regional | Google Drive / PDF |
| 40 | NSU Cybernauts NPC 2019 | Toph (12 Problems MD) |
| 41 | LU CSE Carnival IUPC 2019 | Toph (12 Problems MD) |
| 42 | 2019 ICPC Dhaka Regional Preliminary | Google Drive / PDF |
| 43 | RUET IUPC 2019 | GitHub / PDF |
| 44 | DUET IUPC 2019 | GitHub / PDF |
| 45 | SUST IUPC 2019 | Toph (12 Problems MD) |
| 46 | BUP IUPC 2019 | GitHub / PDF |
| 47 | SUB IUPC 2019 | GitHub / PDF |
| 48 | MIST IUPC 2019 | Codeforces Gym / PDF |
| 49 | MIST IUPC 2019 (Mirror) | GitHub / PDF |
| 50 | BUET CSE Fest 2019 IUPC | Toph (11 Problems MD) |
| 51 | 2018 ACM-ICPC Dhaka Regional | Codeforces Gym / PDF |
| 52 | 2018 ACM-ICPC Dhaka Regional Preliminary | Google Drive / PDF |
| 53 | IUBAT NCPC 2018 | GitHub / PDF |
| 54 | 1st AUB IUPC 2018 | Toph (12 Problems MD) |
| 55 | BUET IUPC 2018 | Toph (13 Problems MD) |
| 56 | Cybernauts NPC 2018 | Toph (12 Problems MD) |
| 57 | IUT 9th ICT Fest 2017 | Toph (11 Problems MD) |
| 58 | 2017 ICPC Dhaka Regional | Google Drive / PDF |
| 59 | 2017 ICPC Dhaka Regional Preliminary | Google Drive / PDF |
| 60 | SUST IUPC 2017 | Toph (12 Problems MD) |
| 61 | LU IUPC 2017 | Toph (11 Problems MD) |
| 62 | SUB IUPC 2017 | Toph (12 Problems MD) |

---

## 🤝 Contributing & Community

Found an error, missing problem statement, or want to contribute alternative solution codes? Contributions and pull requests are warmly welcome!
