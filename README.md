# Pandas-Project

Week 4 FinTech Bootcamp.

This is the homework for week 4 analysing portfolio returns in Python using Pandas.

The file is named "whale_analysis_NJ.ipynb" and is stored in the folder "Starter_Code"

"Whale Analysis"

# Steps involved:
### Prepare the Data

First, read and cleaned several CSV files for analysis. The CSV files include whale portfolio returns, algorithmic trading portfolio returns, and S&P 500 historical prices. Used the Jupyter Notebook to complete the following steps:

1. Use Pandas to read in each of the [CSV files](Starter_Code/Resources) as a DataFrame. Also, converted the dates to a `DateTimeIndex`.

2. Detected and removed the null values.

3. Removed the dollar signs from the numeric values and converted the data types as needed.

4. The whale portfolios and algorithmic portfolio CSV files contained daily returns, but the S&P 500 CSV file contains closing prices. Converted the S&P 500 closing prices to daily returns.

5. Joined `Whale Returns`, `Algorithmic Returns`, and the `S&P 500 Returns` into a single DataFrame with columns for each portfolio's returns.

 

### Conduct Quantitative Analysis

Analyzed the data to see if any of the portfolios outperformed the stock market (i.e., the S&P 500).

#### Performance Analysis

1. Calculated and plotted cumulative returns. Two portfolios outperformed the S&P 500?

#### Risk Analysis

1. Created a box plot for each of the returns. Larger spread of the box indicates more risk in the portfolio.

2. Calculated the standard deviation for each portfolio. 

3. Calculated the annualized standard deviation (252 trading days).

#### Rolling Statistics

1. Plotted the rolling standard deviation of the various portfolios along with the rolling standard deviation of the S&P 500 using a 21 day rolling window. 

2. Constructed a correlation table for the algorithmic, whale, and S&P 500 returns. 

3. Another way to calculate a rolling window is to take the exponentially weighted moving average(ewm). This is like a moving window average, but it assigns greater importance to more recent observations. Calculated the ewm with a 21 day half-life.

### Plot Sharpe Ratios

Investment managers and their institutional investors look at the return-to-risk ratio, not just the returns. (After all, if you have two portfolios that each offer a 10% return, yet one is lower risk, you would invest in the lower-risk portfolio, right?)

1. Using the daily returns, calculated and visualized the Sharpe ratios using a bar plot.

2. Determined whether the algorithmic strategies outperform both the market (S&P 500) and the whales portfolios.
