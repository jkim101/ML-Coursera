###Multivariate Linear Regression

####Multiple Features
####Gradient Descent for Multiple Variables

####Feature Scalining
- Feature Scaling
>Idea: Make sure features are on a similar scale. More generally get every feature into approximately a -1<= xi <= 1 range.

- Mean Normalization
>Replace xi with xi-mui to make features have approximately zero mean (Do not apply to x0 = 1).

####Learning Rate
* Making sure gradient descent is working correctly
>J(theta) should decrease after every iteration
- Example automatic convergence test: Declare convergence if J(theta) decreases by less than 10^-3 in one iteration. 
- But check the graph of the relationship between number of iterations and min J(theta).

