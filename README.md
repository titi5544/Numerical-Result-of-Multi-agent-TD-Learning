# Numerical Result of Multi-agent TD Learning

In this project, we provide some numerical result of our paper "One-Shot Averaging for Distributed TD(λ) Under Markov Sampling". 

We test on a five-state Random Walk task. For more details please refer to Example 6.2 in Sutton and Barto (2018). 

TD(0):

The following graph shows learning curves for different number of agents, which is denoted by n. The performance measure shown in the root mean-squared (RMS) error betwee nthe value function learned and the true value function, averaged over the five states, then averaged over n agnets. One can conclude from the graph that all the method will converge with a faster convergence is achieved with a greater n, which basically matches what we have in the paper. 

![](loss_td(0).png)

The following graph shows the Euclidean distance between the averaged parameters $\bar{\theta}$ and the stationary point $\theta^*$. One can conclude that the convergence is basically n times faster compared with the case n=1. 

![](distance_td(0).png)

TD($\lambda$):

The save result applied for TD($\lambda$), where $\lambda$ is chosen to be 0.5. The first figure is the learning curve and the second figure is the distance. 

![](loss_td(lambda).png)

![](diatance_td(lambda).png)
