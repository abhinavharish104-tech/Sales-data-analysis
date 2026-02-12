# Week 2 Mini Project  
## Student Performance Prediction using Linear Regression

---

## 📌 Project Overview

This mini project focuses on predicting student GPA based on SAT scores using Simple Linear Regression. The objective was to build a regression model, evaluate its performance, visualize the results, and interpret the findings.

---

## 📊 Dataset Description

The dataset contains two variables:

- **SAT** (Independent Variable)
- **GPA** (Dependent Variable)

Total Observations: 84 students

---

## ⚙️ Methodology

### 1️⃣ Data Loading
- Imported dataset using pandas
- Checked first and last rows
- Generated summary statistics

### 2️⃣ Data Splitting
- Divided dataset into training and testing sets

### 3️⃣ Model Training
- Applied **Simple Linear Regression**
- Calculated:
  - Correlation
  - Slope (b1)
  - Intercept (b0)

Regression Equation:

GPA = 0.2750 + 0.0017 × SAT

### 4️⃣ Model Evaluation

- R-squared (R²) ≈ 0.406

This indicates that approximately 40.6% of the variation in GPA is explained by SAT scores.

---

## 📈 Visualizations

### 🔹 Scatter Plot with Regression Line
- Shows relationship between SAT and GPA
- Displays fitted regression line

---

## 📊 Results

- Positive correlation between SAT and GPA
- As SAT score increases, GPA tends to increase
- Model shows moderate predictive power (R² ≈ 0.406)

---

## 🧠 Interpretation

The regression model suggests a positive linear relationship between SAT scores and GPA. However, since R² is around 0.40, SAT alone does not fully explain GPA variations. Other factors such as study habits, school environment, and extracurricular involvement may also influence GPA.

The model is useful for basic prediction but can be improved by adding more features.

---

## ✅ Conclusion

This project demonstrates:

- Implementation of Simple Linear Regression
- Model evaluation using R² score
- Data visualization with regression line
- Interpretation of predictive results

It provides a foundational understanding of regression modeling in machine learning.
