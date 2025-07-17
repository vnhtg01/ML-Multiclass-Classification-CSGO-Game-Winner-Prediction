
<img width="1100" height="300" alt="image" src="https://github.com/user-attachments/assets/080d2a9e-2501-4f2e-b8b4-bc93c170e79b" />

<h1 align="center">ML Multiclass Classification Project for CSGO Game Winner Prediction</h1>

<h4><u>Objective :</u></h4> 
Build a machine learning model to perform <b>Multiclass classification</b> based on a real dataset from Kaggle. Project done in python on jupyter notebook.

<h4><u>Notes :</u></h4> 

Class `0` represents *Lost*, class `1` represents *Tie (Draw)*, class `2` represents *Win*.

# Table of Contents

- [A. Pipeline Overview](#apipeline-overview)
  - [A.1. Data Import](#a1-data-import--from-kaggle)
  - [A.2. Exploratory Data Analysis (EDA) & Data Visualization](#a2-exploratory-data-analysis-eda--data-visualization)
  - [A.3. Data Preprocessing](#a3-data-preprocessing)
  - [A.5. Model Training](#a5-model-training)
  - [A.6. Model Evaluation](#a6-model-evaluation)
  - [A.7. Model Deployment](#a7-model-deployment--not-included)
- [B. Report File extracted by ydata-profiling](#breport-file-extracted-by-ydata-profiling)
- [C. Prediction Model Summary](#c-the-file-summarizing-the-prediction-models-includes-the-accuracy-f1-score-and-time-taken-parameters-and-prediction-execution-time-based-on-this-dataset)
  - [C.1. Models sorted by speed and accuracy](#c1-this-list-of-trained-models-sorted-by-fast-execution-time-and-high-balanced-accuracy-parameter)
  - [C.2. Quickly check other models](#c2-quickly-check-other-models-through-accuracy-roc-auc-f1-score)
- [D. Results](#d-results)



# A.Pipeline-Overview

1. **Data Import** : from Kaggle
2. **Exploratory Data Analysis (EDA) & Data Visualization**  
   - Check for missing values
   - F-statistics, P-value, Chi square
   - Deleting/Keeping unnecessary series according to p-value and domain knowledge
   - Analyze variable distributions/density
   - Compute correlation matrix
   - Labelencoder for target column
   - Create a report of dataset from ydata_profiling
3. **Data Preprocessing**
   - Multi-Collinearity Test
   - SimpleImputer
   - Robusting (scaling) for numerical features and OneHotEncoder for categorical feature (before removing it)
   - Train/Test split
   - GridSearchCV to find the bests hyperparameters
5. **Model Training** 
   - Logistic Regression  
   - Decision Tree  
   - Random Forest
   - (Bonus) LazyPredict to show performances of 30-40 differents models
6. **Model Evaluation** 
   - Accuracy, Precision, Recall, F1-score  
   - Classification report  
   - Confusion matrix
   - ROC AUC
   - (Bonus) Quickly check other models
7. **Model Deployment** : not included

# B.Report-File-extracted-by-ydata-profiling

![image](https://github.com/user-attachments/assets/6abc3a4b-5953-47b0-a254-d02f8f764915)
![image](https://github.com/user-attachments/assets/e89c6901-953c-498f-acd6-a56a99f40f39)
![image](https://github.com/user-attachments/assets/2f719b4d-b550-4685-be32-16f2831d7431)
![image](https://github.com/user-attachments/assets/8711af48-c86b-4f99-afd9-fd3229d0ade4)
![image](https://github.com/user-attachments/assets/6229c6cf-d533-49a9-90f9-2b11deb5e832)
![image](https://github.com/user-attachments/assets/e9082918-ed31-4f08-b399-0ee6672f9042)
![image](https://github.com/user-attachments/assets/7fcc9add-a78d-4eba-acbb-fd3727c8d49b)
![image](https://github.com/user-attachments/assets/9f2317ad-6543-42b2-b806-6cecf5f94ca1)
![image](https://github.com/user-attachments/assets/b1f409c9-487c-4c91-a772-bd41d2a159d7)
![image](https://github.com/user-attachments/assets/1bbc7e42-880f-4cd9-b02f-c610e9a0239c)
![image](https://github.com/user-attachments/assets/dfdf33af-6452-4af1-8386-a80d0282ad96)
![image](https://github.com/user-attachments/assets/11affb03-eafd-4f5b-8abf-9c705f36b586)
<img width="850" alt="image" src="https://github.com/user-attachments/assets/808cd790-6cd9-4c20-b1b9-9421946d4b6c" />

![image](https://github.com/user-attachments/assets/6d939a29-e012-4e98-b2cb-f14b8018224f)
![image](https://github.com/user-attachments/assets/9a150875-15af-4ea2-a419-6a0392f1aed6)
![image](https://github.com/user-attachments/assets/f3ee9cb9-1f5d-4944-91dd-8d58681c3fcb)




# C. The file summarizing the prediction models includes the Accuracy, F1 score and Time Taken parameters and prediction execution time based on this dataset. 

#### C.1. This list of trained models sorted by fast execution time and high Balanced-Accuracy parameter

![image](https://github.com/user-attachments/assets/a82fa6a4-4ea2-42ad-ae53-740dc1bb0cde)



#### C.2. Quickly check other models through Accuracy, ROC AUC, F1 Score

![image](https://github.com/user-attachments/assets/e31e2bb1-91cd-4ded-bbaf-db1e5963f925)


# D. Results
- All models were trained and evaluated to identify the best-performing one for this multiclass classification task.
- Reusability on other datasets thanks to calling the pickle library to store the models.


