# A Study Adopting Statistical and Data Mining Approach to Draw Inferences on Diabetes Mellitus in Women Project

# Project Summary
This study aimed at utilising statistical techniques to model the best predictors for Diabetes in women
and classifying the outcome class based on those predictors - using a machine learning algorithm. 




# Methods and Materials
The dataset was obtained from the National Institute of Diabetes and Digestive and Kidney Diseases. The purpose of the data collection was to use the diagnostic metrics included in the dataset to estimate a patient's likelihood of having diabetes or not. The dataset was chosen from a bigger database, and it was restricted to all female patients in PIMA India who were at least 21 years old. 



## I. Dataset Description
![image](https://github.com/Anthonyomowumi/statistical-Modelling-and-Data-Mining-repo/assets/93340041/b8537df8-0ec3-41d4-988d-8e52453fc632)


## II. Data Preprocessing and Transformation
  a) Data cleaning: Errors, special characters like "Inf" and "NaN," as well as non-negative values, were checked for by developing a check rule. The presence of outliers was visualized using boxplot
  ![image](https://github.com/Anthonyomowumi/statistical-Modelling-and-Data-Mining-repo/assets/93340041/e8abbef8-7004-4274-9abc-d68a8ffd7e03)

  b) Missing Data Imputation using missForest imputation: 652 missing was imputed using missForest imputation
  
  c) Descriptive and Graphical Analysis after Missing Value Imputation; this involve checking the data distribution using kurtosis and skewness of the dataset. 
  d) Correlation and Variance Factor was used to check for multicollinearity in the data features

The dataset was analysed in this study using the R programming language.

