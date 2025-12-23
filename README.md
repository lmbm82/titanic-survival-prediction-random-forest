# Titanic Survival Prediction with Random Forest

This project uses Machine Learning techniques to predict whether a passenger survived the Titanic disaster based on demographic and socio-economic features such as age, gender, class, and fare.

The dataset used is the well-known **"Titanic: Machine Learning from Disaster"** dataset from Kaggle.

## Objective
Build and evaluate a classification model capable of predicting passenger survival using structured data and ensemble learning.

## Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
  - RandomForestClassifier
  - train_test_split
  - accuracy_score
  - confusion_matrix

## Dataset
- Source: Kaggle Titanic Dataset
- Features used:
  - Pclass
  - Sex
  - Age
  - SibSp
  - Parch
  - Fare
  - Embarked (one-hot encoded)

## Data Preprocessing
- Missing values in **Age** filled with the mean
- Missing values in **Embarked** filled with the mode
- Dropped irrelevant columns: Cabin, Ticket, Name, PassengerId
- Encoded categorical variables:
  - Sex: male → 0, female → 1
  - Embarked: One-Hot Encoding

## Exploratory Data Analysis (EDA)
- Survival distribution
- Survival by gender
- Survival by passenger class
- Visualizations created using Seaborn and Matplotlib

## Model
A **Random Forest Classifier** was trained on the processed dataset:
- Train/Test split: 70% / 30%
- Random state set for reproducibility

## Results
- Test Accuracy: **~79.1%**
- The model shows good performance in predicting survival based on passenger features.

## Evaluation
- Confusion Matrix visualization
- Accuracy metric used for performance assessment

## Files
- `titanic_survival_random_forest.ipynb` — Main Jupyter Notebook with full analysis and model

## Notes
This project was developed as part of Machine Learning practice to demonstrate data preprocessing, exploratory analysis, and supervised classification using ensemble methods.
