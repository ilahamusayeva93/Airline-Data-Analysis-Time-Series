### Airline Data Analysis (Time Series)

#### Overview

This R Markdown document is designed for analyzing time series data related to international airline passengers. The analysis involves data exploration, preprocessing, and modeling using three different models: `arima_boost`, `prophet`, and `ets`. The script compares the RMSE scores on the test set, selects the model with the lowest RMSE, and makes forecasts. Finally, it visualizes both past data and forecasted values on a single plot.

#### Script Details

##### 1. Data Exploration and Preparing for Modelling

- **Libraries:** The script begins by loading necessary R libraries, including `tidyverse`, `data.table`, `lubridate`, `skimr`, `timetk`, `highcharter`, `h2o`, `tidymodels`, and `modeltime`.

- **Dataset Loading:** The dataset "airpassengers.csv" is loaded using the `read.csv` function.

- **Data Exploration:** The structure of the data is displayed, and columns are renamed for better readability.

- **Preprocessing Date Column:** The date column is preprocessed to ensure consistency in formatting.

- **Visualizing Time Series Data:** The time series data is visualized using the `plot_time_series` function.

- **Time Series Splitting:** The data is split into training and testing sets using `initial_time_split`.

##### 2. Modelling

- **arima_boost Model:** The first model (`arima_boost`) is trained using the `arima_boost` function with appropriate parameters.

- **prophet Model:** The second model (`prophet`) is trained using the `prophet_reg` function.

- **ets Model:** The third model (`ets`) is trained using the `exp_smoothing` function.

##### 3. Model Evaluation

- **RMSE Scores:** RMSE scores are calculated for each model on the test set.

- **Model Selection:** The model with the lowest RMSE score is selected.

##### 4. Forecasting and Visualization

- **Making Forecasts:** Forecasts are made using the selected model.

- **Plotting Past Data and Forecast Values:** The script generates a plot with past data and forecasted values, using different colors for clarity.

#### How to Use

1. Ensure you have R installed along with the required libraries listed at the beginning of the script.

2. Place the "airpassengers.csv" dataset in the same directory as the R Markdown document.

3. Run the script in an R environment, considering any specific package dependencies.

#### Author

- **Author:** Ilaha Musayeva
- **Date:** 11.20.2023


