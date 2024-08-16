# Credit Scoring

## Project Overview

Credit scoring is a technique used to determine whether or not to extend credit (and if so, how much) to a borrower. This workflow illustrates the process of creating and selecting a credit scoring model using historical data combined with various machine learning algorithms.

## Task

The objective of this project is to create a credit scoring model based on historical credit data. The workflow involves selecting the best machine learning algorithm for this purpose and evaluating the model's performance using cross-validation.

## Data Reading

The dataset used for this project is the German Credit data, which includes credit status, demographic information, and customer history. The dataset can be found in the `TheData/Credit` directory.

## Pre-processing

To prepare the data for model training, all nominal columns are converted into numerical columns, as certain machine learning algorithms, such as Neural Networks and Support Vector Machines (SVM), require numerical input.

## Model Training and Evaluation

The following machine learning algorithms are trained and evaluated using cross-validation within this workflow:

- Neural Network
- Support Vector Machines (SVM)
- Decision Tree

The cross-validation process helps in assessing the performance of each model to ensure the selection of the best one.

## Model Selection

After training, the results from all models, including their respective accuracies, are compiled into a single table. The models are then sorted by descending accuracy, and only the best-performing model is retained for further use.

## Visualize

The accuracy scores of the three models are compared to determine which model performs best. This comparison is visualized to provide a clear understanding of the relative performance of each algorithm.

## Save the Model

The best model is converted back into the PMML (Predictive Model Markup Language) format. KNIME Analytics Platform then saves the model in PMML, allowing it to be used in other applications or systems.

---

This README file provides a detailed overview of the steps and processes involved in creating a credit scoring model using KNIME. The actual workflow is included in the repository, and the necessary data files and scripts are organized in their respective folders.
