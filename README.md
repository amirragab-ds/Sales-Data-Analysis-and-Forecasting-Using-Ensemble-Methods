# Sales Data Analysis and Forecasting Using Ensemble Methods

Sales forecasting is a common task performed by organizations to estimate expected revenue based on historical data. This is a challenging and interesting problem because there are many factors that can influence sales. For example, the weather, the season, and the day of the week can all impact sales. In this project, we will use historical sales data from a large retailer to predict future sales using ensemble methods.

We will also perform Data Analysis and Statistical Analysis to understand the data and its features and how they can influence the sales.

The data is available on [Kaggle](https://www.kaggle.com/competitions/rossmann-store-sales/overview).

## Project Steps

1. Data Collection and Cleaning
2. Exploratory Data Analysis
3. Data Analysis and Data Visualization
4. Sales Forecasting

## Key Findings

- Storetype 1 has a higher customer count than storetype 4, but storetype 4's customers spend more on average.
- Storetype 2 has the highest customer count but the lowest sales per customer. It also has the highest average sales. However, data for storetype 2 is limited.
- Storetype 2 shows the most variability in Sales and Customers, while storetype 4 shows the least.
  These findings were inferred from these KDE and Violin plots along with statistical analysis:
  
- Assortment type 2 has the highest average and median sales and customers but the lowest sales per customer. It also shows the most variability in Sales and Customers. However, data for assortment type 2 is also limited.
- Assortment type 3 outperforms assortment type 1 in terms of average and median sales, customers, and sales per customer. Assortment type 3 appears to be the most profitable, possibly due to its wider product range.
  The assortment type findings were inferred from these:
  
- The Promo feature increases the sales, customers, and sales per customer for all storetypes and assortment types by a significant margin.
- The Promo2 feature has an adverse effect on the sales, customers, and sales per customer for all storetypes and assortment types.
- The sales, customers, and sales per customer are highest in December and lowest in January.
  These finding were inferred from these Catplots:

## Models Used

- Random Forest Regressor
- XGBoost Regressor
  
## Evaluation Metrics
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)
- Symmetric Mean Absolute Percentage Error (SMAPE)
- R2 Score
  
## Model Performance

Both models perform extremely well, with the XGBoost regressor performing slightly better. This is because the XGBoost regressor is an iterative model, so it can learn from its mistakes and improve its predictions. It learnt that the Promo and Promo2 features are very important, while the random forest regressor didn't learn this. 

- The MAE of the random forest regressor is 1115, with a SMAPE of 16.12% and an R2 score of 0.70.
- The MAE of the XGBoost regressor is 1031, with a SMAPE of 15.12% and an R2 score of 0.73.

## Getting Started

1. Clone the repository
2. Install the necessary libraries (e.g., XGBoost, scikit-learn)
3. Run the Jupyter notebook

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
