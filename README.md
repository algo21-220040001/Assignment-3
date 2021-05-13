# Assignment-3

This assignment follows the logic of multi-factor machine learning stock selection in research reports, and instead uses factors from different varieties of futures as features to build the model.  
The features are 84 factors of each variety of futures on the daily frequency, labeled with the daily return of each variety, and trained using the xgboost module. 
The data is rolled over every six months and each set is cross-trained five times for a total of 40 models. 
The test set predictions and label correlation coefficients are summarized in a table, and the model bagging with the best performing set of rolling data is selected to be recorded by taking the average of the predictions.  
The recorded forecast values are generated and back-tested according to certain Bollinger band rules to obtain back-test indicators and return curves.  

