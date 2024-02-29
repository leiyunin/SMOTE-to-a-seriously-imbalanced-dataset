# SMOTE-to-a-seriously-imbalanced-dataset

# Overview
This homework set explores the application of SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance in a dataset featuring a large number of features and data points, specifically targeting the APS Failure at Scania Trucks dataset:

- **Dataset and Preparation**:
  - Utilizes the APS Failure dataset, comprising a training set with 60,000 rows and 171 numeric attributes.
  - Implements techniques to handle missing values without discarding significant data.
  - Calculates the coefficient of variation (CV) for each feature and visualizes the highest CV features through scatter and box plots, aiding in the assessment of feature significance.

- **Tree-Based Methods**:
  - **Random Forest Classification**: Initially trains a random forest without addressing class imbalance, evaluating performance with metrics like confusion matrix, ROC, AUC, and misclassification rates, alongside calculating Out of Bag (OOB) error.
  - **Class Imbalance Compensation**: Investigates methods to adjust for class imbalance within random forest models and applies these adjustments to compare results.

- **Advanced Modeling Techniques**:
  - **XGBoost and Model Trees**: Explores the concept of model trees, employing L1-penalized logistic regression at each node and utilizing XGBoost for model training. Error estimation is performed through cross-validation techniques, with model effectiveness evaluated via confusion matrix, ROC, and AUC metrics.
  - **SMOTE Application**: Implements SMOTE to pre-process the dataset, aiming to correct class imbalances before re-training the XGBoost model. This step emphasizes the importance of proper cross-validation methods in the context of SMOTE, facilitating a comparison between compensated and uncompensated cases.

This comprehensive approach to dealing with imbalanced datasets in a high-dimensional feature space showcases the effectiveness of SMOTE alongside advanced tree-based methods, highlighting the critical role of appropriate data preparation and model evaluation strategies in predictive modeling.