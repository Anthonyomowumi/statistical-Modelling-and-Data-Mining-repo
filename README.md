# A Study Adopting Statistical and Data Mining Approach to Draw Inferences on Diabetes Mellitus in Women Project

# Project Summary
This study aimed at utilising statistical techniques to model the best predictors for Diabetes in women
and classifying the outcome class based on those predictors - using a machine learning algorithm. 




# Methods and Materials
The dataset was obtained from the National Institute of Diabetes and Digestive and Kidney Diseases. The purpose of the data collection was to use the diagnostic metrics included in the dataset to estimate a patient's likelihood of having diabetes or not. The dataset was chosen from a bigger database, and it was restricted to all female patients in PIMA India who were at least 21 years old. 



## I. Dataset Description
![image](https://github.com/Anthonyomowumi/statistical-Modelling-and-Data-Mining-repo/assets/93340041/b8537df8-0ec3-41d4-988d-8e52453fc632)


## II. Data Preprocessing and Transformation
 ### a) Data cleaning: Errors, special characters like "Inf" and "NaN," as well as non-negative values, were checked for by developing a check rule. The presence of outliers was visualized using boxplot
  ![image](https://github.com/Anthonyomowumi/statistical-Modelling-and-Data-Mining-repo/assets/93340041/e8abbef8-7004-4274-9abc-d68a8ffd7e03)

  ### b) Missing Data Imputation using missForest imputation
  652 missing was imputed using missForest imputation
  
  ### c) Descriptive and Graphical Analysis after Missing Value Imputation; 
         By using histogram to check the data distrbution, kurtosis and skewness of the dataset.
  
         Skewness checks the symmetric/assymmetric of the data variable, from the analysis in order of asymmetric, Blood Pressure ~0.14 < Glucose ~0.53 < BMI ~0.61 < Skin             Thickness ~0.70 < Pregnancies ~0.89 < Age ~1.13 < DiabetesPedigreeFunction ~1.92 < Insulin ~2.12, this shows that Insulin is more highly asymmetric than all other            variables and Blood Pressure is closely symmetric. 

         Kurtosis measures the tailedness of a data distribution. from the evaluation using the kurtosis equation and the result is Insulin is closely related to Leptokurtic          having a higher amount of excess kurtosis, same as DiabetesPedigreeFunction and Skin Thickness. Glucose is Platykurtic while other variables fall slightly within             Mesokurtic.
         
         ![image](https://github.com/Anthonyomowumi/statistical-Modelling-and-Data-Mining-repo/assets/93340041/b75fcff2-fe00-497f-a923-e5790ee7fcf7)


  
 ### d) Correlation and Variance Factor was used to check for multicollinearity in the data features

The dataset was analysed in this study using the R programming language.

