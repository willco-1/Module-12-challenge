# Module 12 Report Template

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
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  *The first model that was trained used logistic regression. 
  * This model was able to obtain a balanced accuracy score of 95.2%
  * It had a precison of 86% and a recall score of 91%
  


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * The second model was a random oversampled Logistic regression model 
  * It achieved a balanced accuracy score of 99.4% 
  *It had a precision score of 85% and a recall  score of  99%
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
* Out of the two models, the over sampler performs the best. Applying the random Oversampler to the logistic regression model was able to significantly improve the recal and the f1 score with a miniscule decrease in precision. Furthermore, the resampled model was able to achieve a higher level of accuracy in the case of mislabeling bad loans. The intial model labeled 46 loans as low risk, and the resampled model, only 3. That is a very solid improvement. This being said, I cannot recomend either moodel. The most accurate model would be a Linear Support vectior machine model with balanbced class weights and a MinMax  scaler applied to it. See LendingGenie (Project2) for the code for that. The model was trained on a much , much larger dataset and with a larger feature set. This model acheived a slighlty lower recall score than the Randmom oversampler, but a much higher precision and accuracy. 
If you do not recommend any of the models, please justify your reasoning.
