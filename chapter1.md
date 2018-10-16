---
title: 'Loading Data'
description: 'Loading Wisconsin Breast Cancer Data Set'
---

## Loading the data

```yaml
type: NormalExercise
key: c909bf2ad1
lang: python
xp: 100
skills: 2
```

In this exercise you will build a machine learning model. The following steps will be covered:

1. Loading the data set
2. Exploratory Data Analysis to understand the variables and the associated values
3. Selecting the features
4. Splitting the data in a training and a test dataset
5. Applying a machine learning model on the training data
6. Applying that model to the test data
7. Evaluating the results

The dataset that will be used for this exercise is the Wisconsin Breast Cancer Data Set (available through the UW CS ftp server: ftp ftp.cs.wisc.edu cd math-prog/cpo-dataset/machine-learn/WDBC/). 

32 variables are determined on basis of a fine needle aspirate (FNA) of a breast mass. The variables describe characteristics of the cell nuclei present in the image. For each sample, there is an outcome variable (diagnosis), indicating whether the tumor is benign (0) or malignant (1)

`@instructions`
Data is loaded into a dataframe `breast_cancer` . Check the first 5 rows of data via the command `dataframe.head(n=5)` . Don't forget to replace the `dataframe` tag with the actual name.

`@hint`


`@pre_exercise_code`
```{python}
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split 
from sklearn.model_selection import KFold, cross_val_score 
from sklearn.ensemble import RandomForestClassifier 
from sklearn.metrics import roc_curve
from sklearn.metrics import auc
from urllib.request import urlopen

plt.style.use('ggplot')

UCI_data_URL = 'https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data'

names = ['id_number', 'diagnosis', 'radius_mean', 
         'texture_mean', 'perimeter_mean', 'area_mean', 
         'smoothness_mean', 'compactness_mean', 'concavity_mean',
         'concave_points_mean', 'symmetry_mean', 
         'fractal_dimension_mean', 'radius_se', 'texture_se', 
         'perimeter_se', 'area_se', 'smoothness_se', 
         'compactness_se', 'concavity_se', 'concave_points_se', 
         'symmetry_se', 'fractal_dimension_se', 
         'radius_worst', 'texture_worst', 'perimeter_worst',
         'area_worst', 'smoothness_worst', 
         'compactness_worst', 'concavity_worst', 
         'concave_points_worst', 'symmetry_worst', 
         'fractal_dimension_worst'] 

breast_cancer = pd.read_csv(urlopen(UCI_data_URL), names=names)

# Convert diagnosis to binary 
breast_cancer['diagnosis'] = breast_cancer['diagnosis']\
  .map({'M':1, 'B':0})
```

`@sample_code`
```{python}
#read Wisconsin breast cancer data set
breast_cancer = pd.read_csv(urlopen(UCI_data_URL), names=names)

# Convert diagnosis to binary : M=1, B=0
breast_cancer['diagnosis'] = breast_cancer['diagnosis'].map({'M':1, 'B':0})

# Display first 5 rows of the dataframe
breast_cancer.head()
```

`@solution`
```{python}
#read Wisconsin breast cancer data set
breast_cancer = pd.read_csv(urlopen(UCI_data_URL), names=names)

# Convert diagnosis to binary : M=1, B=0
breast_cancer['diagnosis'] = breast_cancer['diagnosis'].map({'M':1, 'B':0})

# Display first 5 rows of the dataframe
breast_cancer.head(n=5)
```

`@sct`
```{python}
Ex().has_equal_output()
success_msg("Some praise! Then reinforce a learning objective from the exercise.")
```
