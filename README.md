
# Value at Risk Project

Value at Risk (VaR) is a statistical measure used to quantify the level of financial risk within an investment portfolio or a firm. It represents the maximum potential loss that an investment portfolio or trading position may suffer over a specified time horizon at a certain confidence level.

In this project, we explore computing Value at Risk using the Variance-Covariance method, Historical Simulation, and Monte Carlo method.

- Stocks in use: Amazon.com Inc (NASDAQ: AMZN), FedEx Corp (NYSE: FDX), NVIDIA Corp (NASDAQ: NVDA)
- Time Frame: 24 July 2023 - 19 July 2024
- Frequency: Daily


## Collecting the Data

The daily adjusted closing stock prices have been retrieved from Yahoo Finance within the specified time period

![App Screenshot](https://i.postimg.cc/gXYTbfd8/Value-At-Risk-Project-Excel-24-07-2024-05-10-38.png)


## Variance Covariance Method

The Variance-Covariance method, also known as the Parametric method, is another approach for estimating Value at Risk (VaR). Here's how it works:

1. Select Probability Distribution: The Variance-Covariance method assumes that portfolio returns follow a specific probability distribution, often the normal distribution. This assumption allows for the calculation of VaR based on the properties of the chosen distribution.

2. Estimate Parameters: To apply the Variance-Covariance method, you need to estimate the parameters of the chosen distribution, typically the mean (expected return) and standard deviation (volatility) of portfolio returns. These parameters can be estimated using historical data or other methods such as statistical techniques or econometric models.

3. Determine Confidence Level: Decide on the confidence level that corresponds to the desired level of risk tolerance. Common confidence levels include 95%, 99%, or higher.

4. Calculate Z-Score: Using the chosen confidence level, determine the critical value (Z-score) from the standard normal distribution table. For example, for a 95% confidence level, the critical Z-score is approximately 1.645.

5. Compute VaR: Once you have the estimated mean and standard deviation of portfolio returns and the critical Z-score, you can calculate 

The calculated VaR represents the maximum expected loss with the chosen confidence level over the specified time horizon.

![App Screenshot](https://i.postimg.cc/dk4Ss4tX/Value-At-Risk-Project-Excel-24-07-2024-05-11-06.png)

## Historical Simulation Method

The Historical Simulation method of Value at Risk (VaR) calculates the potential loss of an investment or portfolio based on historical data. Here's how it works:

1. Data Selection: Historical prices or returns of the asset or portfolio are collected over a specified historical period, such as daily, weekly, or monthly data.

2. Sorting Data: The historical data is sorted from the most recent to the oldest.

3. Percentile Calculation: The VaR is determined by identifying the nth percentile of the sorted historical returns distribution. For example, the 5th percentile (or another predefined confidence level, such as 95% or 99%) is often used.

4. Calculation: The VaR value is computed as the loss corresponding to the nth percentile of historical returns.

![App Screenshot](https://i.postimg.cc/MfH3vVnG/Value-At-Risk-Project-Excel-24-07-2024-05-11-35.png)

## Monte Carlo Simulation Method

The Monte Carlo method for Value at Risk (VaR) estimation is a simulation-based approach that involves generating multiple scenarios to assess potential losses. Here's how it works:

1. Scenario Generation: Randomly generate numerous scenarios of future asset prices or portfolio values based on statistical assumptions and historical data. This involves simulating potential market movements over the specified time horizon.

2. Portfolio Valuation: For each simulated scenario, compute the portfolio value or asset returns considering factors like market volatility, correlations, and other risk parameters.

3. Loss Calculation: Determine the loss for each simulated scenario by comparing the portfolio value at the end of the period to its initial value. This loss represents the potential adverse impact under that particular scenario.

4. VaR Calculation: Sort the simulated losses in ascending order to identify the nth percentile loss corresponding to the desired confidence level (e.g., 95% or 99%). This percentile loss value is the Monte Carlo VaR.

![App Screenshot](https://i.postimg.cc/kDYhL1HR/Value-At-Risk-Project-Excel-24-07-2024-05-12-13.png)

![App Screenshot](https://i.postimg.cc/kDgp13Td/Value-At-Risk-Project-Excel-24-07-2024-05-12-23.png)

## Acknowledgements

 - [Mehul Mehta](https://www.youtube.com/watch?v=HQvl5c0Ef2M&list=PLn699ZSeIUYdckcUZRJo7MlaTnWguBC4d&index=1)


