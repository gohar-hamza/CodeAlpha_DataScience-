# CodeAlpha_DataScience

This repository contains the tasks I completed during my remote internship in **Data Analytics / Data Science at CodeAlpha**. It showcases my work, learning, and practical implementation of data analysis and machine learning concepts using Python.

## 📌 About This Repository

The purpose of this repository is to organize and present all internship tasks in a clear and professional way. Each task includes the problem statement, objective, tools used, implementation steps, results, and key learning outcomes.

## 🧠 Internship Focus

During this internship, I worked on practical data science tasks involving:

- Data loading and exploration
- Data cleaning and preprocessing
- Exploratory Data Analysis
- Data visualization
- Machine learning model training
- Model evaluation
- Classification and prediction
- Jupyter Notebook documentation

## 🛠️ Tools and Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- GitHub

## 📂 Repository Structure

```text
CodeAlpha_DataScience/
│
├── Task_1/
│   └── task_1_notebook.ipynb
│
├── Task_2/
│   └── task_2_notebook.ipynb
│
├── Task_3/
│   └── task_3_notebook.ipynb
│
├── Task_4/
│   └── task_4_notebook.ipynb
│
├── README.md
└── requirements.txt
```

> Note: You can rename the notebook files according to your actual task names.

---

# ✅ Completed Internship Tasks

## Task 1: Iris Flower Classification

### 📌 Task Objective

Use measurements of Iris flowers to train a machine learning model that classifies the flower species as:

- Setosa
- Versicolor
- Virginica

### 📊 Dataset Used

The Iris dataset was loaded using Scikit-learn. It contains flower measurements such as:

- Sepal length
- Sepal width
- Petal length
- Petal width

### 🧪 Steps Performed

1. Loaded the Iris dataset using Scikit-learn
2. Converted the dataset into a Pandas DataFrame
3. Explored the dataset using basic statistics
4. Visualized feature relationships
5. Split the data into training and testing sets
6. Trained a classification model
7. Evaluated model performance using accuracy, confusion matrix, and classification report
8. Tested the model on new flower measurements

### 🤖 Model Used

- Logistic Regression

### 📈 Results

The model successfully classified Iris flower species based on flower measurements and achieved strong accuracy on the test data.

### 📚 Key Learning

This task helped me understand basic supervised machine learning classification concepts, including features, target labels, train-test split, model training, prediction, and evaluation.

---

## Task 2: Unemployment Analysis with Python — Summary Report

## Dataset Used

This project uses two CSV files:

1. `Unemployment in India.csv`
2. `Unemployment_Rate_upto_11_2020.csv`

The main columns analyzed are:

- Region
- Date
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)
- Area, where available
- Region group, longitude, and latitude, where available

## Project Workflow

The Jupyter Notebook follows these seven steps:

1. Understand the dataset.
2. Clean the dataset.
3. Explore the data.
4. Visualize unemployment trends.
5. Analyze the Covid-19 impact.
6. Identify patterns and trends.
7. Present final insights.

## Key Results

| Metric | Result |
|---|---:|
| Average unemployment before Covid | 9.51% |
| Average unemployment during early Covid lockdown shock | 24.26% |
| Average unemployment after early shock | 11.90% |
| Peak unemployment month | May 2020 |
| Peak monthly unemployment rate | 24.88% |
| Average urban unemployment | 13.17% |
| Average rural unemployment | 10.32% |

## Regions with Highest Average Unemployment

| region           |   unemployment_rate |
|:-----------------|--------------------:|
| Tripura          |             28.3504 |
| Haryana          |             26.2832 |
| Jharkhand        |             20.585  |
| Bihar            |             18.9182 |
| Himachal Pradesh |             18.5404 |

## Regions with Lowest Average Unemployment

| region      |   unemployment_rate |
|:------------|--------------------:|
| Gujarat     |             6.66393 |
| Uttarakhand |             6.58296 |
| Assam       |             6.42808 |
| Odisha      |             5.65786 |
| Meghalaya   |             4.79889 |

## Regions Most Affected During Early Covid Lockdown Shock

| region     |   unemployment_rate |
|:-----------|--------------------:|
| Puducherry |             75.4167 |
| Jharkhand  |             57.1175 |
| Bihar      |             47.2475 |
| Tamil Nadu |             40.855  |
| Haryana    |             40.295  |

## Main Conclusion

The dataset shows a strong unemployment spike around April and May 2020. This suggests that the early Covid-19 lockdown period had a major effect on unemployment in India.

The analysis also shows that urban unemployment was generally higher than rural unemployment in this dataset. Some regions were affected much more strongly than others, which means regional policy responses are important.

## Important Interpretation Note

The dataset covers a limited time period, so it is better to describe the patterns as monthly trends rather than strong long-term seasonal trends. A true seasonal analysis usually requires multiple years of data.

---

