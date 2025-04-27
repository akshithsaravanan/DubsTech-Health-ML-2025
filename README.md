# 🏥 DubsTech Health ML 2025  
**Predicting Hospital Discharge Costs (NY SPARCS Dataset 2009–2024)**

---

## 📋 Project Overview

In this project, our team — **Husky Hackers** — set out to predict the **mean cost** of a hospital discharge based on key factors:

- **Hospital Name**
- **APR DRG Code**
- **Severity of Illness**
- **Year**
- **Mean/Median Charges**
- **Mean/Median Costs**

🎯 By accurately predicting healthcare discharge costs, we aim to help hospitals:
- Plan better budgets
- Improve resource allocation
- Enhance affordability

---

## 📈 Dataset

We utilized a **cleaned version** of the NY SPARCS public dataset, containing **over 1 million rows** across **2009–2024**.

Due to GitHub file size limits, download the cleaned dataset from here:

👉 [**Download Cleaned SPARCS Dataset (CSV)**](https://drive.google.com/file/d/1cdyYMSqdEzTD2ZLJZqAXwYsws1DDFN4g/view?usp=sharing)

**Key Features:**
- Facility Name
- APR DRG Code
- Severity of Illness
- Year
- Discharges
- Mean/Median Charges
- Mean/Median Costs

---

## 🛠️ Methodology

- **Initial Data Cleaning**:
  - Cleaned column names
  - Removed symbols like `$` and `,` from cost fields
  - Handled missing values

- **Exploratory Data Analysis (EDA)**:
  - Visualized distribution of costs
  - Analyzed top hospitals and cost trends by severity of illness
  - Removed extreme outliers (mean cost > $25,000)

- **Model Building**:
  - Tried **Linear Regression** and **Polynomial Regression** — but achieved low accuracy
  - Final Model:  
    **CatBoostRegressor** (1200 iterations, depth=10, learning_rate=0.03)

- **Train/Test Split**:
  - 80% data for training
  - 20% data for testing

---

## 🎯 Model Results

| Metric                         | Value    |
|:------------------------------- |:---------|
| Final Train Score               | 0.9377   |
| Final Test Score                | 0.9341   |
| Margin of Error (95% Confidence Interval) | ±0.0011 |

📈 **Predicted Average Mean Cost for 2025**: **$11,106.70**

---

## 📊 Visualizations Included

- Distribution of Mean Cost (after removing extreme outliers)
- Top 15 Hospitals by Average Mean Cost
- Boxplot of Mean Cost by Severity of Illness
- Line Plot showing Trend of Average Mean Cost (2015–2025)

---

## 💻 Team

**Team Name**: **Husky Hackers** 🚀

**Team Members**:
- Akshith Saravanan
- Aditya Kumar
- Sumedha Komawar
- Manvith Kothapalli 
- Saurav Mukherjee 

---

## 🏆 Final Thoughts

This project gave us deep insights into the challenges of **real-world hospital cost prediction**.  
We successfully achieved **over 93% test accuracy** with a **very low margin of error**, making our model **reliable** and **practically useful** for healthcare budgeting and strategic planning.

---

# Thank you for checking out our project!

