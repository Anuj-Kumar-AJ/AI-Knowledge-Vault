# normalization of features .

## what does normalization in feature engineering means and why do we use it.

feature normalization is a technique which we use so that all the features contribute equally in algorithm to give certain output.

okay this may sound gibberish right. let me explain it with example/


So lets say we have to predict if  a person will buy an house or not. 
the feature we have given is **Salary** and **Year of Experence** 

example

----------------------------------------------------
salary| 10000 | 20000 | 30000|
---------------------------------------------------- 
YoE   |  1    | 2     | 5    |
----------------------------------------------------

okay we can use model like linear regression to get the answer, what the preoblem in that, why do we need to normalize it.

the problem is that our model is just an mathematical machine, they dont have intution, that salary and year of exprence both have diffrerent unit. means one is calculated in rupees/Dollar(salary) and other is calculated in bases of years(YoE).

So the weight both features is given will be different , as our ML model will think that Salary is much more imortant then YoE as it have high vales.


## Normalization Technique


Okay now i guess you get why we need the normalization technique. but how can we normilize it.

Common methods of feature normalization include:

    Min-Max Scaling: This method scales the features to a specific range, often between 0 and 1. The formula for min-max scaling is:

    Xnormalized= (X-min(X)​) / (max(X)-min(X))

    Standardization (Z-score normalization): This method transforms the data to have a mean of 0 and a standard deviation of 1. The formula for standardization is:

    Xstandardized= X-min(X) / std(X)


lets take example of min-max scaling 

salary is 10000, 20000, 30000
minimun value of salary min(X) = 10000
maximum value of salary is max(X) = 30000

salary ofter normalize is | (10000-10000)/30000-10000 | (20000-10000)/30000-10000 | (30000-10000)/30000-10000

i.e ->  0 | 0.5 | 1


so now our salary is normalized . similarly we will do all the normalization to every features.



