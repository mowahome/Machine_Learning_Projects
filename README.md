# Machine_Learning_Projects
# Risky Business
## Background
Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, a client has asked that you help them predict credit risk with machine learning techniques.
For this assignment, I built and evaluated several machine learning models to predict credit risk using data typically used from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), therefore I used imbalanced-learn and Scikit-learn libraries to build and evaluate models using:
1. Resampling
2. Ensemble Learning

## Resampling
I resampled the LendingClub data (in Data folder) and built and evaluated logistic regression classifiers using the resampled data. To do this, I read in the csv file into a dataframe, split the data into training and testing data, scaled the training and testing data using the StandardScaler and ran a simple logistic regression model, and obtained the balanced accuracy score and imbalanced classification report.

Next I oversampled the data using the 'Naive Random Oversampler' and 'SMOTE' algorithms, and obtained the balanced accuracy score and imbalanced classification report.

I undersampled using the 'Cluster Centroids' algorithms and obtained the balanced accuracy score and imbalanced classification report.

And finally, I used the over and undersample using a 'SMOTEENN' algorithm and obtained the balanced accuracy score and imbalanced classification report.

From these results, I was able to identify which model had the best balanced accuracy score, recall score, and geometric score.

### Ensemble learning
For this section, I used two different ensemble classifiers to predict loan risk and evaluate each model. I also obtained the balanced accuracy and classification reports for both models. From these results, I was able to identify which model had the best balanced accuracy score, recall score, and geometric score.