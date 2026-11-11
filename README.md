# 🚗 Car Price Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on predicting automobile prices in the American market using Machine Learning regression techniques.

A Chinese automobile company plans to enter the US market and wants to understand the factors influencing car prices. The objective is to develop predictive models that identify important pricing variables and estimate automobile prices based on their characteristics.

This project compares five regression algorithms to determine which model provides the best predictive performance.

## 🎯 Business Objective

The main objectives of this project are:

- Identify the significant variables affecting automobile prices.
- Understand how different car characteristics influence pricing.
- Develop machine learning models to predict car prices.
- Compare the performance of different regression algorithms.
- Identify the best-performing model.
- Perform hyperparameter tuning to improve model performance.
- Provide insights to support data-driven pricing decisions.

## 📂 Dataset Description

**Dataset Name:** CarPrice_Assignment.csv

The dataset contains 205 observations and 26 columns describing different automobile characteristics.

It includes information related to:

- Car specifications
- Fuel type
- Engine characteristics
- Horsepower
- Car dimensions
- Body type
- Manufacturer
- Automobile price

**Target Variable:** `price`

The target variable represents the price of the automobile.

## 🛠️ Technologies and Libraries Used

**Programming Language:**
- Python

**Development Environment:**
- Jupyter Notebook

**Libraries:**
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Scikit-learn – Machine Learning and model evaluation
- Joblib – Model saving

## ⚙️ Project Workflow

### 1. Data Loading and Understanding
- Loaded the dataset using Pandas.
- Examined dataset dimensions and data types.
- Checked missing values and duplicate records.
- Identified numerical and categorical variables.

### 2. Exploratory Data Analysis (EDA)
- Analyzed car price distribution.
- Identified potential outliers using boxplots.
- Examined correlations using a heatmap.
- Visualized relationships between horsepower, engine size, car body type, fuel type, and price.

### 3. Data Preprocessing
- Removed unnecessary identification columns.
- Extracted manufacturer names from car names.
- Standardized manufacturer name variations.
- Identified numerical and categorical features.
- Applied One-Hot Encoding to categorical variables.
- Applied StandardScaler to numerical variables.
- Created preprocessing pipelines.

### 4. Train-Test Split

The dataset was divided into:

- 80% Training Data
- 20% Testing Data

A random state of 42 was used to ensure reproducibility.

### 5. Model Implementation

Five regression algorithms were implemented:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor
5. Support Vector Regressor (SVR)

### 6. Model Evaluation

The models were evaluated using the following metrics:

| Metric | Description |
|---|---|
| R² Score | Measures the proportion of variance explained by the model. Higher is better. |
| Mean Squared Error (MSE) | Measures the average squared prediction error. Lower is better. |
| Mean Absolute Error (MAE) | Measures the average absolute prediction error. Lower is better. |

The evaluation metrics were used to compare all five models and identify the best-performing algorithm.

### 7. Feature Importance Analysis

Permutation Importance was used to identify the most influential variables affecting car price predictions.

This analysis helps understand which automobile characteristics contribute most to the predictive performance of the selected model.

### 8. Hyperparameter Tuning

GridSearchCV was implemented to optimize the hyperparameters of the best-performing model.

Five-fold cross-validation was used to identify the optimal parameter combination.

The tuned model was evaluated and compared with the original model to check for performance improvement.

### 9. Final Model Evaluation

The final model was further evaluated using:

- Actual vs Predicted Price Plot
- Residual Distribution Plot
- Residuals vs Predicted Values Plot

These visualizations help assess prediction accuracy and model performance.

## 📊 Model Comparison

The five regression models are compared based on:

- R² Score
- Mean Squared Error
- Mean Absolute Error

The best-performing model is selected based on its overall predictive performance on the testing dataset.

Actual evaluation results are generated when the notebook is executed.

## 📁 Project Structure

```text
Car-Price-Prediction/
│
├── CarPrice_Assignment.csv
│
├── Codeathon - Intermediate Assessment.ipynb
│
├── car_price_prediction_model.pkl
│
└── README.md
```

## ▶️ How to Run This Project

**Step 1: Clone the repository**

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

**Step 2: Navigate to the project directory**

```bash
cd Car-Price-Prediction
```

**Step 3: Install the required libraries**

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib jupyter
```

**Step 4: Launch Jupyter Notebook**

```bash
jupyter notebook
```

**Step 5: Open and execute**

Open `Codeathon - Intermediate Assessment.ipynb` and execute the cells sequentially.

Ensure that `CarPrice_Assignment.csv` is available in the same project directory.

## 💡 Key Learning Outcomes

Through this project, I gained practical experience in:

- Data cleaning and preprocessing.
- Exploratory Data Analysis.
- Feature engineering.
- Categorical encoding and feature scaling.
- Regression model development.
- Model evaluation and comparison.
- Feature importance analysis.
- Cross-validation and hyperparameter tuning.
- Building end-to-end Machine Learning workflows using Python.

## 🏁 Conclusion

This project demonstrates the application of Machine Learning regression techniques to automobile price prediction.

By implementing and comparing five regression algorithms, the project aims to identify an appropriate predictive model and understand the important factors influencing automobile prices.

The findings can help automobile companies understand market pricing patterns and make informed business decisions.

---

**Project Category:** Machine Learning | Supervised Learning | Regression

**Developed using:** Python and Scikit-learn
