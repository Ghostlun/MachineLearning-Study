# MachineLearning-Study
This is ML Study. It is based on Python code


## What is Machine-Learning?
<b>Machine Learning : </b>It is an algorithm to make decision-based on analyzing and learning data.
example: Netflix, music, youtube

## What is Deep-Learning?
<b>Deep-Learning : </b> Deep-learning is model of self-computing. Like, the model has a brain to learn a new technique.


## Before start coding:
We use many different libraries.
```python
  import pandas as pd
  import numpy as np
  import matplotlib.pyplot as plt
 ```
  
Always starts with setting up.
```python
  dataset = pd.read_csv('50_Startups.csv')
  X = dataset.iloc[:, :-1].values // X will always DV(dependent variable)
  y = dataset.iloc[:, -1].values // y will always IDV (independent variable)
```

## Machine learning model
### Regression
If the dependent variable and independent variable has a cautions relationship, it analyzes statical reasoning and degree of relationship.

#### Simple Linear Regression

#### Multiple Linear Regression
 
