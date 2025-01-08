# Walmart Sales Analysis 📊🛒

## Project Overview
This project focuses on analyzing Walmart sales data to uncover patterns, trends, and insights that can drive strategic business decisions. The project merges multiple datasets, performs exploratory data analysis (EDA), and implements machine learning techniques to predict future sales and understand contributing factors.

---

## Key Features
1. **Data Integration**:
   - Merges datasets including store details, weekly sales, and external features such as temperature and fuel price.
   - Final dataset contains detailed information for 45 stores and 81 departments.

2. **Exploratory Data Analysis (EDA)**:
   - Examines relationships between features such as markdown values, sales, and holiday effects.
   - Visualizes sales trends, department performance, and store-specific patterns.

3. **Time Series Analysis**:
   - Leverages techniques like ARIMA and Exponential Smoothing to forecast sales.
   - Decomposes time series data to identify seasonal, trend, and residual components.

4. **Machine Learning Models**:
   - Implements models like Random Forest and Linear Regression for sales prediction.
   - Evaluates performance using metrics like Mean Squared Error (MSE) and Mean Absolute Error (MAE).

---

## Datasets
The project utilizes three key datasets:
1. **`stores.csv`**: Contains store type and size information.
2. **`train.csv`**: Weekly sales data with department, store, and date details.
3. **`features.csv`**: External features including fuel price, CPI, unemployment rates, and markdowns.

**Data Size**: Final merged dataset contains 421,570 rows and 16 columns.

---

## Methodology
1. **Data Cleaning**:
   - Removed duplicate columns and handled missing values.
   - Renamed columns for better clarity and consistency.

2. **Data Analysis**:
   - Generated pivot tables for department-wise and store-wise sales.
   - Visualized correlations and trends using matplotlib and seaborn.

3. **Time Series Modeling**:
   - Decomposed sales data using `seasonal_decompose`.
   - Implemented ARIMA and Exponential Smoothing for forecasting.

4. **Machine Learning**:
   - Applied Random Forest Regressor and Linear Regression to predict sales.
   - Used cross-validation for robust model evaluation.

---

## Results
- **Sales Trends**:
  - Significant impact of holidays and markdowns on weekly sales.
  - Seasonal patterns observed in multiple departments and stores.

- **Best Model**:
  - Random Forest Regressor performed well with low error metrics.
  - ARIMA model provided accurate time-series forecasts for sales.

---

## Technologies Used
- **Programming Languages**: Python
- **Libraries**:
  - Data Analysis: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`
  - Time Series: `statsmodels`, `pmdarima`
  - Machine Learning: `scikit-learn`
- **Environment**: Jupyter Notebook

---

## Installation and Usage
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/walmart-sales-analysis.git
   cd walmart-sales-analysis
2. **Install Dependencies:**
   ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn statsmodels pmdarima

3. Run the Notebook: Open and execute walmart_sales_analysis.ipynb in Jupyter Notebook to see the analysis and results.

Future Enhancements
Real-Time Forecasting: Implement real-time data pipelines for live sales predictions.
Advanced Modeling: Explore deep learning models like LSTMs for time-series forecasting.
Dashboard Development: Create interactive dashboards for visualization and reporting.
