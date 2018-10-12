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
After loading the data, we'll look at the first 5 rows via the command bc.head(n=x)

`@hint`


`@pre_exercise_code`
```{python}
import pandas as pd
import numpy as np
import matplotlib as mp
import seaborn as sns
```

`@sample_code`
```{python}

```

`@solution`
```{python}
bc.head(n=5)
```

`@sct`
```{python}
# Update this to something more informative.
success_msg("Some praise! Then reinforce a learning objective from the exercise.")
```
