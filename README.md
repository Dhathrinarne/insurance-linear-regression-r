# 📊 Insurance Cost Prediction using Linear Regression (R)

## 🔍 Project Overview

This project builds a **Linear Regression model in R** to predict medical insurance charges based on factors like age, BMI, smoking status, and gender.

---

## 📁 Dataset

* Insurance dataset containing:

  * Age
  * BMI
  * Smoker status
  * Gender
  * Charges (target variable)

---

## ⚙️ Steps Performed

### 1. Data Preprocessing

* Removed missing values using `na.omit()`
* Converted categorical variables to factors
* Created dummy variables for region
* Label encoding:

  * Smoker (Yes/No → 1/0)
  * Sex (Male/Female → 1/0)

---

### 2. Exploratory Data Analysis

* Summary statistics
* Correlation matrix using `corrplot`
* Pair plots using `pairs.panels`

---

### 3. Model Building (Forward Regression)

* Model 1: Charges ~ Age
* Model 2: Charges ~ Age + BMI
* Model 3: Charges ~ Age + BMI + Smoker ✅ (Best Model)
* Model 4: Charges ~ Age + BMI + Smoker + Sex

---

### 4. Model Evaluation

* Used:

  * Adjusted R²
  * P-values
  * VIF (Variance Inflation Factor)
* Checked:

  * Multicollinearity
  * Heteroscedasticity

---

### 5. Train-Test Split

* 70% Training
* 30% Testing
* Used `caTools` package

---

### 6. Prediction

* Predicted insurance charges on test dataset
* Compared Actual vs Predicted values

---

## 📈 Key Insights

* Smoking status has a **major impact** on insurance charges
* Age and BMI are significant predictors
* Adding smoker variable improved model accuracy significantly

---

## 🛠️ Technologies Used
* R
* Packages:
  * fastDummies
  * corrplot
  * caTools
  * car
  * psych

---

## 📊 Sample Model Equation

Charges = β0 + β1(Age) + β2(BMI) + β3(Smoker)

---

## 🚀 How to Run

1. Open RStudio
2. Load dataset - https://1drv.ms/x/c/f483042b9735aab9/IQA3oNBmDzLDR7kymQ3RNynmAf7x_EW11kbPp3jcfbsONKY?e=TF2T6n
3. Run - https://1drv.ms/f/c/f483042b9735aab9/IgDZhFOMSn1HSaf_3dLh5783Aa-rOC-K1n1jbiNVhaehIhs?e=9s0VFI
4. View outputs and plots

---

## 👩‍💻 Author

Dhathri Narne
