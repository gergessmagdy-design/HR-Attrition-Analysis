# HR Attrition Analysis

## 📖 Introduction
Employee attrition is a major challenge for organizations as it impacts productivity, increases hiring costs, and affects team stability. Understanding the factors behind employee turnover is key to improving employee satisfaction and retention.

In this project, we analyze the **IBM HR Analytics Employee Attrition dataset** to explore the key drivers of attrition. The analysis examines employee characteristics such as age, income, overtime, and job role, aiming to identify patterns and relationships that influence turnover.

The project covers data exploration, cleaning, **exploratory data analysis (EDA)**, and **machine learning modeling** to predict the likelihood of employee attrition. The insights generated can help HR departments make **data-driven decisions** to enhance employee retention and organizational performance.

---

## 🎯 Project Objectives
- Analyze employee attrition patterns  
- Identify factors influencing employee turnover  
- Explore relationships between attrition and employee attributes  
- Build a machine learning model to predict employee attrition  

---

## 🛠️ Tools & Libraries
- Python 3.x  
- `pandas`, `numpy` for data manipulation  
- `matplotlib`, `seaborn` for visualization  
- `sklearn` for preprocessing and evaluation  
- `xgboost` for predictive modeling  
- `imblearn` for handling class imbalance (SMOTE)

---

## 📂 Dataset
- **Source:** IBM HR Analytics Employee Attrition  
- **Rows:** 1470  
- **Columns:** 35  
- **Description:** Includes employee demographic, job-related, and performance features such as Age, JobRole, Department, OverTime, MonthlyIncome, Attrition, etc.  

---

## 🔍 Data Overview & Cleaning
- No missing values in the dataset.  
- Dropped irrelevant columns: `EmployeeNumber`, `Over18`, `StandardHours`, `EmployeeCount`.  
- Converted categorical variables like `Attrition` and `OverTime` to numeric.  
- Ensured all columns are ready for analysis and modeling.  

---

## 📊 Exploratory Data Analysis (EDA)
Key observations from the data:  
1. **Attrition Rate is Low** – Most employees stayed; a smaller proportion left.  
2. **Younger employees leave more** – Attrition is higher among younger staff.  
3. **Lower Monthly Income increases attrition** – Salary is a significant factor.  
4. **Overtime increases attrition risk** – Employees working overtime are more likely to leave.  
5. **Age above 40 shows stability** – Attrition decreases with experience.  
6. **Work-life balance matters** – High correlation between overtime and attrition.  

---

## 📈 Correlation & Feature Importance
- Top numerical features correlated with attrition: `YearsInCurrentRole`, `MonthlyIncome`, `Age`, `YearsWithCurrManager`, `JobLevel`.  
- **XGBoost feature importance highlights:**
  1. Stock Option Level  
  2. Marital Status (Married / Single)  
  3. Department (Sales, R&D)  
  4. Job Level  
  5. Job Satisfaction  
  6. Education Field  

These features significantly influence employee attrition predictions.

---

## 🤖 Machine Learning Model
- **Model Used:** XGBoost Classifier  
- **Class Imbalance:** Handled using **SMOTE**  
- **Performance Metrics (after SMOTE):**
  - Accuracy: 84%  
  - Precision, Recall, F1-score show better prediction for majority class; minority class prediction (Attrition=1) can be improved further  

**Confusion Matrix Example:**
[[227 20]
[ 27 20]]


---

## 💡 Key Insights & Business Recommendations
1. **Financial Incentives** – Improve stock options and salary packages to retain employees.  
2. **Workload Management** – Monitor overtime, especially in high-pressure departments.  
3. **Employee Engagement** – Enhance job satisfaction through engagement programs.  
4. **Early Career Focus** – Implement retention strategies for younger employees.  
5. **Career Development** – Offer training and growth opportunities to reduce turnover.  

---

## ⚡ Conclusion
This analysis provides actionable insights into employee attrition patterns. HR departments can use these insights to make data-driven decisions that improve retention, employee satisfaction, and overall organizational performance.