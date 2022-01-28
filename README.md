# 2022_SDSC8014_Paper_Summary
The paper summary of Online Learning and Optimization by Enming Liang


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
![](2022-01-28-14-35-06.png)
2. Greedy Projection
![](2022-01-28-14-36-07.png)
3. Lazy Projection
![](2022-01-28-14-53-54.png)
4. Performance
   1. online performance
![](2022-01-28-14-40-03.png)
   2. offline static benchmark
![](2022-01-28-14-40-14.png)
   1. regret 
![](2022-01-28-14-40-33.png)
   1. dynamic regret (dynamic offline strategy with path constraints)
![](2022-01-28-14-48-44.png)

#### Algorithm guarantee
1. regret bound
![](2022-01-28-14-41-50.png)
2. dynamic regret bound
![](2022-01-28-14-51-10.png)
3. regret bound for lazy projection
![](2022-01-28-14-55-16.png)


#### Application
1. Repeated Game
    1. action: player A and environment Y
    2. history: sequence of joint actions
![](2022-01-28-14-58-00.png)
    3. utility: 
![](2022-01-28-14-58-36.png)
    4. regret of not playing action a
![](2022-01-28-15-00-25.png)
    5. behavior: mapping from history to action probability
#### 

