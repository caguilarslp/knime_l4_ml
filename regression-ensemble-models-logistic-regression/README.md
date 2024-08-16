# Exercise 03: Random Forest

## Learning Objective

In this exercise, you'll learn how to predict the price of a house in Ames, Iowa, USA, given a number of features such as size, neighborhood, and heating. The objective is to build a Random Forest model that predicts the overall condition ranking of houses based on these features.

## Workflow Description

This workflow uses a dataset describing the sale of individual residential properties in Ames, Iowa from 2006 to 2010. The dataset includes various features, one of which is the overall condition ranking of houses, with values ranging from 1 to 10.

## Steps

### Step 1: Random Forest Learner

- **Task:** Train a Random Forest model to predict the overall condition of a house (high/low).
- **Node:** Random Forest Learner
- **Settings:** Select the `rank` column as the target column. Leave other settings at their defaults.

### Step 2: Random Forest Predictor

- **Task:** Use the trained model to predict the rank of houses in the test set.
- **Node:** Random Forest Predictor

### Step 3: Model Evaluation

- **Task:** Evaluate the accuracy of the Random Forest model.
- **Node:** Scorer
- **Settings:** Select `rank` as the actual column and `Prediction (rank)` as the predicted column.
- **Question:** What is the accuracy of the model?

### Step 4: Parameter Optimization Loop Start (Optional)

- **Task:** Use the Parameter Optimization Loop Start node to define possible values for the tree depth and the number of models.
- **Node:** Parameter Optimization Loop Start
- **Instructions:** Connect the variable port to the Random Forest Learner node and use the created flow variables to overwrite the corresponding setting options in the Random Forest Learner node.

### Step 5: Parameter Optimization Loop End (Optional)

- **Task:** Use the Parameter Optimization Loop End node to define accuracy as the objective function.
- **Node:** Parameter Optimization Loop End
- **Question:** Which settings lead to the model with the highest accuracy?

## Screenshots

Include screenshots of key parts of the workflow, such as the Random Forest model training, prediction, and evaluation.
