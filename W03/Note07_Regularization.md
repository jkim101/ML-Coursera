#Regularization
##Solving the Problem of Overfitting

###The Problem of Overfitting
>Overfitting: If we have too many features, the learned hypothesis may fit the training set very well, but fail to generalize to new examples (predict prices on new examples).


__Addressing overfitting__

[Options]

1. Reduce number of features
  - Manually select which features to keep
  - Model selection algorithm
2. Regularization
  - Keep all the features, but reduce magnitude/values of parameters theta(j)
  - Works well when we have a lot of features, each of which contributes a bit to predicting y.


###Cost Function
>Intuition: Suppose we penalize and make theta(3) and theta(4) really small.

__Regularization__

Small values for parameters theta(0) ~ theta(n)
- "Simpler" hypothesis
- Less prone to overfitting

__Regularization Term and its parameter__

>Two goals of regularization term are..

> 1. Fit the training data well

> 2. Keep the parameters samll


> __Lambda__ plays a role of controlling the trade between these two goals.

###Regularized Linear Regression

###Regularized Logistic Regression
