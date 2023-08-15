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
Accuracy is the right results comming from the test training by our dataset divided in all the predictions. in this case obtaining 99%

Precision is how true are the right predictions, in the case of 0 = 100% all the times it says it was 0 they were actually 0, and with 1 = 85% of the times it says were acctually 0 and the rest were wrong 15%

Recall is: paying attention to the values how many were correctly classified 99% of the times it says it was 1 was actually 1, and 91% of it says it was 0 it was right.  


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

in difference of the model 1 now we have different values starting by

Accuracy: We have 99% all the true results split by all the prediccions.

Precision: 99% of the time it says it was 0 and 1 they really that. 

and Recall: also 99% for 0 and 1

as we can see here the accuracy continues been 99% but there is abig diference with the rest: Precision and Recall. now is more balanced. 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-


With the results obtained, we can observed the accuracy was the same, but the way it arrives to that point is different. 

what we have in teh model #1 is an unbalance data, thay at the moment we train and test it was able to predict better `0` having 75,036 samples, but having a leak of samples of `1` only 2,500 that makes the problems in this model.

As we know the number of samples is important to train better for the moment we test it. and having pour quantity number of samples makes the model unefitient. 

then we change to the model #2 where the Over Sampling solve the leak of samples. duplicating the information of `0`s and `1`s until we have the same number each. 112,541 then been able to train and test it more efficient without lossing information as we could do with different models. 

In this escenario to have a `0` means it is okay to gives you a credit and the problem appear when it was a true negative in the firt model were 102.

In the other side `1` means you're not the best option when to give a credit is what we are talking about, showing that 56 were false negative.

99% right in 0
91% right in 1

with the difference of the second model where the number of wrong test were find but compare with the vast number of samples only takes 1% of the total, obtaining 

99% right in 0
99% right in 1

in this challenge the number of errors were located in Ones (high risk loan) wich means backs were not offering credits to people with healty loan, that only not create more money for the back, they do not make more but they does not lose. at the other side if the ratio of error were locate in Zeros col be tranlte as losses of money for the bank. Bank prefer not to win money that the losse of money. 

so it helps to have more credits but not really a big problem to solve.