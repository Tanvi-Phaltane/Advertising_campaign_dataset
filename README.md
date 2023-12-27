# Advertising_campaign_dataset
Analysing the online advertising dataset to predict if a subject would buy the online course or not

The dataset includes 10k records of respondents who answered a 36-pointer questionnare.The outcome of these questions has been compiled in this Kaggle spreadsheet (https://www.kaggle.com/datasets/ashydv/leads-dataset/)

Data processing was done using Python. In the pre-processing step, the categorical features were converted to numerical features, power-scaling data transformation applied to normalize the dataset. 

Recursive feature elimination technique used to select the most important features in the dataset. 
13 features selected based on variance threshold of > 80%. Logistics regression model was built on training set with a split of 75%-25% of the entire dataset. The feature-matrix and trained model was stored as a pickled-binary object for test dataset. F1 score of 0.75 was obtained on the test dataset. 

A predict.json file with user-defined feature values can be provided as input and output is a binary value for conversion rate.

Prefect, on open source machine learning pipeline orchestration tool was used for automation. 




