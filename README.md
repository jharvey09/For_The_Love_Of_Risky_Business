# Risky Business [Peer To Peer Lending]
![image](https://user-images.githubusercontent.com/80294571/130276179-78282574-0c9b-4b60-8504-560cf956e9f7.png)

## Table Of Contents:
[Background](https://github.com/jharvey09/Risky_Business_Peer_To_Peer_Lending#background)

[Files](https://github.com/jharvey09/Risky_Business_Peer_To_Peer_Lending#files)

[Steps](https://github.com/jharvey09/Risky_Business_Peer_To_Peer_Lending#steps)

[Conclusion](https://github.com/jharvey09/Risky_Business_Peer_To_Peer_Lending#conclusion)


## Background:
Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. 
For this project, I will build and evaluate several machine learning models; to predict credit risk using data typically seen from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem *(the number of good loans is much larger than the number of at-risk loans)*. I will need to employ different techniques for training and evaluating models with imbalanced classes. 

## Files:
1) Resampling Notebook
2) Ensemble Notebook
3) Lending Club Loans Data

## Steps:
1) Read the data into a DataFrame

![image](https://user-images.githubusercontent.com/80294571/130275511-713b2225-a72e-4107-95e8-f1606262f155.png)

2) Split the data into training and testing sets

![image](https://user-images.githubusercontent.com/80294571/130275450-32ff2f71-c6d0-4e27-b938-59a32362f2af.png)

3) Scale the training and testing data using the StandardScaler
4) Generate a classification report using the imbalanced_classification_report

![image](https://user-images.githubusercontent.com/80294571/130275961-4fb880bd-17cf-4a19-b76b-55607b47def9.png)

8) For the balanced random forest classifier only, print the feature importance sorted in descending order



## Conclusion:
### Credit Risk Resampling:
For this analysis, I needed to use many different algorithms to form a cohesive conclusion on the best model for credit risk resampling. The model would fit best in the current peer-to-peer lending market, and to figure this out. I needed to ask myself three questions. First, I would ask ***Which model had the best-balanced accuracy score?***  I would then ask myself as I peered through the data. ***Which model had the best recall score?***  The final determining factor would be in my last question, ***Which model had the best geometric mean score?***
After the initial imports, I trained and tested the data with a StandardScaler. Next, I loaded that data into a simple logistic regression model. Therefore, using that data to calculate the balanced accuracy score. Display the data in a confusion matrix before printing the data in an imbalanced classification report. Next, I would need to train the data with the two algorithms separately, such as the *"Naive Random Oversampling algorithm"* first. Following, I loaded individual oversampled algorithms into a Logistic Regression model. Next, I calculated the balanced accuracy score; before running the data through a confusion matrix. My last step was to print through the imbalanced classification report, repeat the same steps for the SMOTE Oversampling algorithm. 
Now to undersample, I would need to resample the data using the ClusterCentriods algorithm. Train and fit the Logistic Regression model, calculate the balanced accuracy score. Finally, display the data in a confusion matrix and print the imbalanced classification report. 
To conclude my findings, I would need to use the over-under-sampling algorithm to determine if the algorithm results in the best performance compared to the other sampling algorithms above. 
The best credit risk resampling that provided the best-balanced accuracy score was the ***Logistic Regression using SMOTEENN***. The model that had the best recall was the ***Naive Random Sampling***. Last, the model with the best geometrical mean score was the ***Logistic Regression using SMOTEENN***.

### Credit Risk Sampling:
For this analysis, I needed to use a few different algorithms to conclude my findings. I asked myself the same three questions and one additional one. This time I was curious, what were the top three features I used to help me conclude my finding? After initial imports and basic data cleaning, I split and trained data before using a *StandardScaler*. Next, the algorithm used was the *"Balanced Random Forest Classifier"*. I would next calculate the balanced accuracy score before running the data through a confusion matrix. Next, print the data on an imbalanced classification report; I listed the features in descending order. I completed the same steps above for the next algorithm entitled the *"Easy Ensemble Classifier"*. 
The best credit risk sampling that provided the best-balanced accuracy score was the ***Easy Ensemble Classifier***. The model that had the best recall was the ***Easy Ensemble Classifier***. Last, the model with the best geometrical mean score was the ***Easy Ensemble Classifier***. And, the final question was, ***What were the top three features?*** After further review, I feel that the top three features are:

**Regression |
Classification | 
Predict**




