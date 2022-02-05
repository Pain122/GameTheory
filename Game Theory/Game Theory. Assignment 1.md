# Game Theory. Assignment 1

## Question 1. 

Considering the following game:

![image-20210212152549107](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210212152549107.png)

### a. Does either player have a dominant strategy?

For a strategy to be dominant, it must dominate every other strategy of the player. None of the players Have dominant strategies, and this is why:

1) Player1's strategy A dominates strategy C but does not dominate other strategies. Strategy D dominates strategy B but  does not dominate other strategies. Strategies B and C are dominated, so they can not possibly be dominant.

2) None of Player2's strategies dominate any other strategies, so there are no dominant strategies.

### b. Does either player have a dominated strategy?

For a strategy to be dominated, it needs to be dominated by at least one strategy.

1) Player1's strategies C and B are strictly dominated strategies, because they are dominated by strategies  A and D respectively.

2) Since none of the strategies of Player2 dominate other strategy, he does not have any dominated strategy.

### c. Give the equilibrium of the game and show the process.

To find the equilibrium of the game, we need to apply the Iterated Elimination of Strictly Dominated Strategies. On the first step, we will eliminate strategies C and B of the Player1 as established in the previous task:

![image-20210212154202653](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210212154202653.png)

The resulting matrix will be:

![image-20210212154244014](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210212154244014.png)

Now, strategies A and C of Player2 is strictly dominated by strategy D. Let us eliminate them:

![image-20210212154453610](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210212154453610.png)

The resulting matrix will be:

![image-20210212154831020](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210212154831020.png)

Strategy A of the Player1 now strictly dominates strategy D:

![image-20210212154904110](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210212154904110.png)

The resulting matrix is:

![image-20210212154927888](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210212154927888.png)

Finally, strategy B of the Player2 strictly dominates strategy D :

![image-20210212155014682](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210212155014682.png)

And the equilibrium is:

![image-20210212155035637](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210212155035637.png)

## Question 2

The very first thing we need to notice is the fact we can unite Pfizer/BioNTech and AstraZeneca to a single player as:

1. In case Sputnik V is allowed to be sold, they BOTH leave the market as a single player leaving them 0 profit.
2. There is no case when the profit of the company producing Pfizer/BioNTech goes negative which could somehow affect other decisions. The lowest profit is in case of duopoly and is equal to 27 (from REEC gov. decision) -10 (for transportation) =17 millions.

###  2.a)

Here is the payoff table we will use for the game:

![image-20210213234344806](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210213234344806.png)

Later on, all of the profits and losses will be presented in millions of dollars with the units omitted.

### 2.b) 

There are 3 decisions of 3 different players in this game:

1. REEC decides to buy Sputnik V or not
2. Sputnik V decides to make advertisement or not
3. Pfizer/BioNTech and AstraZeneca decide to leave REEC market if REEC decides to buy Sputnik

We will assume the events occur in the order 1 - 3 - 2. Also, Sputnik team may decide to promote even if REEC does not accept it, if for instance,  they assume Sputnik may be accepted later

#### The second tree, events in the order 1-3-2

Here is the resulting tree:

![image-20210223140933353](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210223140933353.png)

Now, let us calculate the outcomes:

##### 1)![image-20210214093925536](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210214093925536.png)

##### 2) ![image-20210214094012013](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210214094012013.png)

##### 3)![image-20210214094123507](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210214094123507.png)

##### 4)![image-20210214094148987](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210214094148987.png)

##### 5)![image-20210223141108257](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210223141108257.png)

##### 6)![image-20210214094326413](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210214094326413.png)

The resulting tree (The outcomes are in form (REEC; Sputnik; Pfizer+Astra)):

![image-20210224121852276](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210224121852276.png)

Thinking backwards, the first choice we will consider is the choice of Sputnic V. It is clear that making an advertisement benefits company more than not making it in case REEC accepts Sputnik. If it does not, there is no need for advertisement:

![image-20210223141303374](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210223141303374.png)

The second decision is done by Pfizer/BioNTech+AstraZeneca. For them, it is better not to choose to leave the market:

![image-20210223141347782](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210223141347782.png)

And the last one, for REEC government it is more beneficial to choose to accept Sputnic V. So we get the result:

![image-20210223141409905](C:\Users\pavel\AppData\Roaming\Typora\typora-user-images\image-20210223141409905.png)

Answer: (50; 125; 50)

It can also be shown that changing sequences of events yields no difference in the result.

## Question 3

What are the best strategies in Iterated Prisoner’s Dilemma in case of 2 players and in case of many players?

1. Case of 2 players
   1. If the number of turns N is known by the players, the best strategy would be to defect (betray or spill the beans) each round as it is proven by induction. On the last round opponent will always defect, therefore I should also defect. On the second to last round opponent will have the last chance to defect, therefore I should also defect and so on
2. In case of many players, we assume that the game is played among M players. Each time players compete with the others for at most N rounds and then switch places
   1. For this game, the best strategy found was tit-for-tat, or cooperating on the first round and then doing the same action an opponent did in the previous round [1], [2]
   2. However, this strategy fails in case of some unknown defects in making turns, when one player mixes two strategies and, for instance, defects on their turn. In this case, forgiving tit-for-tat is more suitable (1-5% of cooperate if someone defects) and is proven by simulations [2]
   3. There are also studies showing emerging strategies and previous ones that outplay tit-for-tat, such as gradual ("Cooperates on the first move, then defect n times after  n th defections of its opponent, and calms down with 2 cooperations"), spiteful tit-for-tat (plays tit-for-tat until two defects, then always defects). [3] 

## Question 4

2







## References

1. Wikipedia contributors. (2021, February 18). *Prisoner’s dilemma*. Wikipedia. https://en.wikipedia.org/wiki/Prisoner%27s_dilemma#Strategy_for_the_prisoner’s_dilemma
2. *The Evolution of Trust*. (2017, July). The Evolution Of Trust. https://ncase.me/trust/
3. Mathieu, Philippe and Delahaye, Jean-Paul (2017) 'New Winning Strategies for the Iterated Prisoner's Dilemma' Journal of Artificial Societies and Social Simulation 20 (4) 12 <http://jasss.soc.surrey.ac.uk/20/4/12.html>. doi: 10.18564/jasss.3517