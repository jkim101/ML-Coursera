##Classification and Representation
###Classification

###Hypothesis Representation

###Decision Boundary


##Logistic Regression Model
###Cost Function


###Simplified Cost Function and Gradient Descent


###Advanced Optimizationn

function [jVal, gradient] = costFunction(theta)
jval = (theta(1) - 5) ^ 2 + (theta(2) - 5) ^ 2;

gradient = zeros(2, 1);
gradient(1) = 2*(theta(1) - 5);
gradient(2) = 2*(theta(2) - 5);

options = optimset('GradObj', 'on', 'MaxIter', '100');

initialTheta = zeros(2, 1);

[optTheta, functionVal, exitFlag] ... = fminunc(@costFunction, initialTheta, options);

