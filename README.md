# 2022_SDSC8014_Paper_Summary
The paper summary of Online Learning and Optimization by Enming Liang

- [2022_SDSC8014_Paper_Summary](#2022_sdsc8014_paper_summary)
    - [Online Convex Programming and Generalized Infinitesimal Gradient Ascent](#online-convex-programming-and-generalized-infinitesimal-gradient-ascent)
      - [Main idea](#main-idea)
      - [Definitions](#definitions)
      - [Algorithm guarantee](#algorithm-guarantee)
      - [Connection with Repeated Game](#connection-with-repeated-game)
      - [Connection with Online Linear Programming](#connection-with-online-linear-programming)
      - [Conclusion remarks](#conclusion-remarks)



### Online Convex Programming and Generalized Infinitesimal Gradient Ascent
#### Main idea
1. an algorithm for general convex functions based on gradient descent
   1. simple, 
   2. general, handle an arbitrary sequence of convex functions
   3. in some circumstances perform better than an experts algorithm
2. background:
   1. infinitesimal gradient ascent
   2. repeated games
 
#### Definitions
1. Online convex programming
![](pic/2022-01-28-14-35-06.png)
2. Greedy Projection
![](pic/2022-01-28-14-36-07.png)
3. Lazy Projection
![](pic/2022-01-28-14-53-54.png)
4. Performance
   1. online performance
![](pic/2022-01-28-14-40-03.png)
   2. offline static benchmark
![](pic/2022-01-28-14-40-14.png)
   1. regret 
![](pic/2022-01-28-14-40-33.png)
   1. dynamic regret (dynamic offline strategy with path constraints)
![](pic/2022-01-28-14-48-44.png)

#### Algorithm guarantee
1. regret bound
![](pic/2022-01-28-14-41-50.png)
2. dynamic regret bound
![](pic/2022-01-28-14-51-10.png)
3. regret bound for lazy projection
![](pic/2022-01-28-14-55-16.png)


#### Connection with Repeated Game
1. Repeated Game
    1. action: player A and environment Y
    2. history: sequence of joint actions
![](pic/2022-01-28-14-58-00.png)
    3. utility: 
![](pic/2022-01-28-14-58-36.png)
    4. regret of not playing action a
![](pic/2022-01-28-15-00-25.png)
    5. behavior: mapping from history to action probability
![](pic/2022-01-28-15-03-38.png)
    6. oblivious deterministic environment: 
       1. plays the same sequence of actions regardless of the actions of the player
2. Repeated Game as an Online Linear Program
![](pic/2022-01-28-15-17-07.png)
   1. greedy projection:
![](pic/2022-01-28-15-26-11.png)
   1. Lazy Projection and Fictitious Play
![](pic/2022-01-28-15-31-32.png)

#### Connection with Online Linear Programming
1. Expert problem
   ![](pic/2022-01-28-15-32-40.png)
2. EA as online linear programming
![](pic/2022-01-28-15-49-56.png)
3. online linear as online convex


#### Conclusion remarks
1. Presenting a gradient based algorithm for online convex programming 
   1. derive regret bound for different projection-based algorithm
2. Building its connection with Repeated Game and Fictitious Play
   1. prove universal consistency
3. Converting expert algorithm -> online linear programming -> online convex programming

