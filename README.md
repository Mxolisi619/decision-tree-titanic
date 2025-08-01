# Titanic Survival Prediction with Decision Trees

This project explores the use of Decision Tree Classifiers to predict the survival of passengers aboard the Titanic. The model is trained and evaluated using the 
classic Titanic dataset, and the effects of tree depth on performance are analyzed.

## Objective

To build and evaluate a Decision Tree model that predicts passenger survival. The focus is on:
- Preprocessing the Titanic dataset.
- Training a full-depth decision tree.
- Evaluating and visualizing accuracy across various tree depths.
- Identifying the best-performing model based on development and test set performance.

## Dataset

- **Source**: `titanic.csv`
- **Target Variable**: `Survived`
- **Features Used**: 
  - Pclass
  - Sex (converted to dummy variables)
  - Age (filled missing with median)
  - SibSp
  - Parch
  - Fare
  - Embarked (converted to dummy variables)

## Steps Performed

1. Loaded and cleaned the dataset (`titanic.csv`).
2. Dropped irrelevant columns: `Cabin`, `PassengerId`, `Name`, `Ticket`.
3. Filled missing values in `Age` and `Embarked`.
4. Encoded categorical variables using one-hot encoding.
5. Split the data into training, development, and test sets (60%, 20%, 20%).
6. Trained a Decision Tree Classifier without depth restriction.
7. Plotted the full tree and computed dev set accuracy.
8. Trained models with `max_depth` from 2 to 10.
9. Plotted training and development accuracy to study overfitting and underfitting.
10. Reported test set accuracy for the best model.

## Results

The notebook includes:
- Visualizations of the decision trees.
- Accuracy plots showing performance over different tree depths.
- Final model evaluation on test data.

## Requirements

Install the required packages using:

```bash
pip install -r requirements.txt
