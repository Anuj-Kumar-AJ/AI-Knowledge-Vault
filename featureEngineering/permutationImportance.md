# Permutation Importance Technique 

## About

This is an ML technique, which we use to check the importance of the features in model accuracy. 

## how to use?

- split the data into training, validation and test sets.
-  now train the model with train data. now check the model accuracy using validation data.
-  now choose the feature you want to check importance. lets say it as ` checkFeature ` . now randomly shuffle the ` checkFeature ` column using numpy liberary. and again check the model accuracy after training it again.
- if the accuracy decreases from base refrence then, that feature is important for model. and if the accuracy increases then the feature is not revelant for the model.



