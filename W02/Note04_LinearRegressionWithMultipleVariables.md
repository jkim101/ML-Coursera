###Multivariate Linear Regression

####Multiple Features
####Gradient Descent for Multiple Variables

####Feature Scalining
- Feature Scaling
>Idea: Make sure features are on a similar scale. More generally get every feature into approximately a -1<= xi <= 1 range.

- Mean Normalization
>Replace xi with xi-mui to make features have approximately zero mean (Do not apply to x0 = 1).

####Learning Rate
- Making sure gradient descent is working correctly
>J(θ) should decrease after every iteration
- Example automatic convergence test: Declare convergence if J(θ) decreases by less than 10^-3 in one iteration. 
- But check the graph of the relationship between number of iterations and min J(θ).

> If alpha is too small: slow convergence
> If alpha is too large: J(θ) may not decrease on every iteration; may not converge.

####Features and Polynominal Regression
- Select the correct feature.. to fit on the data -- square? cubic? squareroot? etc...
    
    We can improve our features and the form of our hypothesis function in a couple different ways.
    We can combine multiple features into one. For example, we can combine x1 and x2 into a new feature x3 by taking x1⋅x2.

- Polynomial Regression
    
    Our hypothesis function need not be linear (a straight line) if that does not fit the data well.We can change the behavior or curve of our hypothesis function by making it a quadratic, cubic or square root function (or any other form).
    
    For example, if our hypothesis function is hθ(x)=θ0+θ1x1 then we can create additional features based on x1, to get the quadratic function hθ(x)=θ0+θ1x1+θ2x21 or the cubic function hθ(x)=θ0+θ1x1+θ2x21+θ3x31
    
    In the cubic version, we have created new features x2 and x3 where x2=x21 and x3=x31.
    To make it a square root function, we could do: hθ(x)=θ0+θ1x1+θ2x1−−√
    
    One important thing to keep in mind is, if you choose your features this way then feature scaling becomes very important. (eg. if x1 has range 1 - 1000 then range of x21 becomes 1 - 1000000 and that of x31 becomes 1 - 1000000000)


###Computing Parameters Analytically
####Normal Equation
>Normal Equation: Method to solve for θ analytically.

Octave: pinv(X'*X)*X'*y

>*Check pros and cons of Gradient Descent vs Normal Equation
>- Gradient Descent: Need to choose 'alpha'; Needs many iterations; Works well even when n is large.
>- Normal Equation:No need to choose 'alpha'; Don't need to iterate; Need to compute (X'X)-1; Slow if n is very large.

####Normal Equation Noninvertibility
Octave: pinv(X'*X)*X'*y 
>Reduntant featurs, where two features are very closely related
>Too many features: Delete some features, or use regularization
