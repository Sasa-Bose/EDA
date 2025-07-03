# 📱 Google Play Store Dataset – EDA & Feature Engineering

This project focuses on **Exploratory Data Analysis (EDA)** and **feature engineering** of the Google Play Store dataset. With over 2.5 million apps available, this dataset offers insights into app categories, user ratings, installs, and more.

---

## 🧩 Problem Statement

Today, mobile applications are an integral part of our daily lives. Our objective in this project is to:

- Identify the most popular app categories
- Find the app with the highest number of installs
- Determine which app has the largest size
- Perform data cleaning and feature extraction to prepare for modeling

---

## 📊 Dataset Overview

- 📁 **Rows**: 10,841  
- 📁 **Columns**: 13  
- 📥 **Source**: [Krishnaik on GitHub](https://raw.githubusercontent.com/krishnaik06/playstore-Dataset/main/googleplaystore.csv)

### Key Columns:

| Column Name        | Description                                    |
|--------------------|------------------------------------------------|
| `App`              | Name of the application                        |
| `Category`         | Category (e.g., FAMILY, GAME)                  |
| `Rating`           | User rating (0.0 to 5.0)                       |
| `Reviews`          | Number of user reviews                         |
| `Size`             | App size (in MB or KB)                         |
| `Installs`         | Number of installs                             |
| `Type`             | Free or Paid                                   |
| `Price`            | Price of the app (0 if Free)                   |
| `Content Rating`   | Appropriate target age group                   |
| `Genres`           | App genre (sub-category)                       |
| `Last Updated`     | Last updated date                              |
| `Current Ver`      | Current app version                            |
| `Android Ver`      | Minimum Android version required               |

---

## 🧹 Data Cleaning Steps

- Removed non-numeric and anomalous entries in `Reviews` and `Installs`
- Handled "Varies with device" and converted `Size` to numerical (in KB)
- Cleaned and transformed `Price` column to numeric
- Converted `Last Updated` to datetime and extracted:
  - Day
  - Month
  - Year
- Removed duplicates based on the `App` name
- Handled missing values using imputation or row removal

---

## 🔨 Feature Engineering

- ✅ Converted all numeric columns to proper datatypes
- ✅ Transformed categorical features using value counts and visual analysis
- ✅ Extracted installation patterns and app rating distributions
- ✅ Grouped apps by category for deeper insights

---

## 📈 EDA Highlights

### 🔝 Top Insights:

- **Most Popular Category**: `FAMILY` (18% of total apps)
- **Highest Installs**: `GAME` category (35+ billion installs)
- **Most Installed App**: `Subway Surfers`
- **Most Popular Communication App**: `Hangouts`
- **Highest Rated App (5.0)**: `CS & IT Interview Questions` (Family category)
- **271** apps have perfect 5.0 ratings

### 📊 Top Charts:

- Top 10 App Categories (by count)
- Top 10 Categories by Total Installs
- Top 5 Most Installed Apps in Each Popular Category
- Univariate analysis of numeric and categorical features

---

## 📁 Output

Cleaned and transformed dataset saved as:  
`google_play_store_data_cleaned.csv`

Final shape: **9,659 rows × 16 columns**

---

## 🧪 Libraries Used

```bash
pandas
numpy
matplotlib
seaborn
warnings
