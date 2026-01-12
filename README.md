## 🏏Cricket Runs Prediction using Linear Regression

This project is a machine learning implementation designed to predict the Runs scored by a batsman based on various match statistics. It utilizes Python's Scikit-Learn library to perform data preprocessing and linear modeling.

---
## 📌 Project Overview

The goal of this project is to build a regression model that can accurately estimate runs scored by analyzing independent variables like balls faced, strike rate, and dot ball percentage.

---
## 📊 Dataset Features
The dataset includes individual match performance metrics:
Independent Variables (X):
Balls: Total balls faced.
Outs: Number of times out (used to derive Not Out status).
SR: Strike Rate.
Dot %: Percentage of balls with no runs scored.
Not_Out: A binary feature derived from the 'Outs' column.
Runs_per_Ball: An engineered feature representing efficiency.
Target Variable (y): * Runs: The actual runs scored in a match.

---
## 🛠️ Technology Stack
Language: Python
Libraries: * Pandas: For data manipulation and analysis.
Scikit-Learn: For scaling, splitting data, and building the regression model.
Openpyxl: To handle Excel file input.

### 🚀 Step-by-Step Implementation
Data Cleaning: Dropped unnecessary columns like Match, Innings, HS, and Avg to focus on predictive features.
Feature Engineering: Created new features such as Not_Out (using a lambda function) and Runs_per_Ball to improve model insights.
Data Scaling: Applied StandardScaler to normalize the feature set, ensuring that variables with different scales (like SR vs. Dot %) don't bias the model.
Model Training: Split the data into 80% training and 20% testing sets using train_test_split.
Algorithm: Implemented Linear Regression to fit the training data.

---
## 📈 Performance Metrics
**The model was evaluated using standard regression metrics:**
**R2 Score: ~0.955 (Indicates a high level of accuracy and fit).**
**Mean Squared Error (MSE): ~73.73**
