# 📊 Housing Price Prediction Project 🏠

## Overview
This project predicts housing rental prices based on various features such as the number of bedrooms, square footage, and location. It processes raw Craigslist data, cleans it, and builds machine learning models to make predictions. The models tested include **Linear Regression** and **Random Forest Regressor**.

To check the full presentation + dashboard link refer to the file vancouver_rentals_presentation.pdf
---

## 🚀 Getting Started

### Prerequisites
To run this project, you'll need the following Python libraries:
- pandas 🐼
- numpy 🔢
- matplotlib 📈
- scikit-learn 🧠

You can install the required packages using:

## 📊 Data

The dataset `craiglist_scrapping.csv` contains information about rental listings from Craigslist. The key features are:

- **postbedrooms**: Number of bedrooms 🛏️
- **postsqft**: Square footage 📏
- **Price**: Rental price 💵
- **location**: Location of the property 🌍

---

## 🧹 Data Cleaning & Preprocessing

- **Dropped Irrelevant Columns**: Removed the `Image`, `Title_URL`, `Label`, and `meta` columns as they didn't contribute to our analysis.
- **Handling Missing Values**: Dropped rows with missing values as they didn’t represent a significant portion of the data.
- **Meta Column Cleanup**: Extracted important features like location, bedrooms, and square footage from the `meta` column.
- **Standardization**: Used `StandardScaler` to scale numerical features like `postbedrooms` and `postsqft`.

---

## 🖼️ Exploratory Data Analysis (EDA)

- **Scatter Plots**: Plotted the relationship between the number of bedrooms, square footage, and price.
- **Histograms**: Analyzed the distribution of rental prices, square footage, and bedroom count.
- **Location Analysis**: Created a scatter plot to compare rental prices across different locations, focusing on 1-bedroom listings.

---

## 🔄 Model Building

### Encoding Categorical Features
Used **Label Encoding** to convert the `location` column into numerical values, as machine learning models require numeric input.

### Feature Scaling
Applied **StandardScaler** to scale the `postbedrooms` and `postsqft` features so that they contribute equally to the model.

---

## 🤖 Machine Learning Models

### 1. **Linear Regression**:
A simple regression model that predicts rental prices based on the features.  
Evaluated using **Mean Squared Error (MSE)** and **R-squared**.

### 2. **Random Forest Regressor**:
A more advanced model that uses multiple decision trees to predict rental prices. This model typically provides better accuracy.  
Evaluated using the same metrics: **MSE** and **R-squared**.

---

## ⚡ Model Evaluation

The **Random Forest Regressor** performed better than **Linear Regression** based on the evaluation metrics:

- **MSE (Random Forest)**: (insert value)
- **R² (Random Forest)**: (insert value)

### Example Predictions:
Predicted rental prices for new data points:

- Vancouver, 2-bedroom, 800 sqft: $X
- Burnaby, 2-bedroom, 800 sqft: $Y
- Coquitlam, 2-bedroom, 800 sqft: $Z

---

## 📅 Future Work

- Explore other machine learning models for better predictions.
- Fine-tune the Random Forest model by adjusting hyperparameters.
- Investigate feature engineering to include additional predictors like listing age or amenities.

---

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

---
## 🙏 Acknowledgments

A big thank you to Teacher Derrick Park for his guidance throughout the career, and to my classmates for being part of this journey.

