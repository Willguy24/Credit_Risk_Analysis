## Credit_Risk_Analysis
## Overview of the Analysis
The objective of this evaluation is to employ supervised learning models to classify credit risk for credit card customers, and assess their effectiveness. To achieve this, we will use data from LendingClub and conduct several analyses to determine if the models created can be used to predict credit risk. We will start by splitting the data into testing and training sets and then using six models to perform the analysis. For each model, we will calculate the balanced accuracy score, precision, and recall score, which will later be used to recommend a particular model.

## Results
## Resampling Techniques
We will begin by looking at the first set of techniques, which involves oversampling and undersampling, and their outcomes.

## Naive Random Oversampling
--Naive Random Oversampling

-Balanced accuracy score: 0.65
-Precision score: 0.99
-Recall score: 0.59

## SMOTE Oversampling
--SMOTE Oversampling

-Balanced accuracy score: 0.65
-Precision score: 0.99
-Recall score: 0.59

## Undersampling
--Undersampling

-Balanced accuracy score: 0.52
-Precision score: 0.99
-Recall score: 0.40

## Combination (Over and Under) Sampling
--Combination (Over and Under) Sampling

-Balanced accuracy score: 0.65
-Precision score: 0.99
-Recall score: 0.59

## Ensemble Techniques
Next, we will move on to the second set of analyses, which involves ensemble techniques and their outcomes:

## Balanced Random Forest Classifier
--Balanced Random Forest Classifier

-Balanced accuracy score: 0.78
-Precision score: 0.99
-Recall score: 0.87

The Balanced Random Forest Classifier also provides scores for the most important features used in the model. The top features, according to the random forest classifier, are:

-total_rec_prncp: (0.07876809003486353)
-total_pymnt: (0.05883806887524815)
-total_pymnt_inv: (0.05625613759225244)
-total_rec_int: (0.05355513093134745)
-last_pymnt_amnt: (0.0500331813446525)

-- Pic

## Easy Ensemble AdaBoost Classifier
--Easy Ensemble AdaBoost Classifier

-Balanced accuracy score: 0.93
-Precision score: 0.99
-Recall score: 0.94

## Summary
The balanced accuracy score, which indicates the accuracy of the test results based on the training module, varied significantly across each model, ranging from 54% to 93%. None of the results were excessively high, which suggests that the data was not oversampled.

The precision scores, which measure the number of true positive results by all positive results (true and false) for each test, were all 99%, indicating that each test accurately determined which results were true and had few false positive results.

Lastly, the recall (or sensitivity) scores for the models ranged significantly, from a low of 40% to a high of 94%. The recall score measures how likely it is that the test will identify a person as a credit risk if they are one. A higher result means that credit risks are more likely to be correctly identified as such and not misclassified as non-credit risks.

## Recommendation
Based on the results, our recommendation is to use the Easy Ensemble AdaBoost method. Its precision rate of 99% means that predicted positive rates are 99