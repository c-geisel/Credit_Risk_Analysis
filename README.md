# Credit Risk Analysis
[Resampling Machine Learning Models](https://github.com/c-geisel/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)

[Ensemble Machine Learning Models](https://github.com/c-geisel/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)

## Overview of the analysis
Analyzing credit risk frequently poses a challenge being that it is an unbalanced classification problem. It poses a challenge as the number of good loans outweigh the number of risky loans. Different techniques are used to train and evaluate models with unbalanced classes. To begin, machine learning models oversample data randomly and through SMOTE, data is undersampled, a combination approach of over and undersampling is used, finally, ensemble models are used. This is done through the use of imbalanced-learn and scikit-learn libraries. The models are then evaluated based on the performance and reccommendations are given to decide whether or not they should be used to predict credit risk. 

## Results 
1. The first machine learning model used is a random oversampler in order to balance our dataset. 
    - Accuracy score of 64.7%
    - Precision high-risk: 0.01
    - Precision low-risk: 1.00
    - Recall high-risk: 0.63
    - Recall low-risk: 0.66

![Random_Oversampling.png](Practice/Images/Random_Oversampling.png)

2. Next, another oversampling model is created using SMOTE. 
    - Accuracy score of 64.6%
    - Precision high-risk: 0.01
    - Precision low-risk: 1.00
    - Recall high-risk: 0.64
    - Recall low-risk: 0.65

![Smote_Oversampling.png](Practice/Images/Smote_Oversampling.png)

3. An undesampling model is used.
    - Accuracy score of 52.9% 
    - Precision high-risk: 0.01
    - Precision low-risk: 1.00
    - Recall high-risk: 0.61
    - Recall low-risk: 0.45

![Undersampling.png](Practice/Images/Undersampling.png)

4. A combination SMOTEENN model is used that combines both over and undersampling techniques.
    - Accuracy score of 64.3% 
    - Precision high-risk: 0.01
    - Precision low-risk: 1.00
    - Recall high-risk: 0.72
    - Recall low-risk: 0.56

![Combinations_Over_Under_Sampling.png](Practice/Images/Combinations_Over_Under_Sampling.png)

5. Ensemble techniques are also used to model the dataset. Here, a Random Forest model is used. 
    - Accuracy score of 89.4% 
    - Precision high-risk: 0.03
    - Precision low-risk: 1.00
    - Recall high-risk: 0.62
    - Recall low-risk: 0.90

![Random_Forest.png](Practice/Images/Random_Forest.png)

6. Finally, an Easy Ensemble Model is used.
    - Accuracy score of 94.2% 
    - Precision high-risk: 0.07
    - Precision low-risk: 1.00
    - Recall high-risk: 0.91
    - Recall low-risk: 0.94

![Easy_Ensemble.png](Practice/Images/Easy_Ensemble.png)

## Summary 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
