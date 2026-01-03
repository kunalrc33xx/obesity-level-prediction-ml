# Predicting Obesity Levels: A Machine Learning Approach 🏥

![Status](https://img.shields.io/badge/Status-Completed-success)
![Tech](https://img.shields.io/badge/Stack-Python_|_Scikit--Learn_|_Pandas-blue)
![Focus](https://img.shields.io/badge/Focus-Healthcare_Analytics_|_Predictive_Modeling-green)

## 📄 Executive Summary
**The Problem:** Obesity is a global health crisis contributing to cardiovascular diseases and diabetes. Traditional BMI measurements often fail to account for lifestyle factors like diet, physical activity, and transportation habits.

**The Solution:** This project utilizes **Supervised Machine Learning (Random Forest)** and **Unsupervised Learning (K-Means Clustering)** to predict obesity levels based on diverse demographic and behavioral data from Mexico, Peru, and Colombia.

**Key Impact:**
* Successfully classified individuals into 7 distinct obesity levels (from "Insufficient Weight" to "Obesity Type III").
* Identified **Family History** and **Physical Activity** as the strongest predictors of obesity, validating the need for lifestyle-based interventions.
* Demonstrated that **Random Forest** outperformed other models in predictive accuracy for multi-class classification.

---

## 📊 Methodology & Approach

### 1. Data Preprocessing
* **Dataset:** 2,111 records covering 17 attributes (Age, Gender, Height, Weight, Smoking, Transportation, etc.).
* **Cleaning:** Handled categorical variables (One-Hot Encoding) and scaled numerical features to prepare for ML ingestion.

### 2. Exploratory Data Analysis (EDA)
We analyzed correlations between lifestyle habits and body mass.
* *Insight:* High caloric consumption (FAVC) and low physical activity (FAF) showed a strong positive correlation with higher obesity classes.
* *Transportation:* Users relying on **Automobiles** showed higher obesity rates compared to those using **Public Transportation** or **Walking**.

### 3. Machine Learning Models
We tested multiple algorithms to find the best fit:
* **Random Forest Classifier:** Selected as the champion model for its high accuracy and ability to handle non-linear relationships between lifestyle factors.
* **K-Means Clustering:** Used to segment the population into "Lifestyle Clusters," revealing natural groupings of individuals with similar risk profiles.

---

## 🚀 Key Results & Insights

| Feature | Impact on Prediction |
| :--- | :--- |
| **Family History** | 🔴 **High:** Strongest predictor of obesity levels. |
| **Physical Activity (FAF)** | 🟡 **Medium:** Negative correlation with obesity (more activity = lower risk). |
| **Transportation (MTRANS)** | 🟡 **Medium:** Sedentary transport (Car) links to higher weight classes. |
| **Smoking (SMOKE)** | 🟢 **Low:** Minimal influence on obesity classification in this dataset. |

**Conclusion:** Obesity is multifactorial. While genetics (family history) plays a major role, modifiable behavioral factors (activity, diet) are critical levers for public health intervention.

---

## 🛠 Tools Used
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn.
* **Environment:** Jupyter Notebook.

## 💻 How to Run This Project
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/obesity-level-prediction-ml.git](https://github.com/yourusername/obesity-level-prediction-ml.git)
