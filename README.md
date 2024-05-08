# Numerical Result of Multi-agent TD Learning

In this project, we provide some numerical result of our paper "One-Shot Averaging for Distributed TD(λ) Under Markov Sampling". 

We test on a five-state Random Walk task. There are five states in a row, named A, B, C, D, and E, from left to right. All episodes start in the center state, C, then proceed either left or right by one state on each step, with equal probability. Episodes terminate either on the extreme left or the exterme right. When an episode terminates on the right, a reward of +1 occurs; all other rewards are zero. The true value of all the states, A through E, are 1/6, 2/6, 3/6, 4/6, and 5/6. For more details please refer to Example 6.2 in Sutton and Barto (2018). 

We test two algorithm on this task, TD(0) and TD($\lambda$). The stepsize is chosen to be 1e-3 and both algorithm will run 100 episode. 

TD(0):

The following graph shows learning curves for different number of agents, which is denoted by n. The performance measure shown in the root mean-squared (RMS) error betwee nthe value function learned and the true value function, averaged over the five states, then averaged over n agnets. One can conclude from the graph that all the method will converge with a faster convergence is achieved with a greater n, which basically matches what we have in the paper. 

![](loss_td(0).png)

The following graph shows the Euclidean distance between the averaged parameters $\bar{\theta}$ and the stationary point $\theta^*$. One can conclude that the convergence is basically n times faster compared with the case n=1. 

![](distance_td(0).png)

TD($\lambda$):

The save result applied for TD($\lambda$), where $\lambda$ is chosen to be 0.5. The first figure is the learning curve and the second figure is the distance. 

![](loss_td(lambda).png)

![](distance_td(lambda).png)
