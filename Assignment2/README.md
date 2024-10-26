# Titanic - Machine Learning from Disaster

This project aims to predict passenger survival on the Titanic using **decision tree** models and **ensemble techniques** such as **Random Forest**, **XGBoost**, and **Decision Tree**. This repository includes the dataset, model code, and results, achieving an accuracy score of **0.83798**.

## Assignment Overview

The Titanic dataset provides information about the passengers, including demographics and ticket information, allowing us to predict survival outcomes based on these features. 

### Dataset Structure

The dataset consists of two main files:
1. **Training Set (`train.csv`)**: Contains labeled data to train the machine learning model.
2. **Test Set (`test.csv`)**: Contains unlabeled data to evaluate model performance.

An additional file, `gender_submission.csv`, serves as a baseline prediction example, assuming only female passengers survive.

### Data Dictionary

| Column     | Definition                         | Key                                             |
|------------|------------------------------------|-------------------------------------------------|
| `survival` | Survival outcome                   | 0 = No, 1 = Yes                                 |
| `pclass`   | Ticket class                       | 1 = 1st, 2 = 2nd, 3 = 3rd                       |
| `sex`      | Gender                             | Male, Female                                    |
| `age`      | Age in years                       | Fractional for under 1; estimates use `xx.5`    |
| `sibsp`    | Siblings/spouses aboard            | Integer                                         |
| `parch`    | Parents/children aboard            | Integer                                         |
| `ticket`   | Ticket number                      | Alphanumeric                                    |
| `fare`     | Passenger fare                     | Float                                           |
| `cabin`    | Cabin number                       | Alphanumeric                                    |
| `embarked` | Port of Embarkation                | C = Cherbourg, Q = Queenstown, S = Southampton  |

### Important Variable Notes

- **pclass** indicates socio-economic status:
  - 1st = Upper class
  - 2nd = Middle class
  - 3rd = Lower class
- **age** is fractional for ages below 1 and estimated ages use `.5`.
- **sibsp** and **parch** define family relations:
  - **sibsp** includes siblings and spouses (excludes fiancés or mistresses).
  - **parch** includes parents and children, excluding nannies or unrelated guardians.

### Steps

1. **Data Preprocessing**: Handle missing values, encode categorical features, and scale numerical values.
2. **Model Training**: Train RandomForest, XGBoost, or AdaBoost models using `train.csv`.
3. **Model Evaluation**: Evaluate model accuracy on `test.csv`, yielding a score of **0.83798**.


### Implementation

- **Assignment2.ipynb**: contains code to train and test various models as mentioned before.

### Result

- **output (43).csv** contains output that leads to accuray of 0.83798 on test data using RandomForest and hypermeter tuning.  
   
