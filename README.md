# 📊 Insurance Cost Prediction using Linear Regression (R)

![Language](https://img.shields.io/badge/Language-R-blue?logo=r)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Enabled-blueviolet)
![Linear Regression](https://img.shields.io/badge/Model-Linear%20Regression-success)
![Correlation](https://img.shields.io/badge/Analysis-Correlation-orange)
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


## 🛠️ Technologies Used
Language: R

Libraries: fastDummies, corrplot, caTools, car, psych

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

## 📊 Sample Model Equation

Charges = β0 + β1(Age) + β2(BMI) + β3(Smoker)

---

## 🚀 How to Run

1. Open RStudio
2. Load dataset - https://1drv.ms/x/c/f483042b9735aab9/IQA3oNBmDzLDR7kymQ3RNynmAf7x_EW11kbPp3jcfbsONKY?e=TF2T6n
3. Run - https://1drv.ms/f/c/f483042b9735aab9/IgDZhFOMSn1HSaf_3dLh5783Aa-rOC-K1n1jbiNVhaehIhs?e=9s0VFI
4. View outputs and plots

---
## Output images

## Correlation
✔ Shows strong positive relationship between smoker and charges
<img width="797" height="753" alt="Correlation" src="https://github.com/user-attachments/assets/1eb10d74-a0ba-40a5-b853-21ed9384ad09" />

## Pairs PLot
✔ Visualizes relationships and distributions between variables
<img width="842" height="811" alt="pairs plot" src="https://github.com/user-attachments/assets/906696dc-d34c-4d6c-b9d7-ea516888b815" />

## Model plot
✔ Residuals are fairly randomly distributed, indicating acceptable model fit
<img width="817" height="786" alt="model3" src="https://github.com/user-attachments/assets/cb24f3f3-70ee-48c4-86b7-e5f2f60d41a2" />

## Actual vs Predicted values plot
✔ Predicted values closely follow actual values, showing good model performance
<img width="833" height="802" alt="Actual vs predicted plot" src="https://github.com/user-attachments/assets/b283dd89-1964-4f0f-86ca-ce609037a0d3" />


## 👩‍💻 Author

Dhathri Narne
