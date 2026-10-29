# Time-Series Sales Forecasting

**Internship:** CODTECH Data Science Internship  
**Intern ID:** CITS8940  
**Duration:** 6 weeks  
**Project:** 4 – Time-Series Sales Forecasting

## Project Overview
This project analyzes historical monthly retail sales data and uses time-series forecasting to predict future sales. It compares a simple baseline forecast with Holt's trend method to evaluate forecasting performance.

## Dataset
- **Source:** Federal Reserve Economic Data (FRED)
- **Series:** Retail Trade Sales (MRTSSM44000USS)
- **Frequency:** Monthly
- **Period:** January 1992 – August 2026
- **Test period:** September 2025 – August 2026

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Jupyter Notebook

## Project Workflow
1. Loaded and inspected the retail sales dataset.
2. Prepared and sorted the date and sales columns.
3. Explored historical sales trends and monthly changes.
4. Split the data into training and testing periods.
5. Built a baseline forecast using the last training observation.
6. Built a Holt trend forecasting model.
7. Evaluated both models using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
8. Visualized actual sales against both forecasts.

## Model Evaluation

| Model | MAE | RMSE |
|---|---:|---:|
| Baseline | 14672.75 | 19076.62 |
| Holt Trend | 8346.25 | 11122.90 |

Holt's trend model achieved lower MAE and RMSE than the baseline on the 12-month test period, indicating better forecasting performance on this dataset.

## Project Outputs
- `notebook/Time_Series_Sales_Forecasting.ipynb`
- `visualizations/actual_vs_forecast.png`
- `visualizations/model_comparison.csv`
- `visualizations/forecast_results.csv`

## Conclusion
The analysis shows a long-term increase in retail sales. The Holt trend model captured the upward trend more effectively than the constant baseline forecast during the selected test period. Forecasts remain estimates and may not capture every sudden change in sales.

## Disclaimer
This project is for educational and internship purposes. Forecasts are not guarantees of future sales.
