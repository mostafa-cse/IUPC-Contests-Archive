# Modified Linear Regression

**URL:** https://toph.co/p/modified-linear-regression  

---

Mr X is a real state business magnate. He hired you to write program for predicting housing prices.

A house can contain many features like – Total area of land, number of windows etc. To be discrete, let’s assume a house has N features and the features are represented as – X1, X2, X3, ….., XN and the price of the house is denoted as Y. Mr X wants you to use this given modified version of the linear regression equation to solve the problem –

D1X1 + D2X2 + D3X3 + ……. + DNXN = Y

Here, the values of D1 through DN must be calculated from a given training set represented by a N*(N+1) matrix whereby, the first N integers in each row are the values of N features of a house and the (N+1)’th integer is its price Y. After that, a test set represented by a K*N matrix will be given as input in which, K is the number of houses in the test set and each row represents the values of N features of a house. Your program shall output the predicted price of the houses using the given modified linear regression equation above.

Note: there is no singular matrix in the input.

Input

The first line of input will contain two integers N (1 <= N <= 103) and K (1 <= K <= 103) denoting the number of features of each house and the number of houses in the test set. Then there will be a N*(N+1) matrix of integers representing the training set and a K*N matrix of integers representing the test set. The first N integers in the i'th row of the training set represent the feature values X1 through XN (1 <= Xj <= 102) of the i'th house of training set and the (N+1)’th value represents it's price Y (1 <= Y <= 107). Similarly, the i'th row in the test set describes the feature values X1 through XN (1 <= Xj <= 102) for the i'th house whose price needs to be predicted.

Output

Print K integers in K separate lines where the i’th integer is the predicted price of the i’th house of the test set.

Examples


---

## Samples

### Sample Input 1
```
2 3
5 3 110
3 2 70
5 6
3 2
1 1
```

### Sample Output 1
```
170
70
30
```

### Sample Input 2
```
2 5
35 1 1538 
70 25 4640 
79 59 
63 65 
6 46 
82 28 
62 92
```

### Sample Output 2
```
7330
7066
3380
5348
8860
```
