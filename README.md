# Kidney Disease Diagnosis using Machine Learning

- Environment: <a href='https://kidney-disease-diagnosis.onrender.com'> Kidney Disease Diagnosis Live WebApp<a>
- Tools: Python, Flask, Scikit-learn, Matplotlib, Pansdas, Numpy 
- Supporting Algorithm: Random Forest
---

 ## **1. Project Objective**

Around 1.7 million people die each year because of Kidney disease. Detecting kidney disease in the initial stage is essential for saving millions of lives. In this project, we applied Ordinal Encoder and Label Encoder to encode categorical value and label, Min-Max Normalization to rescale the data, KNN Imputation to impute missing values, Local Outlier Factor to remove outliers, SMOTE to handle data imbalance, K-stratified K-fold Cross-validation to validate the ML models, a novel hybrid feature selection method to remove redundant features, and Grid Search CV  for hyperparameter tuning. Applied algorithms are Support Vector Machine, Gaussian Naive Bayes, Decision Tree, Random Forest, Logistic Regression, K-Nearest Neighbor, Gradient Boosting, Adaptive Boosting, and Extreme Gradient Boosting. Finally, the Random Forest can detect kidney disease in the initial stage with 100% accuracy without any data leakage. Then we have developed a Web Application using Flask (a micro web-Framework), which detect kidney disease using the trained Random Forest model from the backend. 
  
## **2. Expalaination of the directory tree**
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

 ## **3. WebApp Interface**
 
 - *Home page*
 
 ![image](https://user-images.githubusercontent.com/70132613/210597792-2517c945-383c-4c3e-b3dc-b1487e70f53d.png)
 
 
 - *Form to checkup kidney health*
 
 ![image](https://user-images.githubusercontent.com/70132613/210598400-817c7081-6974-4cde-8b58-c712ecc60989.png)


- *Generated report*

![image](https://user-images.githubusercontent.com/70132613/210598773-ef32e6ba-5940-4fca-bf44-764d824bb417.png)


## **4. Dataset Description**

We have collected the data set from the
University of California Irvine Machine Learning Repository. The data set has 400 samples and 24 features,
with a lot of missing values, outliers, typing mistakes, class
imbalances, etc. In 400 samples, 250 belong to ckd and
150 belong to notckd. The features Packed Cell Volume
(pcv), Red Blood Cell Count (rc), and White Blood
Cell Count (wc) were mistakenly considered as nominal
because of typing errors. We have converted those features
into numerical data types. Similarly, few other features
also have some typos, which have been fixed by the python
map method.
 
![image](https://user-images.githubusercontent.com/70132613/210613049-871177f6-5786-46a9-9a43-9af5259236f6.png)

![image](https://user-images.githubusercontent.com/70132613/210613327-80f6b273-6ff7-4f71-a5e3-0e9fae68d4b8.png)

 
## **5. Method to build the model**
 
 ![image](https://user-images.githubusercontent.com/70132613/210612951-e20cb002-e2ec-4a2d-8307-331daa262405.png)


## **6. Algorithm Performance**

- ***Performance of the Random Forest model***

|  | precision | recall |   f1-score | support |
| ----------- | ----------- | ----------- | ----------- | ----------- | 
| 0 |  0.99 | 1.00 | 0.99 | 66 | 
| 1 |  1.00 | 0.97 | 0.99 | 34 | 
| accuracy |  |  | 0.99  | 100 | 
| macro avg | 0.99 | 0.99 | 0.99 |  100 | 
| weighted avg | 0.99 | 0.99 | 0.99 | 100 | 


![image](https://user-images.githubusercontent.com/70132613/210609181-d25271f5-f0c7-4f7a-8dbf-8eb2a929469b.png)

- ***Performance comparison with other trained models***
 
 ![image](https://user-images.githubusercontent.com/70132613/210614005-b9876a94-55b7-48d3-8f09-226080a12dec.png)
