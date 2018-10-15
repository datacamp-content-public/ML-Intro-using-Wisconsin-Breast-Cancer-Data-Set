---
title: 'Exploratory Data Analysis'
description: 'Explore imported data'
---

## Descriptive statistics on the data set attributes

```yaml
type: NormalExercise
key: 0c2943d19b
xp: 100
```

Explore the desriptive statistics for every single column in the dataset

`@instructions`
Python offers a very easy method to obtain the descriptive statistics through the command `dataframe.describe()`

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
breast_cancer.describe()
```

`@solution`
```{python}
breast_cancer.describe()
```

`@sct`
```{python}
Ex().has_equal_output()
success_msg("Good job !")
```
