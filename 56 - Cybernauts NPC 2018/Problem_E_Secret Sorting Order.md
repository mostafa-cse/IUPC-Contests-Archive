# Secret Sorting Order

**URL:** https://toph.co/p/secret-sorting-order  

---

You will be given a list of words which were sorted based on some unknown ordering among the letters of the alphabet, very likely to be different from regular Latin lexicographic order. Your task is to find the correct ordering of all the letters from the given words.

It is guaranteed that there will always be exactly one valid ordering of letters that satisfies the sorting order of words.

Input

First line of input contains an integer T, the number of test cases, not exceeding 100.

First line of each test case contain an integer N, the number of words. Here, N <= 100. Each of the following N lines contain one word, consisting of at most 15 lowercase Latin letters ('a' to 'z').

Output

For each test case, print the letters in correct order to satisfy the sorting order of words in one line, separating by single space character.

Example


---

## Samples

### Sample Input 1
```
1
20
qdddklkk
qdddklkn
qlkln
qlkkdl
qlknddq
qlknnnqndk
qlnkl
qklkqnkq
qklkfflql
dnkln
dnkndlq
dnkndkdkqf
dnknfnn
dnnffq
dnnfffl
dnnffk
dnnflqq
dnnfll
dnnflln
dnnflkdf
```

### Sample Output 1
```
q d f l k n
```
