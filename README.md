## Pump it Up: Data Mining the Water Table
github Link : https://github.com/Abira16/DM_Water-Table_final/

### Introduction
This is a project to predict which water pumps are faulty

Using data from Taarifa and the Tanzanian Ministry of Water, Task to predict which pumps are functional, which need some repairs, and which don't work at all? This is an intermediate-level practice competition. Predict one of these three classes based on a number of variables about what kind of pump is operating, when it was installed, and how it is managed. A smart understanding of which waterpoints will fail can improve maintenance operations and ensure that clean, potable water is available to communities across Tanzania.

### Steps to predict the tasks

 #### 1. Import the required modules
   ```py
     import numpy as np
     import pandas as pd
     
     # plotting
     %matplotlib inline
     import matplotlib.pyplot as plt
     import seaborn as sns
     from collections import Counter
     from matplotlib import pyplot
     
     # Train Test split 
     from sklearn.model_selection import train_test_split
     
     #preprocess
     from sklearn.impute import SimpleImputer
     from sklearn.compose import ColumnTransformer
     from sklearn.preprocessing import (OneHotEncoder, StandardScaler,FunctionTransformer)
      
     #classify & evaluvation
     from xgboost import XGBClassifier
     from sklearn.multiclass import OneVsRestClassifier
     from sklearn.pipeline import Pipeline
     from sklearn.model_selection import GridSearchCV
     from sklearn.metrics import plot_confusion_matrix
```
  #### 2. Import data and make test train split
  
  #### 3. Preprocessing
  Identify the categorical, numerical variables.
  Change categorical columns to string, fill all missing values, one-hot encode to all categorical variables.
  For the missing values in the numerical variables, filll with median value from the column, scale each variable have mean zero and deviation one.
  Drop some columns
   
   #### 4. Model building and training
   Build the model using XGBClassifier.
   
   #### 5. Predict and Validation Data
   #### 6. Confusion matrix analysis
    
