# Credit_Risk_Analysis

## Overview of the analysis:

FastLending is a peer to peer lending services company that wants to use machine learning to predict credit risk.
Management believes that this will provide a quicker and more reliable loan experience. Furthermore, they also believe that machine learning will lead to a more accurate identification of good candidates for loans which will lead to lower default rates.
The purpose of this project is to assist Fastlending's lead data scientist in implementing this plan by building and evaluating several machine learning models or algorithms to predict credit risk.
The techniques used to achieve this include resampling and boosting as part of the project.
Once designed, we need to evaluate the performance of these models and make a written recommendation on whether these models should be used to predict credit risk.

## Results:
The code for the machine learning algorithms can be found in the jupyter notebook files: [credit_risk_resampling](https://github.com/Cryptotwister/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)
and [credit_risk_ensemble](https://github.com/Cryptotwister/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb).

In the course of the project we developed the following machine learning models:

* Naive Random Oversampling;
* SMOTE Oversampling;
* Undersampling;
* SMOTEENN algorithm - Combination (Over and Under) Sampling;
* Ensemble Classifier - Balanced Random Forest;
* Ensemble Classifier - Easy Ensemble.

For each one of these models, we split the data into training and testing datasets, performed accuracy scores calculations, confusion matrixes and imbalanced classification reports.

### 1. Naive Random Oversampling

![Naive Random Oversampling](https://user-images.githubusercontent.com/42978221/160057077-826b7b46-2090-4aa7-9a37-3a7cdd34d29f.png)

### 2. SMOTE Oversampling

![SMOTE Oversampling](https://user-images.githubusercontent.com/42978221/160057111-b932af26-0625-4680-a789-74f962679dc7.png)

### 3. Undersampling

![Undersampling](https://user-images.githubusercontent.com/42978221/160057122-3a2f62dc-efb2-4176-9c9e-e1376f21d9a1.png)

### 4. SMOTEENN algorithm - Combination (Over and Under) Sampling

![SMOTEENN - combination](https://user-images.githubusercontent.com/42978221/160057141-8b7410c1-937c-40db-beb3-a5f35baf16fd.png)

### 5. Ensemble Classifier - Balanced Random Forest

![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/42978221/160057161-3c690bd1-04af-4e4c-a42d-b89dac3efb28.png)

### 6. Ensemble Classifier - Easy Ensemble

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/42978221/160057185-583c2aae-8bb6-46ae-a51c-13020dfe2e03.png)

## Summary:

![ML Models Summary](https://user-images.githubusercontent.com/42978221/160158094-e18e269a-7750-4685-bffc-913e22757a91.png)

The results of our analysis are summarized  in the table above.
Based on our findings, we can say that AdaBoost Classifier model has the highest accuracy rate of 93%, which means that the model can predict the correct values 93% of the times.
Overall, it is noticeable that regression models are fall behind the classifier counterparts with accuracy scores being 66% and lower.
Based on accuracy rate alone the AdaBoost Easy Ensemble Classifier model is preferable.

Additionally, the F1 score, which indicates the level of imbalance between sensitivity and precision, shows the much higher scores for the classifier models. The Easy Ensemble AdaBoost Classifier in particular having the largest F1 score of 0.97, thereby demonstrating the least disparity between sensitivity and precision.

To summarize, based on the results of our analysis, it is recommended that the Easy Ensemble AdaBoost Classifier machine learning model be adopted for the purpose of predicting a credit risk.

