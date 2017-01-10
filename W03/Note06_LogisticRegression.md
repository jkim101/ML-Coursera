##Classification and Representation
###Classification

###Hypothesis Representation

###Decision Boundary


##Logistic Regression Model
###Cost Function


###Simplified Cost Function and Gradient Descent


###Advanced Optimizationn

```
theta = zeros(2,1);  %declare initial theta

function [jVal, gradient] = costFunction(theta)
  jval = (theta(1) - 5) ^ 2 + (theta(2) - 5) ^ 2;
  gradient = zeros(2, 1); %Declare initial gradient
  gradient(1) = 2*(theta(1) - 5);  %code to compute derivative of J(theta(1))
  gradient(2) = 2*(theta(2) - 5);  %code to compute derivative of J(theta(2))
end;

options = optimset('GradObj', 'on', 'MaxIter', '100');
initialTheta = zeros(2, 1);
[optTheta, functionVal, exitFlag] ... = fminunc(@costFunction, initialTheta, options);
```
