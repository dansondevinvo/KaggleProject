# Kaggle Project: Metastatic Cancer Diagnosis


This repository contains an attempt to use Logistic Regression for metastatic cancer diagnosis using clinical data from a Kaggle challenge.
https://www.kaggle.com/competitions/widsdatathon2024-challenge1/data

### Overview:

The task, as defined by the Kaggle challenge, is to predict the likelihood of metastasis in cancer patients using medical data. The dataset consists of various clinical and genomic features, and the goal is to classify whether a patient’s cancer will metastasize. The approach in this repository formulates the problem as regression task, using Logistic regression to predict whether cancer is metastatic or not and also used data preprocessing techniques like handling missing values and scaling numerical features. My best model had an accuracy of 61% during the logistic regression task.
### Data:

The dataset for this metastatic cancer diagnosis project consists of a CSV file of clinical data containing 12,906 rows and 83 columns. The target variable is "DiagPeriodL90D", which serves as the primary label for classification

### Preprocessing:

- Handled missing values: Numerical features were replaced with the median. Categorical features were replaced with the mode.
- Feature scaling: Min-max scaling was used to transfor values to a standard range for Logistic Regression 
- Removed outliers: Outliers identified by IQR and removed
- Encode categorical variables: One-hot encoding was used to scale categorical variables
- Removed duplicates: Prevent redundant information


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

The training process for the metastatic cancer diagnosis model began with importing essential libraries such as Pandas, NumPy, and Scikit-learn to facilitate data manipulation and machine learning. The clinical dataset was loaded and preprocessed by handling missing values, scaling features, encoding categorical variables, and removing duplicates and outliers. The data was then split into training and testing sets to evaluate model performance. For model training, Scikit-learn's Logistic Regression was used since it's very simple yet effective. The model was trained using the fit() method on the training data (X_train, y_train). Training was very quick taking about 1 minute to complete because simplicity of logistic regression and the dataset size.

### Conclusions

My model had an accuracy of 61%. Logistic regression worked well but can definitely be tuned to perform better and result in a higher accuracy. It was a practical machine learining model to use for this dataset and some improvements could make predictions more precise.

### How to Reproduce Results:

To reproduce the results of the metastatic cancer diagnosis kaggle project, I would start by recreating the repository and installing the required libraries, including Pandas, NumPy, and Scikit-learn. Then, preprocess the dataset using the preprocessing.py script, which handles missing values, scales features, and encodes categorical variables. Next, I would train the logistic regression model using the train_model.py script, which trains the model and saves it as model.pkl. For applying the model to new data, load the trained model, preprocess the new dataset in the same way, and use the model to make predictions. This package can also be applied to other similar datasets by adjusting the model's parameters, and evaluating performance.

### Overview of files in repository:

- training.csv.zip: metastatic cancer dataset
- KaggleProject(2).ipynb: processes dataset, displays visuals, and trains model
- kagglesubmission.csv: submission file after test

### Citations:

https://www.kaggle.com/competitions/widsdatathon2024-challenge1/data

