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

# Task 3: Car Price Prediction with Machine Learning

This project was completed as **Task 3** of the **CodeAlpha Data Science Internship**.

The goal of this project is to build a machine learning model that predicts the selling price of a used car based on features such as present price, age, mileage, fuel type, transmission, ownership history, seller type, and brand.

---

## Project Objectives

- Load and understand the used-car dataset
- Clean the data and check for missing values and duplicate rows
- Perform exploratory data analysis
- Create useful features such as `Car_Age` and `Brand`
- Study the correlation between numerical features
- Remove redundant and highly correlated features
- Prepare numerical and categorical variables for machine learning
- Train and compare multiple regression models
- Evaluate the models using suitable regression metrics
- Tune the best-performing model
- Analyze feature importance and prediction errors
- Save the trained model for future predictions

---

## Dataset

The dataset used in this project is the **Car Price Prediction – Used Cars** dataset available on Kaggle.

Kaggle dataset path used in the notebook:

```python
/kaggle/input/datasets/vijayaadithyanvg/car-price-predictionused-cars/car data.csv
```

### Main Columns

| Column | Description |
|---|---|
| `Car_Name` | Name or model of the car |
| `Year` | Manufacturing year |
| `Selling_Price` | Price at which the car was sold |
| `Present_Price` | Current showroom or market price |
| `Driven_kms` | Total kilometres driven |
| `Fuel_Type` | Petrol, Diesel, or CNG |
| `Selling_type` | Dealer or Individual |
| `Transmission` | Manual or Automatic |
| `Owner` | Number or category of previous owners |

The target variable is:

```text
Selling_Price
```

---

## Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas and inspected using:

- `head()`
- `shape`
- `info()`
- `describe()`

### 2. Data Cleaning

The notebook performs the following cleaning steps:

- Removes duplicate rows
- Checks missing values
- Removes unnecessary spaces from text columns
- Converts numerical columns to the correct data type
- Handles invalid negative values
- Removes rows with a missing target value

### 3. Feature Engineering

Two additional features are created:

#### Car Age

```python
Car_Age = Reference_Year - Year
```

`Car_Age` is more meaningful for prediction than the original manufacturing year.

#### Brand

The first word of `Car_Name` is extracted and used as the car brand.

Example:

```text
Maruti Swift -> maruti
Honda City -> honda
Toyota Corolla -> toyota
```

### 4. Exploratory Data Analysis

The notebook includes visualizations for:

- Selling price distribution
- Present price versus selling price
- Car age versus selling price
- Kilometres driven versus selling price
- Median selling price by fuel type
- Median selling price by seller type
- Median selling price by transmission type

### 5. Correlation Analysis

A numerical correlation matrix is created to study relationships between features.

Highly correlated features are identified using a threshold of:

```python
0.90
```

`Year` is removed because it contains the same information as `Car_Age`.

### 6. Data Preprocessing

A Scikit-learn preprocessing pipeline is used.

#### Numerical Features

- Missing-value imputation using the median
- Feature standardization using `StandardScaler`

#### Categorical Features

- Missing-value imputation using the most frequent category
- One-hot encoding using `OneHotEncoder`

Using a pipeline helps prevent data leakage.

### 7. Machine Learning Models

The following regression models are trained and compared:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regressor
- Extra Trees Regressor
- Gradient Boosting Regressor

### 8. Model Evaluation

The models are evaluated using:

- **MAE** — Mean Absolute Error
- **RMSE** — Root Mean Squared Error
- **R² Score**
- **5-Fold Cross-Validation**

Lower MAE and RMSE values indicate better performance, while a higher R² score indicates a stronger model.

### 9. Hyperparameter Tuning

The best tree-based model is selected and tuned using:

```python
RandomizedSearchCV
```

This improves model performance by testing different combinations of parameters.

### 10. Error Analysis

The final model is analyzed using:

- Actual versus predicted values
- Residual plots
- Residual distribution
- Largest prediction errors

### 11. Feature Importance

Permutation feature importance is used to determine which features contribute most to the model's predictions.

### 12. Model Saving

The trained model and project outputs are saved as:

```text
car_price_prediction_model.joblib
car_price_model_comparison.csv
car_price_test_predictions.csv
car_price_feature_importance.csv
```

The dataset covers a limited time period, so it is better to describe the patterns as monthly trends rather than strong long-term seasonal trends. A true seasonal analysis usually requires multiple years of data.

---

