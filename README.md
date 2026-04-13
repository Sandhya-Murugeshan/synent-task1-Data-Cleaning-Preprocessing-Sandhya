# 🚢 synent-task1 Titanic Data Cleaning & Preprocessing

## Problem Statement
The objective of this task is to clean and preprocess the raw Titanic dataset.  
Real-world datasets often contain missing values, inconsistencies, and irrelevant features.  
The goal is to handle these issues and prepare a structured dataset that is ready for data analysis and machine learning.

---

## 📊 Dataset Details
- **Dataset:** Titanic Dataset  
- **Total Rows:** 891  
- **Total Columns:** 12  

### Features:
- PassengerId – Unique identifier  
- Survived – Survival status (0 = No, 1 = Yes)  
- Pclass – Ticket class  
- Name – Passenger name  
- Sex – Gender  
- Age – Age of passenger  
- SibSp – Number of siblings/spouses aboard  
- Parch – Number of parents/children aboard  
- Ticket – Ticket number  
- Fare – Ticket fare  
- Cabin – Cabin number  
- Embarked – Port of embarkation  

👉 These features include passenger details, travel information, ticket details, and family-related data.

---

## ⚙️ Approach

### 1. Data Exploration
- Used `info()` to understand data types and structure  
- Used `isnull().sum()` to identify missing values  

### 2. Handling Missing Values
- **Age:** Filled using median (robust to outliers)  
- **Embarked:** Filled using mode (categorical data)  
- **Cabin:** Dropped due to excessive missing values  

### 3. Data Cleaning
- Removed duplicate records to ensure data quality  

### 4. Data Type Conversion
- Converted **Survived** and **Pclass** into categorical data types  

### 5. Column Renaming
- PassengerId → Passenger_ID  
- Pclass → Ticket_Class  
- Sex → Gender  

### 6. Final Verification
- Checked again for missing values  
- Saved the cleaned dataset as `cleaned_titanic.csv`

---

## 📈 Results
- All missing values successfully handled  
- Unnecessary column (**Cabin**) removed  
- No duplicate records  
- Improved column readability  
- Correct data types assigned  

✅ The dataset is now clean, structured, and ready for:
- Exploratory Data Analysis (EDA)  
- Machine Learning models  

---

## 🚀 Conclusion
The preprocessing step ensures better data quality and reliability.  
This cleaned dataset provides a strong foundation for further analysis and predictive modeling.
