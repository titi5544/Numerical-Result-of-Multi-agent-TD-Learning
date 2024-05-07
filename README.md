# Numerical Result of Multi-agent TD Learning

In this project, we provide some numerical result of our paper "One-Shot Averaging for Distributed TD(λ) Under Markov Sampling". 

We test on a five-state Random Walk task. For more details please refer to Example 6.2 in Sutton and Barto (2018). 

"loss_td(0)" and "loss_td(lambda)"  shown learning curves for different number of agents, which is denoted by n. The performance measure shown in the root mean-squared (RMS) error betwee nthe value function learned and the true value function, averaged over the five states, then averaged over n agnets. 

"distance_td(0)" and "distance_td(lambda)" shown the Euclidean distance between the averaged parameters $\bar{\theta}$ and the stationary point $\theta^*$. 
