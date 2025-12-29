# 📈 Time-Based TSLA Stock Price Prediction

This project predicts **Tesla (TSLA) next-day closing prices** using historical time-series data and machine learning regression models. Developed during a **Data Science & Machine Learning Internship at Brainybeam Info-Tech Pvt. Ltd. (Summer 2025)**.

---

## 🔍 Project Summary
- **Objective:** Predict next-day TSLA closing price using engineered time-series features  
- **Dataset:** TSLA historical stock data (June 2010 – Feb 2020, 2,416 trading days)  
- **Split Strategy:** 80/20 chronological split to prevent data leakage  
- **Models:** Linear Regression, Decision Tree, Random Forest (with GridSearchCV)

---

## 🧠 Feature Engineering
- **Lag Features:** `Close_lag1`, `Close_lag2`
- **Technical Indicators:** `MA7`, `MA21`
- **Target Variable:** Next-day `Close` price
- Removed NaN rows introduced by lag and rolling operations

---

## ⚙️ Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## 📊 Model Performance (Test Set)

| Model             | MAE  | RMSE | R²  |
|-------------------|------|------|-----|
| Linear Regression | 7.35 | 12.09| 0.97|
| Decision Tree     |15.89 |40.78 |0.68 |
| Random Forest     |15.72 |41.34 |0.67 |

🔹 **Linear Regression performed best**, indicating a largely linear relationship with engineered features.  
🔹 Complex models showed signs of overfitting on limited feature space.

---

## 📈 Key Insights
- Short-term moving average (**MA7**) and previous day close (**Close_lag1**) are the most influential predictors  
- Proper time-based validation is critical in financial forecasting  
- Simpler models can outperform complex ones when features are well-designed

---

---

## 👩‍💻 Author
**Mitali Sharma**  
Data Science & Machine Learning Intern



## 📁 Repository Structure
