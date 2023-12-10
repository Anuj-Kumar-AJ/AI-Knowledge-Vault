# about Feature engineering

To understand about why do we need feature engineering, we need to understand about machine learning models.


## What is ML models?

you have heard many ml models like, 
    - regressing model (like linear regression, logistic regression)
    - classification model ()
    - clustring models (k means clustring)
    - nural networks models etc.

but what these models are? they are just a generlised version of mathematical function. for example you have larned about polynomial function in mathematics during your stay in  middle school . it goes like


 f(x) = a<sub>n</sub>x<sup>n</sup> + a<sub>n-1</sub>x<sup>n-1</sup> + ... + a<sub>2</sub>x<sup>2</sup> + a<sub>1</sub>x + a<sub>0</sub> 


so basically `f(x) = target`. meaning we give the features matrics to a mathematical function which is f(x) and it gives us value which is as close as target value. 

## but why need feature enginerring ?

here you can say that features is saperated with `+` symbol.

lets take an example where we have feature (or in mathematical term `x`) and have target (or in mathematical tem `y`).

our data is like (x1 = x,  y) = (0,0), (1,1), (2,4), (3,9), (4,16)

so as we can observe from our data that .   y = x<sup>2</sup>

but lets say we have choosen a linear regrssion model for this problem , which is bassicaly a linear relation between x and y parameters. so we can train our model as much as we want but we cant get best result. as we are trying f(x) = x. but with our data we need f(x) = x<sup>2</sup>. 

so to tackle this problem we need a new feature which follows a linear relation with our target value. i.e we need to give feature as x<sup>2</sup>. 

so our data which we feed to model will be like (x2 = x<sup>2</sup>  ,y) = (0,0), (1,1), (4,4), (9,9), (16,16)


the difference from before will be here model will get leaner relation from feature and target value. hence we get much optimal model then before.



## how to choose if new feature we created, made better model or not ?

to do to that we have to first train our model on given training dataset. and check the score using validation dataset.

now add the newly created feature, in your previous datasets. by creating new column x[newCol] = [mathematicalExpressionOnPreviousFeature].

eg given dataset `D1 = [feature1, feature2, feature3, target]

newly created dataset

 `D2 = `[feature1, feature2, feature3,feature1*feature2, Feature1/feature3, target]



Okay this is great but there is problem lies in this approch can you guess? 

what will you do if we got a dataset that we have no knowledge before about it, how can we guess which feature is good, or which feature we should multiply like before.
or if we have given a dataset with 100000 features. how can we check which feature impact the target score more , or which is most important features in this.

## well these is a solution for this problem

the answer lies in  Discovering useful features with `mutual information`.