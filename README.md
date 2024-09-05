# Telecom Stock Analysis
    Teaam Lead :Yara  https://github.com/Yelemam/Project1-Telecom-Stock
    Hunter https://github.com/Yelemam/Project1-Telecom-Stock/tree/feature/Hunter
    Sanjana https://github.com/Yelemam/Project1-Telecom-Stock/tree/feature/Sanjana
    Adolphous https://github.com/Yelemam/Project1-Telecom-Stock/tree/feature/Adolphous
    Kowsar https://github.com/Yelemam/Project1-Telecom-Stock/tree/feature/Kowsar
    
## Project Overview
   This project analyzes the stock performance of three major telecom companies: AT&T(T), T-Mobile (TMUS), and Verizon (VZ) over a one-year period until today. 
   The analysis includes trend analysis, volatility assessment, correlation studies, performance comparisons, divedend rate and P/E ratio to provide insights for
   potential investors.

## Data Source
   The data used in this analysis is sourced from Python with the yfinance library. This library allows you to easily download historical market data from Yahoo
   Finance. This data contains daily trading information including opening, closing, high, and low prices, 
   as well as trading volumes , corporate actions and earnings data for each company.

## Analysis Performed

1. **Trend Analysis**
   - A line plot showing the closing prices of all three stocks over the year.
   - This visualizes the overall price trends and allows for easy comparison between the companies.

2. **Moving Averages**
   - Calculation and visualization of 20-day moving averages for each stock. It takes a certain day and finds a trend over 20 days. (takes 10 days before the day 
     and 10 days after and calculates the average)
   - Helps in identifying short-term trends and smoothing out price fluctuations. (if there are any unusual jumps it will show)

3. **Daily Returns**
   - Calculation of daily returns for each stock. (The average change from one day to another. The percentage value is between 0-1
   - Used in subsequent analyses for volatility and correlation.

4. **Volatility Analysis**
   - Computation of annualized volatility for each stock.
   - Visualized using a bar plot to compare the relative risk of each stock
   - The change in stock. If the change gap is huge, it means that the stock is risky and not stable (this can be good for high-risk clients over a short period
     of time. If the Change is small, it’s more stable less risky stock)
     Volatility Bar Chart: https://raw.githubusercontent.com/Yelemam/Project1-Telecom-Stock/main/Volatility.png
     
5. **Correlation Analysis**
   - Calculation of correlation between the daily returns of the three stocks. (to measure the size of the stock with the other companies)
   - Visualized using a heatmap to show the strength and direction of relationships between the stocks. (Same colour and similar they are 100% matching stocks)
     Heatmap: https://raw.githubusercontent.com/Yelemam/Project1-Telecom-Stock/main/correlation.png
     
6. **Cumulative Returns**
   - Calculation and visualization of cumulative returns for each stock. (Return is between 0-1 so we need to add 1 to the return before calculating the cum to  
     remove the decimal 
   - Provides insight into overall performance over the entire period.
    Cumulative return chart: https://raw.githubusercontent.com/Yelemam/Project1-Telecom-Stock/main/cum_returns.png

7. **Candlestick Charts**
   - Creation of candlestick charts for each company. (This is one of the main Charts used to analyse stock market data)
   - Offers a detailed view of daily price movements, including opening, closing, high, and low prices.
     TMUS candlestick:  https://raw.githubusercontent.com/Yelemam/Project1-Telecom-Stock/main/TMUS_candlestick_plot.png 
     T canlestick: https://raw.githubusercontent.com/Yelemam/Project1-Telecom-Stock/main/T_candlestick_plot.png
     VZ candlestick: https://raw.githubusercontent.com/Yelemam/Project1-Telecom-Stock/main/VZ_candlestick_plot.png
     
8. **Trading Volume Analysis**
   - Visualization of trading volume over time for each stock.
   - Helps in understanding liquidity and investor interest.
     Volume graph: https://raw.githubusercontent.com/Yelemam/Project1-Telecom-Stock/main/Volume.png
     
9. **Dividend and P/E ratio**
   - Retrieves the dividends rate and trailling price to earning ratio from yfinance.
   - Calculate dividend yield by taking dividend rate/ last stock price.
  
10. **Summary Statistics**
   - Compilation of key statistics including start price, end price, percent change, average daily return, and volatility.
   - Provides a quick overview of each stock's performance.

## Key Findings

1. Best Performer: The analysis identifies the stock with the highest price appreciation over the year.
2. Lowest Volatility: The stock with the lowest volatility is highlighted, indicating potentially lower risk.
3. Correlation Insights: The correlation analysis reveals how the stocks move in relation to each other,
   which is crucial for portfolio diversification.
4. Volume Trends: The trading volume analysis provides insights into the liquidity
   of each stock.
5. VZ stands out for its relatively high dividend yield, making it potentially attractive for income-seeking investors. T falls in between the other two companies in terms of both dividend yield and P/E ratio.

## Recommendations

Based on the analysis, the script provides a basic recommendation for portfolio composition, considering both growth potential and stability. 
However, it emphasizes that these recommendations should be considered in the context of an investor's risk tolerance and overall investment strategy.
For income-oriented investors looking for steady dividends, VZ may be a suitable choice. T could be a balanced choice for investors looking for a mix 
of dividends and possible bargain.

## Limitations and Future Improvements

- The analysis is based on historical data and does not predict future performance.
- Additional factors such as company fundamentals, market conditions, and economic indicators could be incorporated for a more comprehensive analysis.
- The time frame could be extended or shortened to observe different trends.

## How to Run the Script

1. Ensure you have Python installed on your system.
2. Install required libraries: pandas, numpy, matplotlib, seaborn, and mplfinance.
3. Place the "cell_phone_companies_trading_data.csv" file in the same directory as the script.
4. Run the script using a Python interpreter.

## Output

The script generates several visualizations saved as image files and prints summary statistics and recommendations to the console.

## Conclusion

This analysis provides a comprehensive overview of the performance of AT&T, T-Mobile, and Verizon stocks over a one-year period. It offers valuable insights 
for investors considering these telecom stocks, highlighting trends, risks, and relative performance.
