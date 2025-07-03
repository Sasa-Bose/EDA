# 🍷 EDA with Red Wine Quality Dataset

## 📌 Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on the Red Wine Quality dataset from the UCI Machine Learning Repository. The dataset contains physicochemical properties of Portuguese "Vinho Verde" red wine, along with quality scores rated by wine tasters. The aim is to uncover patterns, relationships, and insights that affect wine quality.

---

## 🎯 Objectives

- Understand the structure and statistical properties of the dataset  
- Identify key factors influencing wine quality  
- Visualize the distribution of features and quality ratings  
- Examine correlations between chemical attributes and sensory scores  
- Handle duplicates and prepare clean data for further modeling

---

## 📁 Dataset Information

- **Source**: UCI Machine Learning Repository  
- **Wine Type**: Red  
- **Records**: 6,497 total entries (5,318 after removing duplicates)  
- **Features**: 11 input variables (numeric), 1 target variable (quality)

---

## 🧪 Attribute Description

**Input Features (Physicochemical Tests):**

1. Fixed Acidity  
2. Volatile Acidity  
3. Citric Acid  
4. Residual Sugar  
5. Chlorides  
6. Free Sulfur Dioxide  
7. Total Sulfur Dioxide  
8. Density  
9. pH  
10. Sulphates  
11. Alcohol

**Output Variable:**

- **Quality** — Integer score between 0 and 10 based on sensory evaluation

---

## 🧼 Data Cleaning Summary

- No missing values were found in the dataset  
- Duplicate rows were identified and removed  
- All columns were verified for accuracy and consistency  
- Dataset was clean and ready for visual and statistical exploration

---

## 📊 Key EDA Insights

- The dataset is **imbalanced**; majority of wines have quality ratings of 5 or 6  
- **Alcohol** content shows the strongest **positive correlation** with quality  
- **Volatile acidity** is negatively correlated with quality, suggesting higher levels reduce wine appeal  
- Other moderately influencing features include **sulphates**, **citric acid**, and **pH**  
- Attributes such as **density**, **chlorides**, and **sulfur dioxide** have less predictive value

---

## 📈 Visual Analysis Summary

- **Bar plots** show that most wines are rated between 5 and 6  
- **Histograms** illustrate distribution skewness of each chemical attribute  
- **Correlation heatmaps** reveal linear dependencies between features and target variable  
- **Box plots** demonstrate how alcohol and acidity vary with wine quality  
- **Scatter plots** provide insight into the relationship between variables like pH, alcohol, and quality

---

## 🧠 Conclusion

- **Higher alcohol content** often leads to better quality ratings  
- Wines with **balanced acidity and higher sulphate content** tend to score higher  
- The dataset provides a strong foundation for predictive modeling  
- The imbalance in quality ratings should be accounted for in future machine learning applications

---

## 🚀 Future Scope

- Apply classification and regression models to predict wine quality  
- Use feature selection techniques to identify the most impactful variables  
- Address class imbalance using resampling techniques  
- Extend analysis to the white wine dataset or combine both for comparative insights  
- Develop an interactive dashboard to visualize and predict wine quality

---

## 📎 License

This dataset is publicly available from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wine+Quality) and is intended for educational and research use only.
