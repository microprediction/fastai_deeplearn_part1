# Lesson 7

- Live:  28-Apr-2020
- Time: 6:30 to 9pm PST  (9:30pm to midnight EST)
- 9:30pm 101 watching
- 10:30pm 177 watching

## Topics
- weight decay, regularization
- embedding
- PyTorch code
- Tablular

## Notebook
- Collaborative filtering:  https://github.com/fastai/course-v4/blob/5a9fca472f55a8186e62a21111deab119001e0df/nbs/08_collab.ipynb
- Tabular:  https://github.com/fastai/course-v4/blob/5a9fca472f55a8186e62a21111deab119001e0df/nbs/09_tabular.ipynb

## Regularization
- use for **overfitting**
- **weight decay** is also known as **L2 Regularization**
- in general, big coefficients are going to cause a big swing in the loss

## Embeddings
- index lookup into an array
  - computational shortcut to one hot encoding
- cardinality: number of levels of a variable

## Dataset 
- Blue Book for Bulldozers Kaggle Competition

## Random Forests:  Bagging
- to improve the random forests, use **bagging**
- randomly select subsets of data and train it
- then average the different versions of the models
- advantage to this is that these models have errors which are not correlated to each other

Here is the procedure that Breiman is proposing:
1. Randomly choose a subset of the rows of your data (i.e., "bootstrap replicates of your learning set")
2. Train a model using this subset
3. Save that model, and then return to step one a few times
4. This will give you a number of trained models. To make a prediction, predict using all of the models, and then take the average of each of those model's predictions.

## BAGGING
it means that we can improve the accuracy of nearly any kind of machine learning algorithm by training it multiple times, each time on a different random subset of data, and average its predictions.

## Leo Breiman: Random Forest
In 2001 Leo Breiman went on to demonstrate that this approach to building models, when applied to decision tree building algorithms, was particularly powerful. He went even further than just randomly choosing rows for each model's training, but also randomly selected from a subset of columns when choosing each split in each decision tree. He called this method the random forest

## OOB:  out-of-box
- review: remove each variable and how it impacts the R MSE

## Partial Dependence Plot

## Boosting
