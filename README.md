# Student Placement Prediction Using Logistic Regression

## 📌 Project Overview

This project uses **Logistic Regression** to predict whether a student is likely to be **Placed** or **Not Placed** based on academic performance, skills, internships, projects, and other student-related factors.

The dataset is already divided into separate training and testing files.

## 🎯 Objective

The main objective of this project is to build a simple binary classification model that can predict student placement status.

## 📊 Dataset

* Training data: 45,000 records
* Testing data: 5,000 records
* Target variable: `Placement_Status`

### Features Used

* Age
* Gender
* Degree
* Branch
* CGPA
* Internships
* Projects
* Coding Skills
* Communication Skills
* Aptitude Test Score
* Soft Skills Rating
* Certifications
* Backlogs

`Student_ID` was not used as a model feature because it is only an identifier.

## 🛠️ Technologies Used

* Python
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## 🔄 Project Workflow

1. Load the training and testing datasets
2. Understand the dataset
3. Check missing values
4. Check duplicate records
5. Separate features and target
6. Identify numerical and categorical features
7. Apply preprocessing using `ColumnTransformer`

   * `StandardScaler` for numerical features
   * `OneHotEncoder` for categorical features
8. Build a Logistic Regression model using a Pipeline
9. Train the model
10. Predict placement status on the test dataset
11. Evaluate the model
12. Predict placement for a new student

## 🤖 Machine Learning Model

**Logistic Regression** is used because the target variable contains two possible outcomes:

* `Placed`
* `Not Placed`

The preprocessing and model are combined using a Scikit-learn Pipeline.

```python
Pipeline([
    ('preprocessor', preprocessor),
    ('classifier', LogisticRegression())
])
```

## 📈 Model Evaluation

The model is evaluated using:

* Accuracy
* Confusion Matrix
* Precision
* Recall
* F1-score

A confusion matrix is also visualized using Seaborn.

## 🔮 New Student Prediction

The trained model can also take the details of a new student and predict:

* Placement status
* Probability of being placed

This makes the project more practical than simply evaluating the model on the test dataset.

## 📁 Project Structure

```text
Student-Placement-Prediction/
│
├── Logistic_Regression_Project.ipynb
├── train.csv
├── test.csv
└── README.md
```

## 🎯 Key Learning

Through this project, I learned how to build a classification model using Logistic Regression and how to handle both numerical and categorical features using `ColumnTransformer`, `StandardScaler`, and `OneHotEncoder`.

I also learned how to use a Pipeline to combine preprocessing and model training into a single workflow.

## 👤 Author

**Sahil Shinde**
