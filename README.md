# 🏥 Medical Insurance Cost Prediction

## 📌 Project Overview
This project aims to build a **Linear Regression** model to predict medical insurance costs for individuals based on various demographic and lifestyle factors. By analyzing features such as age, BMI, smoking status, and more, the model provides accurate cost estimates, helping to understand the key drivers of healthcare expenses.

## 🚀 Key Highlights
- **Algorithm:** Linear Regression (Supervised Learning).
- **Core Skill:** Full Data Science Lifecycle (EDA -> Preprocessing -> Modeling -> Evaluation).
- **Insight:** Identified smoking status as the most significant factor affecting insurance charges.
- **Accuracy:** Validated model performance using robust metrics like RMSE and R² Score.

## 📊 Dataset Features
The dataset (`insurance.csv`) contains 1,338 records with the following attributes:
- **age:** Age of the primary beneficiary.
- **sex:** Gender (female, male).
- **bmi:** Body mass index (providing an understanding of body weights that are relatively high or low relative to height).
- **children:** Number of children covered by health insurance.
- **smoker:** Smoking status (yes, no).
- **region:** The beneficiary's residential area in the US (northeast, southeast, southwest, northwest).
- **charges:** Individual medical costs billed by health insurance (Target Variable).

## 🛠️ Methodology & Workflow

### 1. Exploratory Data Analysis (EDA)
- Analyzed data distribution using `head`, `info`, and `describe`.
- Visualized the target variable (`charges`) distribution.
- Investigated relationships between features using **Pairplots** and **Heatmaps** to identify correlations.

### 2. Data Preprocessing
- **Encoding:** Converted categorical variables (`sex`, `smoker`, `region`) into numerical format using `LabelEncoder` (or `get_dummies`) to make them machine-readable.
- **Splitting:** Divided the data into Training (70%) and Testing (30%) sets with a fixed `random_state=23` for reproducibility.

### 3. Model Building
- Utilized the `LinearRegression` model from `scikit-learn`.
- Trained the model on the training dataset using the `fit` method.

### 4. Evaluation & Testing
- Generated predictions on the test set.
- Visualized the model's performance:
    - **Scatter Plot:** Predicted vs. Actual values.
    - **Residual Histogram:** To analyze the distribution of errors.
- Calculated key evaluation metrics:
  - **MAE (Mean Absolute Error):** ~4044.99
  - **MSE (Mean Squared Error):** ~35,359,546
  - **RMSE (Root Mean Squared Error):** ~5946.39
  - **R² Score:** 0.73 (The model explains approx. 73% of the variance in costs).

## 📈 Key Findings
- **Smoking** has the strongest positive correlation with insurance charges.
- **Age** and **BMI** also show positive trends with costs, but to a lesser extent than smoking.

## 💻 Technologies Used
- **Python**
- **Libraries:**
  - `Pandas` & `NumPy` (Data Manipulation)
  - `Matplotlib` & `Seaborn` (Data Visualization)
  - `Scikit-Learn` (Modeling & Evaluation)

---
*Developed by Marwan Ali*
