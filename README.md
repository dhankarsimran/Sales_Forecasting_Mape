# Walmart Sales Forecasting 

## 📌 Project Overview
This project focuses on forecasting **weekly sales for Walmart stores** using historical sales data.  
The goal is to support business decision-making such as inventory management, demand planning, and supply chain optimization.  

I built a machine learning model using **Python, Pandas, and XGBoost**, achieving a **MAPE of ~7%**, which improved accuracy by 15% compared to a baseline model.  

---

## 📂 Dataset
- Source: [Walmart Sales Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/walmart-dataset)  
- Contains weekly sales data for different Walmart stores and departments.  
- Features include: `Store`, `Dept`, `Date`, `Weekly_Sales`, `Holiday_Flag`.

---

## ⚙️ Approach
1. **Data Preprocessing**  
   - Converted `Date` column to datetime format.  
   - Aggregated sales by week.  
   - Handled missing values.  

2. **Feature Engineering**  
   - Extracted **Year, Month, Week** from date.  
   - Created lag features (`Lag_1`, `Lag_2`) and rolling averages (`Rolling_mean_4`).  

3. **Modeling**  
   - Used **XGBoost Regressor** for forecasting.  
   - Performed **GridSearchCV** for hyperparameter tuning (`max_depth`, `n_estimators`, `learning_rate`).  

4. **Evaluation Metrics**  
   - **MAPE (Mean Absolute Percentage Error): ~7%**  
   - **RMSE (Root Mean Squared Error)** also computed.  

---

## 📊 Results
- Achieved ~7% MAPE, significantly improving forecasting accuracy.  
- Feature engineering contributed to ~15% accuracy improvement.  
- Helps Walmart optimize **stock levels, promotions, and holiday planning**.  

---

## 🛠️ Tech Stack
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost  
- **Environment:** Jupyter Notebook
