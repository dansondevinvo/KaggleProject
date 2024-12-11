# Kaggle Project


This repository contains an attempt to use Logistic Regression for metastatic cancer diagnosis using clinical data from a Kaggle challenge.
https://www.kaggle.com/competitions/widsdatathon2024-challenge1/data

### Overview:

The task, as defined by the Kaggle challenge, is to predict the likelihood of metastasis in cancer patients using medical data. The dataset consists of various clinical and genomic features, and the goal is to classify whether a patient’s cancer will metastasize. The approach in this repository formulates the problem as regression task, using Logistic regression to predict whether cancer is metastatic or not and also used data preprocessing techniques like handling missing values and scaling numerical features. My best model had an accuracy of 61% during the machine learning test.

### Data:

- CSV file of clinical data
- Target Variable: DiagPeriodL90D
- 12906 Rows
- 83 Columns

### Preprocessing:

- Handled missing values
- Feature scaling
- Removed outliers
- Encode categorical variables
- Removed duplicates

<img width="938" alt="Screenshot 2024-12-11 at 11 17 12 AM" src="https://github.com/user-attachments/assets/fa9f089d-1203-4ffc-b14b-e5ac1e321384" />


### Problem Formulation:

- Input / Output:
  tabular data / binary classification
- Logistic regression model: predicts probability of metastatis,
  great for binary classification, fast to train
  
### Training:

- Used Scikit-learn's Logistic Regression model
- model.fit(x_train, y_train)
- Fast to train, about 1 minute

### Overview of files in repository:

- training.csv.zip: metastatic cancer dataset
- KaggleProject(2).ipynb: processes dataset, displays visuals, and trains model
- kagglesubmission.csv: submission file after test



