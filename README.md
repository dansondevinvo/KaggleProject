# Kaggle Project


This repository contains an attempt to use Logistic Regression for metastatic cancer diagnosis using clinical data from a Kaggle challenge.
https://www.kaggle.com/competitions/widsdatathon2024-challenge1/data

### Overview:

The task, as defined by the Kaggle challenge, is to predict the likelihood of metastasis in cancer patients using medical data. The dataset consists of various clinical and genomic features, and the goal is to classify whether a patient’s cancer will metastasize. The approach in this repository formulates the problem as regression task, using Logistic regression to predict whether cancer is metastatic or not and also used data preprocessing techniques like handling missing values and scaling numerical features. My best model had an accuracy of 61% during the logistic regression task.
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


<img width="799" alt="Screenshot 2024-12-11 at 11 30 57 AM" src="https://github.com/user-attachments/assets/c6ce7a08-0a77-47ad-8a5a-73bace955537" />


### Problem Formulation:

- Input / Output:
  Numerical data was scaled to range from [0,1] using min-max scaling and one-hot encoding used   
  to scale categorical variables to binary columns. //
  The output indicates whether metastatic cancer diagnosis occured within 90 days.
- Logistic regression model: predicts probability of metastatis,
  great for binary classification and very simple and effective,
  also fast to train
  
### Training:

- Import necessar libraries like pandas, numpy, sklearn
- Load and preprocess dataset and split data into features into sets
- Used Scikit-learn's Logistic Regression model
- model.fit(x_train, y_train)
- Fast to train, about 1 minute

### Overview of files in repository:

- training.csv.zip: metastatic cancer dataset
- KaggleProject(2).ipynb: processes dataset, displays visuals, and trains model
- kagglesubmission.csv: submission file after test



