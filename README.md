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

## Type of Regression Model

#### Simple Linear Regression
Pros - It can work any size of datasets, also it gives information about the relevence of features <br/>
Cons - It is Linear regression Assumption. If it has more than dependent varaible, It is not accurate

#### Polynomial Linear Regression
Pros - It can work any size of datasets, It works well in non-linear problems <br/>
Cons - It need to choose right polynomial degreee for a good prediction

#### Support Vector Regression
Pros - It is easily adaptable. It works very well on non-linear problems, not biased by outfilters <br/>
Cons - It is compulsory to apply feature scaling

#### Decision Tree Regression
Pros - It doesn't need for feature scaling. It work on both linear / non-linear problem <br/>
Cons - It has poor results to small datasets overfitting can easily occur

#### Random Forest Regression
Pros - It is powerful and accurate, has good performance on many problems <br/>
Cons - It is overfitting can easily occur, need to choose of trees


# What If we can apply the stock market graph into a machine learning model?
Plans gets stock API first,
Display data in differen


# Deep learning: 
Deep Model : A netowrk with two or more hidden layer is considered
Depth is important
strscture model to reprsent an inheretnly composia


# Coding test
1. Two Sum
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
You can return the answer in any order.

 My answer
 ```
    def twoSum(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
        print(nums)
        result = target
        for first_index in range (0, len(nums)):
            first_n = nums[first_index]
            print(first_n)
            for second_index in range(first_index + 1, len(nums)):
                second_n = nums[second_index]
                print(second_n)
                if first_n + second_n == target:
                    return [first_index, second_index]
        return []
```
Another Approach
```
    def twoSum(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
        
        a=0
        for i in range(len(nums)):
            p = target-nums[i]
            if p in nums:
                a=nums.index(p)
                if a==i:
                    continue
                break
        return i,a
```
