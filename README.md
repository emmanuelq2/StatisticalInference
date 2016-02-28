# Statistical Inference - Assignment for Coursera JHU Coursera course
==================================================

This assignment has two parts:
- investigate exponential distribution in R and compare it with the Central Limit Theorem
- analyze the ToothGrowth data in the R datasets packag

1. In this project you will investigate the exponential distribution in R and compare it with the Central Limit Theorem. 
The exponential distribution can be simulated in R with rexp(n, lambda) where lambda is the rate parameter. 
The mean of exponential distribution is 1/lambda and the standard deviation is also 1/lambda. Set lambda = 0.2 for all of the simulations. 
You will investigate the distribution of averages of 40 exponentials. Note that you will need to do a thousand simulations.

Illustrate via simulation and associated explanatory text the properties of the distribution of the mean of 40 exponentials. 
You should:
* Show the sample mean and compare it to the theoretical mean of the distribution.
* Show how variable the sample is (via variance) and compare it to the theoretical variance of the distribution.
* Show that the distribution is approximately normal.

In point 3, focus on the difference between the distribution of a large collection of random exponentials and the distribution of a large collection of averages of 40 exponentials.

As a motivating example, compare the distribution of 1000 random uniforms

hist(runif(1000))

and the distribution of 1000 averages of 40 random uniforms

mns = NULL
for (i in 1 : 1000) mns = c(mns, mean(runif(40)))
hist(mns)

This distribution looks far more Gaussian than the original uniform distribution!
This exercise is asking you to use your knowledge of the theory given in class to relate the two distributions. 



2. Now in the second portion of the class, we're going to analyze the ToothGrowth data in the R datasets package.

* Load the ToothGrowth data and perform some basic exploratory data analyses
* Provide a basic summary of the data.
* Use confidence intervals and/or hypothesis tests to compare tooth growth by supp and dose. (Only use the techniques from class, even if there's other approaches worth considering)
* State your conclusions and the assumptions needed for your conclusions. 