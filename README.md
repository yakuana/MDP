# MDP
Markov Decision Process

CS 2400 FALL 2020

ASSIGNMENT 5: MARKOV DECISION PROCESSES

Kayla Stuhlmann and Ya'kuana Davis 

## Experiment Results: 
1. How many iterations does Value Iteration need to solve this problem? Use a discount
factor of 0.99, a maximum state error of 1e-6, a positive terminal state reward of +1,
a negative terminal state reward of −1, and a step cost of −0.04.

    It takes 22 iterations for Value Iteration to solve this problem with a discount factor of 0.99, a maximum state error of 1e-6, a positive terminal state reward of +1, a negative terminal state reward of -1, and a step cost of -0.04.

2. The number of iterations in the previous question is what was needed to reduce the
state error to the specified level. How many iterations does it actually take before the
policy is optimal?

    It takes 12 iterations before the policy is optimal. 

3. Measure the effect of the following factors on the policy arrived at. Test the values
suggested. When testing a given parameter, hold the other parameters constant at
the values used in the previous experiment. For each parameter, describe its impact
on the policy. Note that different values of a given parameter may produce the same
policy. 


#### The Discount Factor

 | Discount Factor | Number of Iterations |
 | -- | -- |
 | 0.1 | 5 |
 | 0.4 | 12 |   
 | 0.7 | 10 |  
 | 1.0 | 41 | 

    Explaination: Excluding the outlier of a discount factor of 0.7, the trend reflects an increase in discount factor leads to an increase in the number of iterations neccessary to solve the problem. The higher the discount factor, the more iterations neccessary for the following comparison to be true and halt the Markov Decision Process: utilityChange <= EPSILON * (1 - DISCOUNT_FACTOR) / DISCOUNT_FACTOR 

#### The Step Cost

 | Step Cost | Number of Iterations |
 | -- | -- |
 | -10.0 | 23 |
 | -0.04 | 22 |       
 | 0.0 | 138 | 
 | 0.04 | 895 | 

    Explaination: 
    -10 is significantly greater than the positive and negative rewards we have provided. As a result, the agent actively seeks a terminal state, even if the terminal state provides a negative reward.
    
    -0.04 is a reasonable step cost. Given this step cost, the agent will reach a positive reward in a fair amount of time given the low risk of taking any step. 
    
    No step cost results in the agent having 0 probability of landing in the negative reward terminal state and eliminates some relatively shorter paths to the positive reward as reflected in the large number of iterations required to reach the solution.
    
    0.04 is the most positive step cost in the list. Given this step cost, the agent will avoid both the positive and negative terminal states in order to increase its total amount of rewards before reaching the solution. 


#### The Negative Reward

 | Negative Reward | Number of Iterations |
 | -- | -- |
 | -1.0 | 22 |
 | -10.0 | 140 |   
 | -100.0 | 140 | 

    Explaination:
        

#### The Positive Reward

 | Positive Reward | Number of Iterations |
 | -- | -- |
 | 1.0 | 22 |
 | 10.0 | 136 |   
 | 100.0 | 165 | 

    Explaination:
