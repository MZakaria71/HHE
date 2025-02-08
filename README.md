# A comparative study of heterogeneous and homogeneous ensemble approaches for landslide susceptibility assessment
Landslide Susceptibility Assessment - Ensemble Comparison

https://link.springer.com/article/10.1007/s11356-023-26247-3

DOI: https://doi.org/10.1007/s11356-023-26247-3

Overview

This study aims to compare the performance of different ensemble models for landslide susceptibility assessment. The ensembles include both heterogeneous and homogeneous ensemble types, each with its set of base learners. The study also evaluates the ensembles using various metrics and conducts sensitivity analysis to assess the importance of different factors.

Ensembles Evaluated
Heterogeneous Ensembles
Stacking (ST): Stacking ensemble technique.
Meta-Dynamic Ensemble Selection (METADES): A novel approach in landslide assessment.
Voting (VO): Voting classifier.
Weighted Voting (WE): Weighted voting classifier.
Homogeneous Ensembles
AdaBoost (ADA): Adaptive boosting ensemble.
Bagging (BG): Bagging ensemble.
Random Forest (RF): Random forest ensemble.
Random Subspace (RSS): Random subspace ensemble.

Key Steps

Data Preparation

Data is loaded into a Pandas DataFrame named Full_datafreme.
Features and the target variable are separated into Features and Target.
Random undersampling is performed to balance the class distribution.

Base Learners

A list of base learners, including Logistic Regression, Decision Tree, SVM, Gaussian Naive Bayes, K-Nearest Neighbors, Linear Discriminant Analysis, Quadratic Discriminant Analysis, and MLP Classifier, is defined.

Feature Analysis

Correlation matrix and Variance Inflation Factors (VIF) are calculated and plotted to analyze feature relationships and multicollinearity.
Model Evaluation
The base learners are evaluated using grid search to find the best hyperparameters.
Metrics such as RMSE, AUC, Recall, Accuracy, and Kappa are calculated and stored in a DataFrame.
ROC curves are plotted for each base learner.

Heterogeneous Ensembles

Heterogeneous ensembles are created and evaluated:
Stacking (ST)
METADES
Voting (VO)
Weighted Voting (WE)
Homogeneous Ensembles
Homogeneous ensembles are created and evaluated:
Random Forest (RF)
AdaBoost (ADA)
Bagging (BG)
Random Subspace (RSS)

Predictions and Wilcoxon Analysis

Predictions are made using the best models and stored in a DataFrame.
A Wilcoxon signed-rank test is performed to compare the predictions of different models.

Sensitivity Analysis

Sensitivity analysis is conducted for the best models to assess the importance of factors.
Sensitivity results are plotted as bar charts.

Taylor Diagram

A Taylor diagram is created to visually represent model performance.

Dependencies

NumPy
Seaborn
Scikit-learn
Imbalanced-learn
SciPy
Pandas
Matplotlib
Joblib
DESlib
Researchpy
Easy_mpl

Usage

Ensure you have the required dependencies installed.
Load your dataset into the Full_datafreme DataFrame and modify the data preparation steps accordingly.
Run the code to evaluate different ensemble models for landslide susceptibility assessment.

Credits

This code was developed by Matougui Zakaria.
