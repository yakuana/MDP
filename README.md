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

    A. The Discount Factor

 | Discount Factor | Number of Iterations |
 | -- | -- |
 | 0.1 | 5 |
 | 0.4 | 12 |   
 | 0.7 | 10 |  
 | 1.0 | 41 | 


    B. The Step Cost

 | Step Cost | Number of Iterations |
 | -- | -- |
 | -10.0 | 23 |
 | -0.04 | 22 |       
 | 0.0 | 138 | 
 | 0.04 | 895 | 

        Explaination: 

    C. The Negative Reward

 | Negative Reward | Number of Iterations |
 | -- | -- |
 | -1.0 | 22 |
 | -10.0 | 140 |   
 | -100.0 | 140 | 

        Explaination:

    D. The Positive Reward

 | Positive Reward | Number of Iterations |
 | -- | -- |
 | 1.0 | 22 |
 | 10.0 | 136 |   
 | 100.0 | 165 | 

        Explaination:
