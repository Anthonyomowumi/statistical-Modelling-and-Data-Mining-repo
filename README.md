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
   By using histogram to check the data distrbution, as well as kurtosis and skewness of the dataset.
  
   Skewness checks the symmetric/assymmetric of the data variable, from the analysis in order of asymmetric, Blood Pressure ~0.14 < Glucose ~0.53 < BMI ~0.61 < Skin             Thickness ~0.70 < Pregnancies ~0.89 < Age ~1.13 < DiabetesPedigreeFunction ~1.92 < Insulin ~2.12, this shows that Insulin is more highly asymmetric than all other            variables and Blood Pressure is closely symmetric. 

   Kurtosis measures the tailedness of a data distribution. from the evaluation using the kurtosis equation and the result is Insulin is closely related to Leptokurtic          having a higher amount of excess kurtosis, same as DiabetesPedigreeFunction and Skin Thickness. Glucose is Platykurtic while other variables fall slightly within             Mesokurtic.
         
   ![image](https://github.com/Anthonyomowumi/statistical-Modelling-and-Data-Mining-repo/assets/93340041/b75fcff2-fe00-497f-a923-e5790ee7fcf7)


 ### d) Correlation and Variance Factor:
 A spearman correlation plot and Variance Inflation Factor was used to check for multicollinearity in the data features. 
 
 ![image](https://github.com/Anthonyomowumi/statistical-Modelling-and-Data-Mining-repo/assets/93340041/cdbedfe6-7ea5-4f70-bc26-1fce8b00b184)
The Spearman correlation plot shows a moderately positive between Age and Pregnancies, a strong correlation between (Insulin and Glucose), and (BMI and Skin Thickness) 

This is further studied by using the Variance Inflation Factor (VIF) to confirm the presence of multicollinearity. VIF determines the strength of multicollinearity between independent variables in a regression model. A VIF equal to 1 means no correlation between predictors while VIF < 5 means low multicollinearity or moderately correlated and VIF > 5 or 10 means high multicollinearity between predictors. None of the 8 features had VIF values larger than 5, as shown by the computed VIF values, implying that none of the features have high multicollinearity with one or more of the variables in a regression model.

 ![image](https://github.com/Anthonyomowumi/statistical-Modelling-and-Data-Mining-repo/assets/93340041/b68d9775-6f80-4f6a-8ffb-18d91ef05cc1)



All the analysis was done using the R programming language and in R studio using R markdown

## III.	STATISTICAL ANALYSIS OF THE INDEPENDENT VARIABLES USING LOGISTICS REGRESSION (LR)
Two Logistics Regression Model was built to check statistically significant predictors and compared with each other using the ANOVA function. The results of the ANOVA chi-square test pr(>chi) equals 0.611, which shows the p-value for a chi-squared test comparing the two models Since the p-value is higher than 0.05 (the usual significance level), the null hypothesis cannot be rejected and it can be concluded that there is not enough evidence to suggest that the model 1 provides a significantly better fit to the data than model 2. So, therefore all the features in the dataset is valuable in the prediction of Diabetes in Female. 

## IV.	MODEL TRAINING AND TESTING USING RANDOM FOREST ALGORITHM
The dataset was split into a 70:30 ratio and a Two Random Forest model was built, first model was built with the 8 predictors and other with 4 statistically significant predictors while the first model with higher performance was chosen. Accuracy of 76%, Sensitivity of 80%, and Specificity of 66% were used as the metric to evaluate its performance, and the ROC curve was drawn having an AUC score of 82% which means the model is good at predicting the outcomes. 
![image](https://github.com/Anthonyomowumi/statistical-Modelling-and-Data-Mining-repo/assets/93340041/1986d4c6-7e2b-482a-80b6-4b1818436b5e)


## V.CONCLUSION
It  was inferred from the outcomes of the various statistical analyses performed on the dataset indicates that all independent variables (8 features) from the original dataset are crucial for the prediction of Diabetes in women. Although It is suggested that further analysis should be conducted to ascertain the 4 statistically significant importance probably by using statistical controls and other methods. Also, the analysis's use of statistical and data mining tools was successful in reaching the study's objective as the conclusion was reached based on this study that the 8 features are necessary for the prediction of Diabetes Mellitus in Women. 

