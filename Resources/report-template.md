# Module Report 

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * The logistic regression model performs very well in predicting both the 0 (healthy loan) and 1 (high-risk loan) labels. Here are the evaluation metrics for each label:

For label 0 (healthy loan):

Precision (pre): 1.00
Recall (rec): 0.99
Specificity (spe): 0.91
F1-score (f1): 1.00
For label 1 (high-risk loan):

Precision (pre): 0.85
Recall (rec): 0.91
Specificity (spe): 0.99
F1-score (f1): 0.88
These metrics indicate that the model has high accuracy, precision, recall, and F1-score for both labels. It correctly predicts the majority of healthy loans (label 0) with high precision, recall, and F1-score. It also performs well in identifying high-risk loans (label 1) with acceptable precision, recall, and F1-score.



* Machine Learning Model 2:
  * The logistic regression model, fit with oversampled data, performs very well in predicting both the 0 (healthy loan) and 1 (high-risk loan) labels.

For the healthy loans (label 0), the model achieves perfect precision (1.00) and high recall (0.99), indicating that it accurately identifies the majority of healthy loans. The specificity (0.99) is also high, suggesting that the model correctly identifies the majority of non-high-risk loans.

For the high-risk loans (label 1), the model achieves good precision (0.84) and excellent recall (0.99), indicating that it identifies a high proportion of actual high-risk loans while maintaining a relatively low false positive rate. The specificity (0.99) is also high, suggesting that the model correctly identifies the majority of non-high-risk loans.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
---
Comparing the evaluation metrics, the model with oversampled data shows improvements in various aspects. The precision for label 1 (high-risk loans) has increased from 0.85 to 0.84, indicating a slightly lower false positive rate. The recall for label 1 has significantly improved from 0.91 to 0.99, indicating a higher proportion of actual high-risk loans correctly identified. The specificity for label 0 (healthy loans) has also increased from 0.91 to 0.99, indicating a better identification of non-high-risk loans.
If you do not recommend any of the models, please justify your reasoning.
