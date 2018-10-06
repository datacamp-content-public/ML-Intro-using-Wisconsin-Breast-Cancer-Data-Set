---
title: Test
description: Test
---

## Loading the data

```yaml
type: NormalExercise
key: c909bf2ad1
lang: python
xp: 100
skills: 2
```

In this exercise we are going to follow what steps are followed to build a machine learning model. The following steps will be covered:

1. Loading the data set
2. Exploratory Data Analysis to understand the variables and the associated values
3. Selecting the features
4. Splitting the data in a training and a test dataset
5. Applying a machine learning model on the training data
6. Applying that model to the test data
7. Evaluating the results

The dataset that will be used for this exercise is the Wisconsin Breast Cancer Data Set (available through the UW CS ftp server: ftp ftp.cs.wisc.edu cd math-prog/cpo-dataset/machine-learn/WDBC/). 

32 variables are determined on basis of a fine needle aspirate (FNA) of a breast mass. The variables describe characteristics of the cell nuclei present in the image. For each sample, there is an outcome variable (diagnosis), indicating whether the tumor is benign (B) or malignant (M)

This is the list of variables

1-id: ID number
2-diagnosis: The diagnosis of breast tissues (M = malignant, B = benign)
3-radius_mean: mean of distances from center to points on the perimeter
4-texture_mean: standard deviation of gray-scale values
5-perimeter_mean: mean size of the core tumor
area_mean
smoothness_meanmean of local variation in radius lengths
compactness_meanmean of perimeter^2 / area - 1.0
concavity_meanmean of severity of concave portions of the contour
concave points_meanmean for number of concave portions of the contour
symmetry_mean
fractal_dimension_meanmean for "coastline approximation" - 1
radius_sestandard error for the mean of distances from center to points on the perimeter
texture_sestandard error for standard deviation of gray-scale values
perimeter_se
area_se
smoothness_sestandard error for local variation in radius lengths
compactness_sestandard error for perimeter^2 / area - 1.0
concavity_sestandard error for severity of concave portions of the contour
concave points_sestandard error for number of concave portions of the contour
symmetry_se
fractal_dimension_sestandard error for "coastline approximation" - 1
radius_worst"worst" or largest mean value for mean of distances from center to points on the perimeter
texture_worst"worst" or largest mean value for standard deviation of gray-scale values
perimeter_worst
area_worst
smoothness_worst"worst" or largest mean value for local variation in radius lengths
compactness_worst"worst" or largest mean value for perimeter^2 / area - 1.0
concavity_worst"worst" or largest mean value for severity of concave portions of the contour
concave points_worst"worst" or largest mean value for number of concave portions of the contour
symmetry_worst
fractal_dimension_worst"worst" or largest mean value for "coastline approximation" - 1


`@instructions`
- Instruction 1
- Instruction 2
- Instruction 3

`@hint`
- Here is the hint for this setup problem. 
- It should get students 50% of the way to the correct answer.
- So don't provide the answer, but don't just reiterate the instructions.
- Typically one hint per instruction is a sensible amount.

`@pre_exercise_code`
```{python}
# Load datasets and packages here.
```

`@sample_code`
```{python}
# Your
# sample
# code
# should
# be
# ideally
# 10 lines or less,
# with a max
# of 16 lines.
```

`@solution`
```{python}
# Answer goes here
# Make sure to match the comments with your sample code
# to help students see the differences from solution
# to given.
```

`@sct`
```{python}
# Update this to something more informative.
success_msg("Some praise! Then reinforce a learning objective from the exercise.")
```
