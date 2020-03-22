# Optimization Algorithms in Machine Learning
 
## Gradient Descent 
Goal is to visualize the parameters of Gradients and level sets in a contour plot, i.e. plotting the level sets of the objective f(x1, x2, x3)  when x1 = x∗ and to compare different values of the step size in the ALgorithm.

There are n=10 million data points. The purpose is to apply linear regression to predict y, i.e. we want to find parameters x = [x1, x2, x3].T that minimizes the least square error. Comparing the Gradient Descent with the Normal Equation - ### x∗ = ((ATA)^-1 AT) to find the parameters.

![GD plots](https://github.com/m2rik/m2rik.github.io/blob/master/images/GradientVis.png)




## Stochastic Gradient Descent
At step k, choose a data point index ik uniformly randomly from the set of all indices {1, 2, . . . , n} and consider the iterations
where we replace the gradient in the GD method with a random estimate of it.
