# Logistic-Regression
Classification using Logistic-Regression.

This type of statistical model (also known as logit model) is often used for classification and predictive analytics. Logistic regression estimates the probability of an event occurring, such as voted or didn’t vote, based on a given dataset of independent variables. Since the outcome is a probability, the dependent variable is bounded between 0 and 1. In logistic regression, a logit transformation is applied on the odds—that is, the probability of success divided by the probability of failure.

Because of sigmoid function's property to give output between 0 and 1, we can use its output like a probability, but not exactly as probability. For example, the property of probability that P(true) + P(false) = 1 may not be true is case of sigmoid function i.e. S(true) + S(false) may not be equal to 1.

This is also commonly known as the log odds, or the natural logarithm of odds, and this logistic function is represented by the formula, Logit(pi) = 1/(1+exp(pi))

The logistic function has this further, important property, that its derivative can be expressed by the function itself,
𝑆′(𝑡)=𝑆(𝑡)(1−𝑆(𝑡))
As at t = 0 we have  𝑆(𝑡)=0.5  , and for t > 0 we have  𝑆(𝑡)>0.5  (sharply rising to 1 so we consider it 1) and for t < 0 we have  𝑆(𝑡)<0.5  (sharply falling to 0 so we consider it 0) , we have our decision boundary as 0.5.

For example, if our threshold is 0.5 and our prediction function returned 0.7, we would classify this observation as 'positive' (1). If our prediction was 0.2 we would classify the observation as 'negative' (0).

For logistic regression with multiple classes we could select the class with the highest predicted probability.

Observe the image below for better understanding :


![s4-7069](https://user-images.githubusercontent.com/63576861/203704527-25ba2043-f1b7-4005-8852-40e1945381b4.png)

The Titanic dataset:-

The Titanic data set is a very famous data set that contains characteristics about the passengers on the Titanic. It is often used as an introductory data set for logistic regression problems.

In this project, I used the Titanic data set combined with a Python logistic regression model to predict whether or not a passenger survived the Titanic crash.
The original Titanic data set is publicly available on Kaggle.com, which is a website that hosts data sets and data science competitions.
To make things easier for me as a student, I used a semi-cleaned version of the Titanic data set, which saved my time on data cleaning and manipulation.

   These are the names of the columns in the DataFrame. Here are brief explanations of each data point:-
          
          PassengerId: a numerical identifier for every passenger on the Titanic.
          
          Survived   : a binary identifier that indicates whether or not the passenger survived the Titanic crash. This variable will hold a value of 1 if they                                  survived and 0 if they did not.
          Pclass     : the passenger class of the passenger in question. This can hold a value of 1, 2, or 3, depending on where the passenger was located in the                                ship.            
          Name       : the passenger's name.
          Sex        : male or female.
          Age        : the age (in years) of the passenger.
          SibSp      : the number of siblings and spouses aboard the ship.
          Parch      : the number of parents and children aboard the ship.
          Ticket     : the passenger's ticket number.
          Fare       : how much the passenger paid for their ticket on the Titanic.
          Cabin      : the passenger's cabin number.
          Embarked   : the port where the passenger embarked (C = Cherbourg, Q = Queenstown, S = Southampton)
