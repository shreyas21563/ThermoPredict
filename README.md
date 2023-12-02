# Machine-Learning-Project

## Motivation
The increasing global population demands growth in the agri-food industry. Understanding and addressing the environmental impact of the agri-food industry is crucial for mitigating climate change and developing sustainable practices within this sector.

The motivation for this project is the need to develop tools for predicting and managing the temperature change caused by CO2 emissions. By harnessing the power of ML, the project aims to create a predictive model that will enable stakeholders and anyone connected to the agri-food industry to make informed decisions and reduce carbon emissions.

## Dataset Details
The Agri-food CO2 emission dataset  available on Kaggle has been curated by combining and meticulously processing multiple distinct datasets sourced from the Food and Agriculture Organization (FAO) and data provided by the Inter governmental Panel on Climate Change (IPCC). As shown by the dataset, these emissions make a significant and noteworthy contribution to the annual global emissions. The dataset contains 6965 rows and 31 columns, including 30 distinct features and 1 target column. The target column, labelled “Average Temperature °C“, indicates the yearly average temperature rise.

## Preprocessing Techniques
1) Handling Null Values: Rows containing Null values were removed from the dataset to ensure data integrity and prevent potential bias in the analysis.
2) Eliminating Duplicate Rows: Duplicate rows were identified and removed from the dataset to avoid redundancy and ensure the accuracy of the analysis.
3) Outlier Removal:  Outliers were removed from the dataset because have the potential to significantly impact the dataset by introducing variations and deviations from its typical distribution.
4) Feature Removal: Features exhibiting a high correlation, represented by a correlation coefficient greater than or equal to 0.99, were identified and removed. This step helps in improving the model’s interpretability and generalization.
5) Encoding for Categorical Features: We used 2 techniques for encoding the categorical features:
    ●   Label Encoding: Used Label Encoding to transform the categorical feature "Area" into a numerical format for modelling and analysis.
    ●   One-Hot Encoding: The categorical feature "Area" was transformed using One-Hot encoding. This technique creates binary columns for each category, allowing machine learning algorithms to work effectively         with categorical data.
6) Standard Scaling: Standard scaling was used to standardize the data. Standardization helps ensure that features with different units and scales do not disproportionately influence the modeling process and helps machine learning algorithms converge faster.

## Machine Learning Models Used
1) Random Forest Regressor
2) Linear Regressor
3) Gradient Boosting Regressor
4) Adaboost Regressor
5) XGB Regressor
6) Lasso Regressor
7) Ridge Regressor
8) Support Vector Regression (SVR) with various kernels: 
      - RBF kernel
      - Linear kernel
      - Polynomial kernel
      - Sigmoid kernel
9) Artificial Neural Network (ANN):
  - Label-encoded data 
  - One-Hot encoded data
  The parameters that they used are the following: 
    - optimizer: Stochastic gradient descent
    - Number of Iterations: 500
    - Learning rate: 1e-4 (Low because there were high variations in the output with higher lr.
    - Activation Function: : ReLU




