# Loan Status Prediction

This project demonstrates a machine learning model for predicting loan status based on various applicant attributes. The dataset used contains historical data of applicants and their loan status, and the model is trained using a Support Vector Machine (SVM).

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [How to Use](#how-to-use)

---

## Introduction

Loan status prediction is a critical task for financial institutions to assess the risk associated with loan approvals. This project uses a Support Vector Machine (SVM) classifier to predict whether a loan will be approved based on applicant details like income, credit history, property area, and more.

---

## Dataset

The dataset contains the following features:
- **Loan_ID**: Unique identifier for each loan
- **Gender**: Gender of the applicant
- **Married**: Marital status of the applicant
- **Dependents**: Number of dependents
- **Education**: Education level of the applicant
- **Self_Employed**: Employment status
- **ApplicantIncome**: Income of the applicant
- **CoapplicantIncome**: Income of the co-applicant
- **LoanAmount**: Loan amount applied for
- **Loan_Amount_Term**: Term of the loan
- **Credit_History**: Credit history of the applicant
- **Property_Area**: Type of property area (Rural, Semiurban, Urban)
- **Loan_Status**: Target variable (Loan approved: 1, Loan not approved: 0)

---

## Dependencies

The following Python libraries were used:
- `numpy`
- `pandas`
- `seaborn`
- `scikit-learn`

To install these dependencies, run:
```bash
pip install numpy pandas seaborn scikit-learn
```

---

## Data Preprocessing
- **Handling Missing Values**: Missing values in the dataset were removed to ensure data consistency.
- **Label Encoding**: Categorical features like Loan_Status, Gender, and Property_Area were converted into numerical values for model compatibility.
- **Feature Transformation**: The target variable (Loan_Status) was encoded as 0 for "N" and 1 for "Y".

---

## Exploratory Data Analysis (EDA)
- **Loan Status by Education**: Analyzed the relationship between loan approval and education level.
- **Loan Status by Marital Status**: Explored how marital status affects loan eligibility.

---

## Model Training and Evaluation

### Model
**Support Vector Machine (SVM)**: A linear kernel SVM was trained on the preprocessed data.

### Performance Metrics
- Training Accuracy: 79.86%
- Test Accuracy: 83.33%

---

## How to Use

1. Clone the repository and navigate to the project directory:
   ```bash
    git clone https://github.com/iDharitri-Raj/Loan_Status_Prediction
    cd Loan_Status_Prediction
   ```
2. Install the dependencies.
3. Run the script to train the model and evaluate it.

---

## License
This project is licensed under the [**MIT License**](LICENSE) 
