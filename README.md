After importing necessary libraries for the model creation and hyper parameter
tuning, the data frame is being read from the file “Call.csv”. 

After evaluating the “Churn” of the customers, it can the said that given samples are 
unbalanced thus preprocessing is needed. I have done this
by using SMOTE and pipelines, because as we do cross validation of the models, data 
leakage is a very possible risk that can make the all evaluations worthless.

By implementing the smote and pipelines into classification models I was able to evaluate the 
“Accuracy Score” and “ROC AUC Score” of the models. 

By doing comparison between the Accuracy and the ROC AUC scores of the models I was able to see that Random Forest has performed best 
among Decision Tree, Bagging, Addaptive Boosting and Gradient boosting.

In the second part of the process I focused on improving the accuracy of Random Forest model.
To have a benchmark I decided to use the original model as the base line. I decided to use three different 
hyper parameter tuning methods which are, manual hyper parameter tuning, grid search hyper parameter tuning and randomized search.

Although the manual tuning the model resuleted in worse results(which was expected), I was able to increase the
model accuracy with grid search and random search algorithms. While random search algorithms was able to increase 
the model accuracy by 1.53851%, the grid search algorithms was able to increase the model accuracy by 1.6084%.

Eventhough I was able to get a better result by grid search method, it was a computationally heavy process 
and it took approximately 15 minutes to compute the optimal hyper paramaters.


