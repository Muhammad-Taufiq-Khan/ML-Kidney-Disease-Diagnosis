# Kidney Disease Diagnosis using Machine Learning

- Environment: <a href='https://kidney-disease-diagnosis.onrender.com'> Live WebApp in render<a> </li>
- Tools: Python, Flask, Scikit-learn, Matplotlib, Pansdas, Numpy </li>
- Supporting Algorithm: Random Forest</li>
---
 
 **1. Project Objective**

Around 1.7 million people die each year because of Kidney disease. Detecting kidney disease in the initial stage is essential for saving millions of lives. In this project, we applied KNN Imputation to impute missing values, Local Outlier Factor to remove outliers, SMOTE to handle data imbalance, K-stratified K-fold Cross-validation to validate the ML models, and a novel hybrid feature selection method to remove redundant features. Applied algorithms in this study are Support Vector Machine, Gaussian Naive Bayes, Decision Tree, Random Forest, Logistic Regression, K-Nearest Neighbor, Gradient Boosting, Adaptive Boosting, and Extreme Gradient Boosting. Finally, the Random Forest can detect kidney disease in the initial stage with 100% accuracy without any data leakage. Then we have developed a Web Application using Flask (a micro web-Framework), which detect kidney disease using the trained Random Forest model from the backend.
  
**2. Expalaination of the directory tree**
```
- Notebooks       : Google colab notebooks and dataset to train the Machine Learning model.
- joblib_dump     : Saved/dumped best models and fitted preprocessing objects.
- static          : CSS, JavaScript, and image files.
- templates       : HTML pages to render.
- .gitignore      : Script to automaticallty ignore redundant files and directories during version control.
- app_pred.py     : Python script to preprocess the upcoming data using preprocessing objects (dumped) and classify using dumped model.
- app.py          : Flask script to handle get and post requests.
- reqirements.txt : Required dependencies list with preferred version.
```


