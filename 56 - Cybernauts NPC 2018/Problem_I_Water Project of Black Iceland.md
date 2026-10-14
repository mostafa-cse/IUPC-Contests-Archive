# Water Project of Black Iceland

**URL:** https://toph.co/p/water-project-of-black-iceland  

---

Black Iceland is one of the largest populated city in this world. Due to pollution and scarcity of pure water, the government decided to store rainwater so that it can be used later. To demonstrate this, City Corporation along with the help of government and investors decided to build a large water tank. There were lots of sitting, meeting, and negotiations. Finally, they have decided to build a large water tank.

It was a large scale project and the project was supposed to be finished within 1 year. But it took three and half years to complete it. There was a big opening ceremony for this purpose. It took 3 months to complete all the preparations for the ceremony. Higher officials, businessman, investors, political leaders, electronic media and local people everyone was there. “At last, our water problem is going to be resolved”- they said.

But Alas!!! The government, City corporation and Water development board of Black Iceland started to quarrel with each other - “Who is the legal owner of this project!!!” So, residents of Black Iceland did not get any benefit and their water scarcity remained as it was.

Years passed by. Day by day water scarcity became in Black Iceland became acute. You have K taka. You want to resolve water problem as much as possible with this little amount.

The water tank is consists of N pillars. These pillars will create bunker and water is stored there. Due to gravity Water will try to move left, right and downward only. But, water can’t pass through a pillar.

The height of ith pillar is Pi.

To collect water from the ith pillar you have to set up a pipe at height (position) (Pi+1) on the ith pillar. This will create a hole and all the water that has height level more than Pi will be collected. Note that: It is possible that all the waters/some of the waters from neighboring pillars may also be collected by in this process.

It will take Ci taka to setup a pipe at ith pillar.

You have K taka budget. What is the maximum amount of water you can collect?

Input

Input starts with an integer T( ≤ 250) denoting the number of test cases.

Each of the following T test cases starts with an integer N(≤100) denoting the number of pillars in the water tank.

Next line contains N-space separated integers denoting the height of each pillar (0≤ Pi ≤100).

Next line contains N-space separated integers denoting cost of setting up pipe on each pillar (0 ≤ Ci ≤ 100).

Next line contains K(≤100) denoting your budget.

Output

For each test case print the case number followed by the maximum amount of water that you can collect. Please follow the sample input/output section for more clarity.

Example

Notes

Explanations:

Case 1: Setup pipe at the 6th pillar with the cost of 2 taka. So, the 2 units water from each of the 4th, 5th, 6th and 7th pillar will be collected. So, total 2X4 = 8 unit water will be collected.

Case 2: Setup pipe on 2nd and 4th pillar. So, all 14 units water will be collected.

Case 3: Setup pipe at 4th, 7th and 11th pillar. It will cost 3+2+2=7 taka and you will get 25 unit water in total.


---

## Samples

### Sample Input 1
```
3
8
5 3 6 1 1 3 3 5
1 2 1 3 4 2 3 4
2
8
5 3 6 1 1 3 3 5
1 2 1 3 4 2 3 4
5
16
4 6 9 3 5 7 2 9 4 6 7 12 6 8 3 1
3 2 6 3 9 8 2 3 4 5 2 7 3 2 4 2
7
```

### Sample Output 1
```
Case 1: 8
Case 2: 14
Case 3: 25
```
