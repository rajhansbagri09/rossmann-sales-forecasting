# Rossmann Store Sales Forecasting 📊

This project was completed as part of the **Machine Learning Internship at Future Interns**. The objective was to forecast daily sales for Rossmann drug stores using historical data and advanced machine learning models.

---

## 🔍 Problem Statement

Rossmann operates over 3,000 drug stores across Europe. Sales are influenced by factors like promotions, holidays, competition, and more. The goal was to **predict store sales** for the test period using the provided training dataset.

---

## 📁 Dataset

- Provided by: Kaggle (Rossmann Store Sales)
- Files used:
  - `train.csv`: Historical sales data
  - `test.csv`: Test data without target
  - `store.csv`: Store-specific additional info

---

## 🔧 Project Workflow

1. **Data Preprocessing**
   - Merged `train` and `store` datasets
   - Handled missing values
   - Extracted date features (Year, Month, Day, WeekOfYear, IsWeekend)

2. **Feature Engineering**
   - Added categorical encodings (StoreType, Assortment)
   - Removed stores that were closed (Open=0)

3. **Modeling**
   - Applied **XGBoost Regressor**
   - Used `log1p(Sales)` to handle skewness
   - Evaluated using RMSE

4. **Predictions**
   - Generated predictions on the test set
   - Saved as `sales_predictions.csv`

---

## 📊 Evaluation

- **Model Used:** XGBoost
- **Metric:** RMSE (Root Mean Squared Error)
- **Final Output:** `sales_predictions.csv`

---

## 📈 Next Steps

- Create Power BI dashboards using the predictions
- Explore feature importance & business insights

---

## 🧑‍💻 Author

- **Rajhans Bagri**
- B.Tech Artificial Intelligence, Gautam Buddha University
- [GitHub Profile](https://github.com/rajhansbagri09)

