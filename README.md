# Unilever-Global-Demand-Forecasting-Using-Machine-Learning
# Unilever Global Demand Forecasting Using Machine Learning

## Project Overview
This project focuses on building a machine learning based demand forecasting system for Unilever, a multinational FMCG company.  
The objective is to predict future product demand using historical sales, pricing, promotions, marketing, and supply chain data.

Accurate demand forecasting helps reduce stockouts, minimize overstocking, and improve inventory planning.

## Business Problem
Unilever operates across multiple regions with diverse product categories. Demand varies due to pricing, promotions, seasonality, marketing spend, and competition.

Traditional forecasting approaches do not capture these combined effects effectively.

## Objective
Predict future Units Sold for Unilever products across regions and product categories using machine learning models.

## Dataset Description
The dataset is synthetically generated to resemble real-world FMCG sales data.

### Dataset Details
- Rows: 500  
- Granularity: Daily  
- Regions: Asia, Europe, North America, Middle East, Africa  

### Key Features
- Date  
- Region  
- Country  
- Product Category  
- Brand  
- Product Name  
- Unit Price  
- Discount Percent  
- Units Sold (Target Variable)  
- Revenue  
- Promotion Type  
- Marketing Spend  
- Inventory Level  
- Supply Lead Time  
- Competitor Price  
- Weather Index  
- Holiday Flag  
- Online Sales Percent  
- Customer Satisfaction  

## Machine Learning Problem Type
- Supervised Learning  
- Regression  
- Time-aware demand forecasting  

## Target Variable
- Units_Sold

## Machine Learning Workflow
1. Load and inspect the dataset  
2. Data cleaning and preprocessing  
3. Feature engineering from date column  
4. Encode categorical variables  
5. Perform exploratory data analysis  
6. Split data using time-based logic  
7. Train regression models  
8. Evaluate model performance  
9. Analyze feature importance  
10. Interpret results for business use  

## Models Used
- Linear Regression  
- Random Forest Regressor  
- Gradient Boosting Regressor  

Deep learning models were intentionally excluded to maintain interpretability and simplicity.

## Evaluation Metrics
- Mean Absolute Error (MAE)  
- Root Mean Squared Error (RMSE)  
- R² Score  

## Results
- Tree-based models outperformed linear regression  
- Pricing, promotions, inventory level, and marketing spend were key demand drivers  
- The final model produced stable and realistic forecasts  

## Business Impact
This model helps Unilever:
- Improve inventory planning  
- Reduce supply chain inefficiencies  
- Align marketing campaigns with demand  
- Avoid stockouts and overstocking  
- Support data-driven decision making  

## Tools and Technologies
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Jupyter Notebook  

## Project Structure
Unilever-Demand-Forecasting  
│  
├── Unilever.ipynb  
├── unilever_global_demand_forecasting_dataset.csv  
└── README.md  

## How to Run the Project
1. Clone the repository  
2. Open Unilever.ipynb in Jupyter Notebook  
3. Install required libraries  
4. Run all cells sequentially  

## Future Improvements
- Add SARIMA or Prophet models  
- Integrate forecasts into Power BI or Tableau  
- Extend dataset for multi-year forecasting  
- Perform pricing and promotion scenario analysis  

## Author
Qamar Mehmood  
Machine Learning and Data Analytics Project
