# Cache Cash

**URL:** https://toph.co/p/cache-cash  

---

You are a software developer in a reputed firm. For a previously written badly optimized module you want to design a caching system that will store some data which is calculated by that module. You are hoping that this cache will save a lot of time as the module isn't being used when a certain input occurs again which is already cached by your system.

You have a large collection of words and that module takes a word as input and outputs the number of similar words found in your collection.

Your cache has limited space to work with. For each request for result, you will search inside the cache and return the result. If it cannot be found, you will use the module, calculate the result and add that word and it's result in your cache. If the cache limit exceeds as a result of adding the word, you will remove the word which was last used earliest among other words present in the cache.

Now your boss wants you to write another tester module to see how much time is actually being saved by your caching system.

Input

Input start with

T ( T ≤ 5 )

, the number of test cases. Each test case starts with 3 integers.

N

, number of words,

X

, the time required by the module to output the result and

C

, the size of your cache.

( 1 ≤ N, C ≤ 100,000 ), ( 1 ≤ X ≤ 1,000,000 )

. Following

N

lines will contain

N

words, the inputs for the module. Each word will contain a maximum of

100

letters.

Output

For each case, print the case number followed by the time saved by your system.

Example


---

## Samples

### Sample Input 1
```
2
3 1 1
SUB
IUPC
2017
4 2 2
SUB
IUPC
SUB
IUPC
```

### Sample Output 1
```
Case 1: 0
Case 2: 4
```
