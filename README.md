# 📊 Data Analysis with Python – Student Performance (Task 1)

## 🚀 Project Overview

This project was completed as part of my **Data Analysis Internship**. The objective is to analyze a real-world student dataset using Python and extract meaningful insights through data exploration, analysis, and visualization.

The project demonstrates fundamental data analysis workflow including:

* Data collection
* Data preprocessing
* Exploratory Data Analysis (EDA)
* Visualization
* Insight generation

---

## 📁 Dataset Information

* **Dataset Name:** Student Performance Dataset
* **File Used:** `student-mat.csv`
* **Source:** Kaggle / UCI Machine Learning Repository

### 📌 Dataset Description

The dataset contains academic and personal information of students, which helps in analyzing factors affecting their performance.

### 🔑 Key Features:

* `sex` → Gender of student
* `age` → Age of student
* `studytime` → Weekly study time
* `G1`, `G2`, `G3` → Grades (Final grade = G3)

---

## 🛠️ Technologies & Libraries Used

* **Python** → Programming language
* **Pandas** → Data manipulation and analysis
* **Matplotlib** → Data visualization
* **Google Colab** → Development environment

---

## ⚙️ Project Workflow

### 🔹 1. Data Loading

* Dataset uploaded into Google Colab
* Loaded using:

  ```python
  pd.read_csv('student-mat.csv', sep=';')
  ```

---

### 🔹 2. Data Exploration (EDA)

* Checked dataset structure using:

  * `df.shape`
  * `df.info()`
  * `df.describe()`
* Verified missing values:

  * `df.isnull().sum()`
* Observed data distribution and types

---

### 🔹 3. Data Cleaning

* Removed duplicate records (if any)
* Confirmed dataset contains no missing values
* Ensured proper formatting of columns

---

### 🔹 4. Data Analysis

Performed the following analysis:

* 📊 **Average Final Grade**

  ```python
  df['G3'].mean()
  ```

* 🏆 **Students scoring above 15**

  ```python
  len(df[df['G3'] > 15])
  ```

* 📈 **Correlation between study time and performance**

  ```python
  df[['studytime','G3']].corr()
  ```

* 👨‍🎓👩‍🎓 **Gender-based performance comparison**

  ```python
  df.groupby('sex')['G3'].mean()
  ```

---

### 🔹 5. Data Visualization

Created visual representations for better understanding:

* 📊 **Histogram**

  * Shows distribution of final grades (G3)

* 📈 **Scatter Plot**

  * Relationship between study time and performance

* 📉 **Bar Chart**

  * Comparison of performance based on gender

---

## 📊 Key Insights

* ✔ Average student score is approximately **10.41**
* ✔ Only **40 students** scored above 15 (high performers)
* ✔ Study time has a **very weak correlation** with performance
* ✔ Gender difference in performance is **minimal**

---

## 🎯 Conclusion

The analysis indicates that:

* Most students have **average academic performance**
* Increasing study time alone does not guarantee higher marks
* Other external factors may influence student performance
* Gender does not significantly impact academic results

---

## 🔗 Project Repository

👉 GitHub Link:
https://github.com/irfanashaik398/data-analysis-python-task1.git

---

## 🙌 Learning Outcomes

Through this project, I gained hands-on experience in:

* Data preprocessing and cleaning
* Exploratory Data Analysis (EDA)
* Data visualization techniques
* Drawing insights from real-world datasets

---

## 🔮 Future Improvements

* Apply machine learning models for prediction
* Analyze more features affecting performance
* Use advanced visualization libraries (Seaborn, Plotly)

---

## 📌 Acknowledgement

This project was completed as part of my internship to enhance my practical skills in data analysis using Python.

---
