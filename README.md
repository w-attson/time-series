# Forecasting Net Prophet

This project anaylses MercadoLibre. With over 200 million users, MercadoLibre is the most popular e-commerce site in Latin America. It involves analysing the company's financial and user data in ways to help the company grow. 

## Part 1: Patterns in hourly Google Search Traffic
* Read the search data into a DataFrame
  * Slice the data to just the month of May 2020
  * Plot to visualize the results. Do any unusual patterns exist?
* Calculate the total search traffic for the month.
  * Then compare the value to the monthly median across all months.
  
## Part 2: Mine the search traffic data for seasonality
* Group the hourly search data to plot the average traffic by the day of the week (for example, Monday vs. Friday).
* Visualize this traffic as a heatmap.
* Group the search data by the week of the year.

## Part 3: Relate the search traffic to stock price patterns

* Read in and plot the stock price data. 
* Concatenate the stock price data to the search data in a single DataFrame.
* Slice the data to just the first half of 2020 (2020-01 to 2020-06 in the DataFrame),
* Use hvPlot to plot the data. 

* Lagged Search Trends
  * Offsets, or shifts, the search traffic by one hour. to determine trends.

* Stock Volatility
  * Which holds an exponentially weighted four-hour rolling average of the company’s stock volatility

* Hourly Stock Return
*Which holds the percent change of the company's stock price on an hourly basis

*Review the time series correlation, and then answer the following question:
  * Determine a relationship between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns.

## Part 4: Time series model with Prophet

* Set up the Google search data for a Prophet forecasting model.

* After estimating the model, plot the forecast.

Plot the individual time series components of the model to determine the following:
  * What time of day exhibits the greatest popularity?
  * Which day of the week gets the most search traffic?
  * What's the lowest point for search traffic in the calendar year?

## Part 5: Forecast revenue by using time series models

* Read in the daily historical sales (that is, revenue) figures, and then apply a Prophet model to the data.
* Interpret the model output to identify any seasonal patterns in the company's revenue.
* Produce a sales forecast for the finance group. Give them a number for the expected total sales in the next quarter. Include the best- and worst-case scenarios to help them make better plans.
