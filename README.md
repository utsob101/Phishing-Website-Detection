# Phishing-Website-Detection
# 🎣 Phishing Website Detection using Data Mining

This project is a **Data Mining & Machine Learning** initiative designed to detect phishing (malicious) websites based on URL features. The project covers the complete pipeline from **Exploratory Data Analysis (EDA)** to **Data Preprocessing**, preparing the dataset for Classification, Clustering, and Regression tasks.

## 📌 Project Overview
Phishing attacks are one of the most common security threats today. This project analyzes a dataset of website URLs to identify patterns that distinguish legitimate sites from phishing ones.

**Key Objectives:**
- Load and inspect the dataset.
- Perform **EDA** (Exploratory Data Analysis) to understand data distribution and correlations.
- **Preprocess** the data (cleaning, handling duplicates, and splitting) for model training.

## 📂 Dataset
The project uses the **Phishing Websites Dataset** (available on Kaggle/UCI Machine Learning Repository).
- **Rows:** ~11,000 website entries.
- **Columns:** 30+ features (e.g., `URL_Length`, `having_IP_Address`, `HTTPS_token`).
- **Target Variable:** `Result`
  - `1`: Phishing Website
  - `-1`: Legitimate Website

## 🛠️ Technologies Used
- **Language:** Python
- **Environment:** Google Colab
- **Libraries:**
  - `pandas` & `numpy` (Data Manipulation)
  - `matplotlib` & `seaborn` (Data Visualization)
  - `scikit-learn` (Preprocessing & Model Selection)

## 📊 Features of the Notebook

### 1. Data Loading
- Mounts Google Drive to access the dataset directly.
- Handles file not found errors gracefully.

### 2. Exploratory Data Analysis (EDA)
- **Data Info:** Checks data types and structure.
- **Class Balance:** Visualizes the ratio of Phishing vs. Legitimate sites using Countplots.
- **Null & Duplicate Checks:** Ensures data quality.
- **Correlation Heatmap:** Visualizes relationships between different features.

### 3. Data Preprocessing
- **Cleaning:** Removes duplicate rows and unnecessary columns (e.g., `id`).
- **Feature Separation:** Splits the dataset into Features (`X`) and Target (`y`).
- **Train-Test Split:** Divides data into 80% Training and 20% Testing sets.

## 🚀 How to Run this Project

### Option 1: Using Google Colab (Recommended)
1. Upload the `dataset.csv` file to your Google Drive in a folder named `Phishing website detection`.
2. Open the `.ipynb` file in Google Colab.
3. Mount your drive when prompted.
4. Run all cells to see the EDA and Preprocessing outputs.

### Option 2: Local Machine
1. Download the repository.
2. Change the file path in the code:
   ```python
   # Change this line
   filename = 'path/to/your/dataset.csv'
