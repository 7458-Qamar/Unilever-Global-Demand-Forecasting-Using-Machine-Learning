# Unilever Global Demand Forecasting Using Machine Learning
## Project Overview
This project focuses on building a **machine learning–based demand forecasting system** for a multinational FMCG company (Unilever).  
The goal is to accurately predict **product-level demand (Units Sold)** using historical sales, pricing, promotions, marketing, supply chain, and external factors.

The project demonstrates an **end-to-end ML workflow**, from data exploration and feature engineering to model training, evaluation, and business interpretation — without using deep learning.

## Business Problem
Unilever operates across multiple regions and product categories.  
Inaccurate demand forecasts can lead to:
- Stockouts and lost sales  
- Excess inventory and increased holding costs  
- Inefficient supply chain planning  

The objective is to **forecast future demand** to support better inventory, pricing, and marketing decisions.

## Dataset Description
- **Rows:** 1200  
- **Time Range:** 2022 – 2025 (daily data)  
- **Granularity:** Product-level daily sales  
- **Company:** Unilever (simulated but realistic FMCG data)

### Key Columns
- Date  
- Region, Country  
- Product Category, Brand, Product Name  
- Unit Price, Discount Percent  
- Units Sold (Target Variable)  
- Revenue  
- Marketing Spend  
- Inventory Level  
- Supply Lead Time  
- Competitor Price  
- Weather Index  
- Holiday Flag  
- Online Sales Percent  
- Customer Satisfaction  

## Machine Learning Objective
> Predict future **Units Sold** using historical sales data and influencing factors such as pricing, promotions, marketing, inventory, and seasonality.

This is a **supervised regression and time-series forecasting problem**.

## Exploratory Data Analysis (EDA)
The following analyses were performed:
- Distribution of Units Sold  
- Units Sold vs Revenue relationship  
- Daily demand trend over time  
- Average demand by region  
- Demand variation by product category  
- Impact of promotions and pricing  
- Marketing spend vs demand  
- Correlation heatmap of numeric variables  

These analyses helped identify key demand drivers and seasonality patterns.

## Feature Engineering
### Time-Based Features
- Year  
- Month  
- Week  
- Day of Week  
- Weekend Indicator  

### Lag and Rolling Features
- Lag 1 (previous day demand)  
- Lag 7 (weekly lag)  
- 7-day rolling mean of demand  

### Categorical Encoding
- Label encoding for:
  - Region  
  - Country  
  - Product Category  
  - Brand  
  - Product Name  
  - Promotion Type  

## Train–Test Strategy
- Data sorted chronologically  
- **80% training data**, **20% testing data**  
- Time-based split to prevent data leakage  

## Model Used
### Random Forest Regressor
Chosen because:
- Handles non-linear relationships well  
- Robust to multicollinearity  
- Provides feature importance for interpretability  

**Model Configuration:**
- Number of trees: 300  
- Maximum depth: 15  
- Minimum samples split: 5  

## Evaluation Metrics
The model was evaluated using:
- Mean Absolute Error (MAE)  
- Root Mean Squared Error (RMSE)  
- R² Score  

### Model Performance
- **MAE:** ~228 units  
- **RMSE:** ~286 units  
- **R²:** ~0.84  

This indicates strong predictive performance for demand forecasting.

## Feature Importance Insights
Top drivers of demand identified by the model:
1. Inventory Level  
2. Discount Percent  
3. Unit Price  
4. Marketing Spend  
5. Competitor Price  
6. Rolling Mean Demand  
7. Lagged Demand Features  

These insights align with real-world FMCG demand behavior.

## Results Visualization
- Feature importance bar chart  
- Actual vs predicted demand over time  

The predicted demand closely follows actual trends, validating the model’s effectiveness.

## Business Impact
This forecasting model can help Unilever:
- Optimize inventory planning  
- Reduce stockouts and overstocking  
- Align marketing spend with demand patterns  
- Improve revenue predictability  
- Enhance supply chain efficiency  

## Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

## Future Improvements
- Try Gradient Boosting or XGBoost  
- Add longer rolling windows (14, 30 days)  
- Perform region-specific forecasting  
- Build scenario simulations for pricing and promotions  

## Conclusion
This project demonstrates a **complete, production-style demand forecasting pipeline** using classical machine learning techniques.  
It combines strong data analysis, feature engineering, and model interpretability to deliver actionable business insights.

## Author
Qamar Mehmood  
Machine Learning and Data Analytics Project
