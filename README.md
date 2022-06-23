# Comparing Weather Trends in Madrid and the World

This project was a warmup for the Udacity "Data Analyst" certificate. I was provided with an SQL database consisting of tables with global yearly average temperatures as well as yearly averages for major cities. The objective was to compare global temperatures with those of my nearest large city across time. My nearest large city was Madrid, Spain. 

## Data Gathering

To gather the data, I used a simple join to connect global temperatures and Madrid temperatures based on year. I then downloaded the data as a csv file and imported it into a Pandas dataframe in Python.

## Data Cleaning

The only true cleaning to be done was to remove the data from before the year 1750, as there were NaN values.

I did, however, have to prepare the data for visualization. Since this was to be a time series analysis of temparature, the best visual I could think to use was a simple line chart. Having many data points would have made the graph chaotic, and trends wouldn't be visible. So I added a rolling average column to smooth out the data for the line chart. 

## Visualization

Finally, using Python's Matplotlib library, I plotted line charts of Madrid temparatures and global temperatures on the same graph to facilitate comparison. 
