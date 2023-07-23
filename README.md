Here is a more detailed explanation of the steps involved in each question:

Q1-Create a combined report with all key metrics (esp: Spends and Returns %) in a weekly and monthly format. Decide the number of data fields you would like to showcase here.
file: p1.ipynb

Preprocessing:
The first step is to convert the NAN values in the Payment and Cost column to some mathematical values which will be optimal for mathematical calculations. This can be done using the fillna() function in Pandas.
The next step is to extract the week and month from the week column in the Google Ads dataset. This can be done using the dt.isocalendar() function in Pandas.
Calculations:
The next step is to calculate the returns. This can be done by subtracting the cost from the payment.
Once the returns have been calculated, we can aggregate them by week and month. This can be done using the groupby() function in Pandas.
Visualization:
Finally, we can visualize the weekly and monthly returns using line plots and bar plots. This can be done using the plot() function in Matplotlib.


Q2-Which is the most profitable channel
file: p2.ipynb

Preprocessing:
The first step is to convert the values in the Paid column to some useful mathematical value. This can be done by converting the string values to numeric values.
Calculations:
The next step is to find the amount spent on each channel. This can be done by using the pivot_table() function in Pandas.
Once the amount spent on each channel has been calculated, we can find the amount earned on each channel. This can be done by using the pivot_table() function again, but this time setting the values argument to Payment.
Finally, we can subtract the amount earned from the amount spent to find the profit for each channel.
Visualization:
Finally, we can visualize the profit for each channel using a bar chart. This can be done using the bar() function in Matplotlib.


Q3-Which category/keyword is the most profitable
file: p3.ipynb

Calculations:
The first step is to find the cost for each category. This can be done by using the pivot_table() function in Pandas.
Once the cost for each category has been calculated, we can find the profit for each category. This can be done by using the pivot_table() function again, but this time setting the values argument to Payment.
Finally, we can find the category with the highest profit by comparing the profits for each category.
Visualization:
Finally, we can visualize the profit for each category using a bar chart. This can be done using the bar() function in Matplotlib.

Q4-Look for insights by analyzing data points on time series graphs
file: p4.ipynb

Calculations:
The first step is to analyze each data point with respect to the date that has been provided in the dataset. This can be done by using the dt.date() function in Pandas.
Once the data has been analyzed with respect to the date, we can plot the data points on a time series graph. This can be done using the plot() function in Matplotlib.
Visualizations:
We can use the matplotlib and sns packages to plot a heatmap of the data. This will help us to visualize the trends in the data over time.

Q5-Analyse the Impact of geography
file: p5.ipynb

Calculations:
The first step is to analyze each data point with respect to the geography that has been provided in the dataset. This can be done by using the dt.country() function in Pandas.
Once the data has been analyzed with respect to the geography, we can plot the data points on a map. This can be done using the plot() function in Matplotlib.
Visualizations:
We can use the matplotlib and sns packages to plot a heatmap of the data. This will help us to visualize the trends in the data for each geography.
