# Credit Risk Analysis
[Resampling Machine Learning Models](https://github.com/c-geisel/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)

[Ensemble Machine Learning Models](https://github.com/c-geisel/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)

## Overview of the analysis
Analyzing credit risk frequently poses a challenge being that it is an unbalanced classification problem. It poses a challenge as the number of good loans outweigh the number of risky loans. Different techniques are used to train and evaluate models with unbalanced classes. To begin, machine learning models oversample data randomly and through SMOTE, data is undersampled, a combination approach of over and undersampling is used, finally, ensemble models are used. This is done through the use of imbalanced-learn and scikit-learn libraries. The models are then evaluated based on the performance and reccommendations are given to decide whether or not they should be used to predict credit risk. 

## Results 
1. The first machine learning model used is a random oversampler in order to balance our dataset. 
    - Accuracy score of 64.7%
    - Precision low-risk: 0.01
    - Precision high-risk: 1.00
    - Recal low-risk: 
    - Recall High Risk: 
    - The precision is very low for high-risk loans at 0.01, and very high for low-risk at 1.00
    - The recall scores for high and low risk loans are relatively high at over 0.6 for both. 
![Random_Oversampling.png](Practice/Images/Random_Oversampling.png)

2. Next, another oversampling model is created using SMOTE. 
    - This model had an accuracy score of 64.6% 
    - The precision is once again very low for high-risk loans at 0.01, and very high for low-risk at 1.00
    - As in the earlier oversampling model, the recall numbers for both low and high-risk loans are good at over 0.6.
![Smote_Oversampling.png](Practice/Images/Smote_Oversampling.png)

3. An undesampling model is used.
    - This model had an accuracy score of 52.9% 
    - The precision score for low risk is very high at 1.00, and the precision for high-risk is very low at 0.01.
    - The recall for low risk is 0.45 and the recall rate for high risk is better at 0.61
![Undersampling.png](Practice/Images/Undersampling.png)

![Combinations_Over_Under_Sampling.png](Practice/Images/Combinations_Over_Under_Sampling.png)

![Random_Forest.png](Practice/Images/Random_Forest.png)

![Easy_Ensemble.png](Practice/Images/Easy_Ensemble.png)

## Summary 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
