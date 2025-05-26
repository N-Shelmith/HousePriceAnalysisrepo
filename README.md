# HousePriceAnalysisrepo
# 🏠 King County House Price Prediction

This notebook is part of a final data analysis project where I worked as a Data Analyst for a Real Estate Investment Trust (REIT). The goal was to analyze residential housing data and build predictive models to estimate home prices based on features such as square footage, location, number of bedrooms, and more.

---

## 📊 Dataset
The dataset contains information on houses sold in King County (Seattle), including:
- House features (e.g., bedrooms, bathrooms, sqft_living, floors)
- Geographical data (lat, long, zipcode)
- Renovation details and year built
- Price (target variable)

---

## 📌 Key Tasks Performed

### 1. **Data Import and Cleaning**
- Loaded the housing dataset.
- Handled missing values in `bedrooms` and `bathrooms` using mean imputation.
- Dropped unnecessary columns like `id` and `Unnamed: 0`.

### 2. **Exploratory Data Analysis (EDA)**
- Used `value_counts()` to inspect the distribution of categorical features.
- Applied seaborn `boxplot` and `regplot` to identify price outliers and feature correlations.
- Computed Pearson correlation to determine the strongest predictors of price.

### 3. **Model Development**
- Built and evaluated several regression models:
  - **Simple Linear Regression** with single features.
  - **Multiple Linear Regression** using selected predictors.
  - **Pipeline with Polynomial Features** to capture non-linear relationships.

### 4. **Model Evaluation and Refinement**
- Used **Ridge Regression** with regularization (`alpha = 0.1`) to avoid overfitting.
- Applied **Polynomial Transformation (degree=2)** to improve model accuracy.
- Split data into training and test sets and calculated **R²** scores for evaluation.

---

## 📈 Results

| Model                        | R² Score (Test) |
|-----------------------------|-----------------|
| Linear Regression (sqft)    | 0.4929          |
| Multiple Linear Regression  | 0.6577          |
| Ridge Regression            | 0.6478          |
| Ridge + Polynomial (deg=2)  | **0.7003** ✅    |

---

## ✅ Tools Used
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn (Regression, Pipelines, Polynomial Features)
- Jupyter Notebook / JupyterLite

---

## 📌 Final Thoughts
This project enhanced my ability to:
- Perform end-to-end regression analysis.
- Preprocess and visualize real-world data.
- Build and tune models to improve prediction accuracy.

---

## 📁 File
- `House_Sales_in_King_Count_USA-20231003-1696291200.jupyterlite (1).ipynb`: Full analysis notebook

---


