# Titanic-Dataset-on-Regression
## Performing Regression on Titanic Dataset and Predicting the Survival of Titanic Passengers.

### The terminology will often listen related to regression analysis is :

* Dependent variable or target variable : Variable to predict.

* Independent variable or predictor variable : Variables to estimate the dependent variable.

* Outlier : Observation that differs significantly from other observations. It should be avoided since it may hamper the result.

* Multicollinearity : Situation in which two or more independent variables are highly linearly related.

* Homoscedasticity or homogeneity of variance : Situation in which the error term is the same across all values of the independent variables.


Logistic Regression is a statistical model that in its basic form uses a logistic function to model a binary dependent variable, although many more complex extensions exist. In regression analysis, logistic regression (or logit regression) is estimating the parameters of a logistic model (a form of binary regression).

*  First, binary logistic regression requires the dependent variable to be binary and ordinal logistic regression requires the dependent variable to be ordinal.

*  Second, logistic regression requires the observations to be independent of each other.  In other words, the observations should not come from repeated measurements or matched data.

*  Third, logistic regression requires there to be little or no multicollinearity among the independent variables.  This means that the independent variables should not be too highly correlated with each other.

*  Fourth, logistic regression assumes linearity of independent variables and log odds.  although this analysis does not require the dependent and independent variables to be related linearly, it requires that the independent variables are linearly related to the log odds.

*  Finally, logistic regression typically requires a large sample size.  A general guideline is that you need at minimum of 10 cases with the least frequent outcome for each independent variable in your model.


## Introduction

* This notebook is going to be focused on solving the problem of predicting whether a passenger on the titanic would have been survived or not.

* Here, I will go through the whole process of creating a machine learning model on the famous "Titanic dataset" , which is used by many people all over the world. It provides information on the fate of passengers on the Titanic, summarized according to economic status (class), sex, age and survival.

### History of RMS Titanic

The RMS Titanic was a British passenger liner that sank in the North Atlantic Ocean in the early morning hours of 15 April 1912, after it collided with an iceberg during its maiden voyage from Southampton to New York City. There were an estimated 2,224 passengers and crew aboard the ship, and more than 1,500 died, making it one of the deadliest commercial peacetime maritime disasters in modern history. The RMS Titanic was the largest ship afloat at the time it entered service and was the second of three Olympic-class ocean liners operated by the White Star Line. The Titanic was built by the Harland and Wolff shipyard in Belfast. Thomas Andrews, her architect, died in the disaster.


### Content

* survival Survival : 0 = No, 1 = Yes

* pclass Ticket class : 1 = 1st(Upper), 2 = 2nd(Middle), 3 = 3rd(Lower)

* sex : M (Male), F (Female)

* Age : Age in years (Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5)

* sibsp : of siblings / spouses aboard the Titanic ( The dataset defines family relations in this way...)

* parch : of parents / children aboard the Titanic (The dataset defines family relations in this way...) (Parent = mother, father Child=daughter, son, stepdaughter, stepson. Some children travelled only with a nanny,therefore parch=0 for them.)

* ticket : Ticket number

* fare : Passenger fare

* cabin : Cabin number

* embarked : Port of Embarkation C = Cherbourg, Q = Queenstown, S = Southampto


### Data Visualization

![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/Age.png)


![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/sex.png)


![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/Survived.png)


![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/SexandSurvived.png)


![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/SurvivedandPclass.png)


![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/SurvivedandEmbarked.png)


![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/SibspandSurvived.png)


![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/ParchandSurvived.png)


![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/correlation.png)



![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/ROC.png)


![](https://github.com/CreatorAswin/Titanic-Regression/blob/main/Data%20Visualization/TPRvsFPR.png)
