# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

### Overview Analysis
The primary objective of this analysis is to construct a predictive model for assessing the creditworthiness of borrowers. To carry out this analysis, we have utilized a dataset from a peer-to-peer lending service company, which comprises several key features, including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. These features are utilized to determine the loan status. The chosen algorithm for this integrated model is logistic regression, which aims to ascertain whether a loan provided to a borrower in the testing dataset carries a low or high-risk classification.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

### Results Analysis
Precision:
For class 0: Precision is 1.00, signifying that every prediction labeled as class 0 is indeed a true positive. The model exhibits impeccable precision for class 0.
For class 1: Precision is 0.85, indicating that 85% of predictions assigned to class 1 are true positives, while 15% are false positives.

Recall:
For class 0: Recall is 0.99, denoting that the model accurately identifies 99% of actual class 0 samples as true positives. Only 1% of class 0 samples are incorrectly classified as class 1 (false negatives).
For class 1: Recall is 0.91, revealing that the model correctly identifies 91% of actual class 1 samples as true positives. However, 9% of class 1 samples are erroneously predicted as class 0 (false negatives).

F1-Score:
For class 0: The F1-score is 1.00, representing the harmonic mean of precision and recall for class 0. Given high precision and recall (close to 1), the F1-score is also very high.
For class 1: The F1-score is 0.88, indicating a well-balanced trade-off between precision and recall for class 1.

Support:
For class 0: There are 18,765 samples in the dataset belonging to class 0.
For class 1: The dataset contains 619 samples classified as class 1.

Accuracy:
The overall model accuracy is 0.99, meaning it correctly classifies 99% of all samples in the dataset.

## Summary

Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

### Summary
According to the confusion matrix, the regression model demonstrates strong performance, particularly in the "healthy loan" class, where it achieves nearly perfect precision, recall, and F1-score. In the "high-risk loan" class, the model's performance is also commendable, albeit with a slightly lower F1-score compared to the "healthy loan" class. Nonetheless, it maintains a well-balanced trade-off between precision and recall in this class.
