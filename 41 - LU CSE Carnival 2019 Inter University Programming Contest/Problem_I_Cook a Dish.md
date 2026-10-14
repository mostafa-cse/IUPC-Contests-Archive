# Cook a Dish

**URL:** https://toph.co/p/cook-a-dish  

---

Have you ever cooked something? No? Not a problem! Whenever you try to cook something, you need some ingredients, obviously with some water, oil and heat. May be finally you will manage to cook the dish you wanted. But I am not sure if you will dare to taste it! 😉

Here, you are given some ingredients, you need to tell me how many different recipes are possible from the ingredients? Ingredients will be given as a string S consisting of digits (0-9) where each digit is an ingredient. A recipe is a mixture of some unique ingredients. So, you need to pick up exactly D ingredients from the ingredients in string S to make a recipe. Also, there is a restriction that you can’t use ‘0’ as the first ingredient of a recipe. And keep in mind ‘240’ and ‘420’ are different recipes.

Now, can you tell me how many recipes you can make using D ingredients from the ingredients given in string S?

Input

The first line will contain

T

(1 ≤ T ≤ 100), denotes the number of test cases. Next T lines will contain a string

S

(1 ≤ |S| ≤ 10), which holds the ingredients and no ingredient will come more than once, and

D

(1 ≤ D ≤ |S|) .

Output

Print the number of possible recipes.

Example


---

## Samples

### Sample Input 1
```
2
1235 3
490 2
```

### Sample Output 1
```
24
4
```
