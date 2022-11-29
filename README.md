# Credit_Risk_Analysis
Supervised Machine Learning and Credit Risk

## Loan prediction risk analysis, Overview & Resources:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. We can use different techniques to train and evaluate models with unbalanced classes. Multible libraries and algorithms were used to build and evaluate models using resampling:

  * **`imbalanced-learn`**
  * **`scikit-learn`**
  * **`RandomOverSampler`**
  * **`SMOTE algorithms`**
  * **`ClusterCentroids algorithm`**
  * **`SMOTEENN algorithm`**
  * **`BalancedRandomForestClassifier (bias reduction model)`**
  * **`EasyEnsembleClassifier (bias reduction model)`**

## Purpose
  1. Define how a machine learning algorithms are used in data analytics.
  2. Create training and test groups from data sets.
  3. Implement the logistic **regression**, **decision tree**, **random forest**, and **support vector machine      algorithms**.
  4. Interpret the results of the **logistic regression**, **decision tree**, **random forest**, and **support vector machine algorithms**.
  5. Compare, advantages and disadvantages of supervised learning algorithm.
  6. Show and determine which supervised learning algorithm is best used for a given data set or scenario.
  7. Use **ensemble** and **resampling** techniques to improve performance of the sample model.

## Results:
For the six machine learning models tested, including, respective balanced accuracy, precision, and recall scores are shown here:

## Naive Random Oversampling

![Naive_Random_Oversampling](https://user-images.githubusercontent.com/109354592/204424096-939e936b-c7c0-4e20-8695-596548753f49.png)

1. Balanced Accuracy: `0.648767580808264`
2. Precision: The precision is low for High-risk loans `0.01` and is high for Low-risk loans `1.00`.
3. Recall: High/Low risk = `.61/.69`

## SMOTE Oversampling

![SMOTE Oversampling](https://user-images.githubusercontent.com/109354592/204425178-d739d560-7b6b-4bdf-b4d8-1fef902d388e.png)

Balanced Accuracy: `0.6159507435206336`
Precision: The precision is low for High-risk loans `0.01` and is high for Low-risk loans `1.00`.
Recall: High/Low risk = `.59/.65`

## Undersampling

![Undersampling](https://user-images.githubusercontent.com/109354592/204425538-a26f14c4-da99-4fbd-9476-584b572af843.png)

1. Balanced Accuracy: `0.6159507435206336`
2. Precision: The precision is low for High-risk loans `0.01` and is high for Low-risk loans `1.00`.
3. Recall: High/Low risk = `.59/.46`

## Combination Under-Over Sampling

![Combination (Over and Under) Sampling](https://user-images.githubusercontent.com/109354592/204425737-c466b9a7-d433-4f05-a962-33ea900d6758.png)

1. Balanced Accuracy: `0.6419346846030192`
2. Precision: The precision is low for High-risk loans `0.01` and is high for Low-risk loans `1.00`.
3. Recall: High/Low risk = `.70/.58`

## Balanced Random Forest Classifier

![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/109354592/204426092-1a037c08-498f-4f1e-acc5-cfaec974844c.png)

1. Balanced Accuracy: `0.7877672625306695`
2. Precision: The precision is low for High-risk loans `0.04` and is high for Low-risk loans `1.00`.
3. Recall: High/Low risk = `.67/.91`

## Easy Ensemble AdaBoost Classifier

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/109354592/204426324-e2f267de-af00-45cd-9bd9-eb16e708eb19.png)

1. Balanced Accuracy: 0.925427358175101
2. Precision: The precision is low for High-risk loans and is high `0.07` for Low-risk loans `1.00`.
3. Recall: High/Low risk = `.91/.94`

## Summary:

Working with balanced accuracy, the highest compared accuracy is between 0 and 1 which is closest to 1, representing the best machine learning model for our analysis. Credit card data, the Easy Ensemble AdaBoost Classifier shows to be the best model to show this data, with a .93 balanced accuracy. Other models tested showed below .80 balanced accuracy. 
Precision data across each model presented similar data, and showed to be within an appropriate data range. The recall score shows to also fall within 0 and 1, with the data showing to be closer to 1, determining to be the better model. 
Finally, Easy Ensemble AdaBoost Classifier showed to have the highest recall score, making it the best machine learning model, which can be used for further credit card analysis.

