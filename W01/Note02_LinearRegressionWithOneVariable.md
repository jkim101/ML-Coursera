##Linear Regression with one variable


###Model and Cost Function
- Supervised Learning: Given the "right answer" for each example in the data
- Unsupervised Learning: Predict real-valued output


####Model Representation
- A pair of input variable and target variable is called a 'training example'. A list of training examples is called a 'training set'.

'Hypothesis' <-- Call this for historical reason, not fit on ML (Andrew said).

Types of Problems
>Predict continuous things... call the learning problem a 'regression problem'.
>Predict (a smally number of) discrete values of y, it could be a 'classification problem'.

Linear Regression with one variable = Univariate linear regression

####Cost Function, J
Idea: Choose \theta 0, \theta 1 so that h(x) is close to y for our training examples (x, y)

In univariate linear regression, h(x) comes with x (power 1).

>So, overall goal is to minimize cost function J by changing 'theta's.....

####Cost Function Intuition I and II
>Think the relationship between h(x) and J(\theta)


###Parameter Learning

####Gradient Descent and Intuition
Check the 'Gradient Descent Algorithm'
>:= 'Assignment Sign'
>alpha - learning rate
>'(for j = 0 and j = 1)' means 'Simultaneously Update theta0 and theta1

- Sign of 'alpha': Positive vs Negative
- Value of 'alpha': Small vs Large (step size)

>If the learning rate 'alpha' fixed, as we approach a local minimum, gradient descent will automatically take smaller steps. So, no need to decrease 'alpha' over time.
