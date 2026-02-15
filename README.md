# Algerian-Forest-Fires-Dataset---Project-
The dataset has 244 records from Algeria’s Bejaia (northeast) and Sidi Bel-abbes (northwest) regions, with 122 instances each collected between June–September 2012. It includes 11 attributes plus one output class, categorizing 138 cases as fire and 106 as not fire

# 🌲 Algerian Forest Fires Prediction 

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Project Overview
This repository contains a machine learning project that predicts the occurrence and intensity of forest fires in two regions of Algeria: **Bejaia** and **Sidi Bel-abbes**. Using meteorological data, we employ various regression techniques to model the **Fire Weather Index (FWI)**.

## 🗂️ Dataset Information
The dataset includes 244 instances spanning from June 2012 to September 2012. 
**Key Features:**
* **Weather Data:** Temperature, Relative Humidity (RH), Wind Speed, Rain.
* **FWI System Components:** FFMC, DMC, DC, ISI, BUI.
* **Target:** FWI (Fire Weather Index).



## 🚀 Research & Methodology

### 1. Data Preprocessing
* **Cleaning:** Handled missing values and stripped inconsistent string formatting from column names.
* **Encoding:** Converted the 'Classes' feature (fire/not fire) into binary labels.
* **Regional Split:** Handled the two distinct datasets for Bejaia and Sidi Bel-abbes.

### 2. Exploratory Data Analysis (EDA)
* Performed correlation analysis to identify multi-collinearity.
* Visualized the impact of Temperature and Humidity on fire density using Seaborn.

### 3. Feature Selection & Regularization
To prevent overfitting and handle highly correlated features, we implemented:
* **Lasso Regression ($L1$):** Used for automated feature selection by shrinking coefficients of less important variables to zero.
* **Ridge Regression ($L2$):** Used to reduce model complexity and handle multicollinearity.
* **ElasticNet:** A hybrid of both $L1$ and $L2$ to find the optimal balance.



## 📊 Results & Performance
The models were evaluated using MAE, RMSE, and R² Score.

| Model | MAE | R² Score |
| :--- | :--- | :--- |
| Linear Regression | 0.56 | 0.98 |
| Lasso Regression | 1.13 | 0.94 |
| Ridge Regression | 0.56 | 0.98 |
| ElasticNet | 1.88 | 0.87 |

## 🛠️ Installation & Usage
1. Clone the repo:
   ```bash
   git clone [https://github.com/your-username/Algerian-Forest-Fire-Prediction.git](https://github.com/your-username/Algerian-Forest-Fire-Prediction.git)