## UPENN_DSBC_Credit_Risk_Classification

##### This was another straightforward challenge. The lessons from class provided the necessary information required to successfully complete this challenge. I reviewed all of the class materials while working through this challenge. Geeks for Geeks, W3Schools, and Stack Overflow are all good sources when needed, as well as Pandas Docs. I reference these additional sources for assistance whenever necessary.

### Credit Risk Analysis Report

#### Overview of the Analysis

##### 1. Explain the purpose of the analysis
#####  * To evaluate the creditworthiness of potential borrowers.

##### 2. Explain what financial information the data was on, and what you needed to predict.
#####  * A loan risk model based on historical lending activity from a peer-to-peer lending services company used to predict low-risk and high-risk borrowers.

##### 3. Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
#####  * The independent variable (X) consisted of loan size, interest rate, borrower income, debt to income, number of accounts, and derogatory marks. The dependent variable (y) was the loan status.

##### 4. Describe the stages of the machine learning process you went through as part of this analysis.
#####  * The data was split into two sets; training and testing.

##### 5. Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
#####  * Two different methods of Logistic Regression were used in this analysis; one using the Original Data and the other using Resampled Data.

#### Results

##### Machine Learning Model 1:
##### Description of Model 1 Accuracy, Precision, and Recall scores.

##### Balanced Accuracy Score: 0.9520479254722232

#### Classification Report

              precision    recall  f1-score   support

            0       1.00      0.99      1.00     18765
            1       0.85      0.91      0.88       619

     accuracy                           0.99     19384
    macro avg       0.92      0.95      0.94     19384
    weighted avg    0.99      0.99      0.99     19384

##### Machine Learning Model 2:
##### Description of Model 2 Accuracy, Precision, and Recall scores.

##### Resampled Balanced Accuracy Score: 0.9936781215845847

#### Resampled Classification Report

              precision    recall  f1-score   support

            0       1.00      0.99      1.00     18765
            1       0.84      0.99      0.91       619

     accuracy                           0.99     19384
    macro avg       0.92      0.99      0.95     19384
    weighted avg    0.99      0.99      0.99     19384

#### Summary

##### Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
##### 1. Which one seems to perform best? How do you know it performs best?
##### The Resampled Model performed slightly better overall but the results from both models are close enough that you could use either one with confidence.

##### 2. Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
##### Predicting both 1's and 0's is important to insure that loans are approved for low-risk borrowers and not approved for high-risk borrowers. However, there can be false negatives and false positives which could impact a low-risk borrower from receiving a loan or a high-risk borrower being approved for a loan.

##### 3. If you do not recommend any of the models, please justify your reasoning.
##### Both models work well and could be used to determine low-risk and high-risk candidates with a very low chance of error.
