# statistical-Modelling-and-Data-Mining-repo
Data Science Master Course @Ulster University, Northern Ireland, United Kingdom

# A Study Adopting Statistical and Data Mining Approach to Draw Inferences on Diabetes Mellitus in Women Project

# Abstract
The study aimed at utilising statistical techniques to model the best predictors for Diabetes in women and classifying the 
outcome class based on those predictors - using a machine learning algorithm. The dataset used for this was sourced at
Kaggle containing 768 records and 8 predictors/Independent variables and 1 Dependent variable with missing values recorded as NA, 
dealt with by using the missForest Algorithm in RStudio to impute the missing values. Appropriate statistical methods were done, 
and most attributes show rightly skewed and more asymmetrical than normal distribution around the mean. 

Two Logistics Regression Model was built to check statistically significant predictors and compared with each other using the ANOVA function. 
The results of the ANOVA chi-square test pr(>chi) equals 0.611, which shows the p-value for a chi-squared test comparing the two models 
Since the p-value is higher than 0.05 (the usual significance level), the null hypothesis cannot be rejected and it can be concluded that there is not enough evidence 
to suggest that the model 1 provides a significantly better fit to the data than model 2. 

Furthermore, the dataset was split into a 70:30 ratio and a Two Random Forest model, first model was built with the 8 predictors and 
other with 4 statistically significant predictors while the first model with higher performance was chosen. 
Accuracy of 76%, Sensitivity of 80%, and Specificity of 66% were used as the metric to evaluate its performance, 
and the ROC curve was drawn having an AUC score of 82% which means the model is good at predicting the outcomes. 
Overall, the study was successful in achieving its goals.
