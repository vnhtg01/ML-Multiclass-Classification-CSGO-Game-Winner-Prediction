
![image](https://github.com/user-attachments/assets/392f1ae5-83e5-4502-975a-053949bda7c2)




# ML Multiclass Classification Project for CSGO Game Winner Prediction

## A. Objective
Build a machine learning model to perform **Multiclass classification** based on a real dataset from Kaggle. Project done in python on jupyter notebook.
#### Notes : Class `0` represents *Lost*, class `1` represents *Tie (Draw)*, class `2` represents *Win*.

## B. Pipeline Overview
1. **Data Import** : not included
2. **Exploratory Data Analysis (EDA) & Data Visualization**  
   - Check for missing values  
   - Analyze variable distributions  
   - Compute correlation matrix
   - Create a report of dataset from ydata_profiling
3. **Data Preprocessing**  
   - Standardization (scaling)
   - Train/Test split
   - (Bonus) GridSearchCV to find the best hyperparameter
4. **Model Training** 
   - Logistic Regression  
   - Decision Tree  
   - Random Forest
   - (Bonus) LazyPredict to show performances of 30-40 differents models
5. **Model Evaluation** 
   - Accuracy, Precision, Recall, F1-score  
   - Classification report  
   - Confusion matrix
6. **Model Deployment** : not included

## C. Report File extracted by ydata_profiling

## D. The file summarizing the prediction models includes the Accuracy, F1 score and Time Taken parameters and prediction execution time based on this dataset. 

#### D.1. This list of trained models sorted by fast execution time and high A-parameter

![image](https://github.com/user-attachments/assets/c9f57597-cf36-4983-b4b3-ac684d975bdb)


#### D.2. Top 5 as horizontal bar chart

![image](https://github.com/user-attachments/assets/6fdd69b0-aae6-4fe0-843e-fdc674067ba0)

## E. Results
- All models were trained and evaluated to identify the best-performing one for this multiclass classification task.
- Reusability on other datasets thanks to calling the pickle library to store the models.


