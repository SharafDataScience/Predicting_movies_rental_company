# Movie Rental Demand Prediction System

This project is a machine learning-driven solution designed to **predict customer rental behavior** for a movie rental company. It helps the business **forecast movie demand**, **optimize inventory**, and **improve customer experience** through data-driven insights.

> Built using Python and machine learning libraries like scikit-learn, this project includes data preprocessing, exploratory analysis, model building, evaluation, and recommendations.

---


## Project Overview

The main goal of this project is to **predict the likelihood of movie rentals** based on historical customer and movie data. This model can support:

- **Inventory management** – Keep popular titles in stock.
- **Customer retention** – Identify high-value customers.
- **Marketing campaigns** – Target customers more effectively.

---

## Dataset Description

> Dataset used is assumed to contain customer transactions and movie metadata.  

Typical columns:
- `Customer_ID` – Unique ID per customer
- `Movie_ID` – Unique movie identifier
- `Genre`, `Year`, `Rating`, etc.
- `Rental_Date` – When the rental occurred
- `Rental_Status` – Target (e.g., 1 = rented, 0 = not rented)

---

## Project Workflow

---

### 1. Data Collection & Understanding
- Loaded customer, rental, and movie-related datasets.
- Reviewed data types, column descriptions, and basic statistics.
- Identified the target variable (`Rental_Status`) for prediction.

---

### 2. Data Preprocessing & Cleaning
- Removed missing values and irrelevant columns.
- Converted `Rental_Date` and `Release_Date` into datetime formats.
- Created features like `rental_month`, `days_since_last_rent`, etc.
- Encoded categorical features using Label Encoding / One-Hot Encoding.
- Scaled numerical features with `StandardScaler` or `MinMaxScaler`.

---

### 3. Exploratory Data Analysis (EDA)
- Analyzed rental trends using time-based plots.
- Visualized rental frequency by genre, day of week, and customer.
- Used heatmaps to understand feature correlations.
- Identified outliers and distribution patterns.

---

### 4. Feature Engineering
- Extracted temporal features: month, weekday, weekend.
- Aggregated customer behavior metrics: rental count, frequency.
- Transformed categorical features (e.g., genre, rating).
- Selected key features based on correlation and importance.

---

### 5. Model Building
- Split data into training and test sets (e.g., 80/20 split).
- Trained multiple machine learning models:
  - Logistic Regression
  - Random Forest Classifier
  - Decision Tree Classifier
  - XGBoost / LightGBM (optional)
- Tuned hyperparameters using `GridSearchCV`.

---

### 6. Model Evaluation
- Evaluated model performance using:
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion Matrix
  - ROC-AUC Score
- Compared performance across models to choose the best one.

---

### 7. Results Interpretation
- Analyzed feature importance for top-performing model.
- Visualized confusion matrix and ROC curve.
- Interpreted model predictions to generate business insights.

---



