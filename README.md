
# Time-Series-Forecasting-using-SARIMA-MODEL

Sales forecasting is a crucial business exercise. Accurate sales forecasts allow business leaders to make smarter decisions about things like goal-setting, budgeting, hiring, and other things that affect cash flow.

Meanwhile, an inaccurate sales forecast leaves sales managers guessing at whether they’ll actually hit quota. As a result, they may not be aware of any problems in the sales pipeline in time to fix them.

A sales forecast is a prediction of future sales revenue. Sales forecasts are usually based on historical data, industry trends, and the status of the current sales pipeline. Businesses use the sales forecast to estimate weekly, monthly, quarterly, and annual sales totals.




## Business Problem:
One of the most important tasks for any retail store company is to analyze the performance of its stores. The main challenge faced by any retail store is predicting in advance the sales and inventory required at each store to avoid over-stocking and under-stocking. This helps the business to provide the best customer experience and avoid getting into losses, thus ensuring the store is sustainable for operation.
## Methodology
SARIMA stands for Seasonal Autoregressive Integrated Moving Averages. It is a simple but quite powerful model to use for analyzing time series with seasonality.

I will load a sample dataset to examine its trend and seasonality, then I will use a grid search algorithm to find the best-fit SARIMA model, and finally I will use the best-fit model to train with the historical data and predict the future.
## Metric Of Success
- Evaluation Metrics

There are two popular metrics used in measuring the performance of regression (continuous variable) models i.e `MAE & RMSE`.

`Mean Absolute Error (MAE):` It is the average of the absolute difference between the predicted values and observed values.

`Root Mean Square Error (RMSE):` It is the square root of the average of squared differences between the predicted values and observed values.

`MAE` is easier to understand and interpret but `RMSE` works well in situations where large errors are undesirable. This is because the errors are squared before they are averaged, thus penalizing large errors. In our case, `RMSE` suits well because we want to predict the sales with minimum error (i.e penalize high errors) so that inventory can be managed properly.

The `lower` the `RMSE`, the better a given model is able to “fit” a dataset. However, the range of the dataset you’re working with is important in determining whether or not a given RMSE value is “low” or not.