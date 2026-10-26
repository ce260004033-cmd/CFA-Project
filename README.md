CFA Project — Mean Reversion Trading Strategy

Overview

This project implements a mean-reversion trading strategy using Python and evaluates its performance through historical backtesting.

The project also incorporates brokerage and slippage costs to make the backtest more realistic.

Strategy

The strategy is based on the relationship between the current price and its recent moving average.

The main indicators used are:

- 20-day Simple Moving Average (SMA)
- 20-day Standard Deviation
- Z-score

The Z-score is calculated as:

Z = (Price − SMA20) / STD20

Trading Rules

- BUY: Z-score < -2
- SELL: Z-score > 0
- Otherwise, maintain the existing position.

Backtesting

The project evaluates the strategy using historical market data and compares its performance with a Buy & Hold approach.

The backtest accounts for:

- Brokerage
- Slippage
- Trading signals
- Portfolio value
- Returns
- Drawdown
- Risk-adjusted performance

Analysis

The notebook includes analysis of:

- Strategy returns
- Buy & Hold returns
- Brokerage costs
- Slippage costs
- Equity curve
- Drawdown
- Trading signals
- Z-score
- Performance comparison

Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- yfinance
- Jupyter Notebook

Project Structure

CFA-Project/
│
├── .gitignore
├── README.md
└── CFA_Club_Mean_Reversion_Final_Project_with_Brokerage_and_Slippage.ipynb

How to Run

The project can be opened using Jupyter Notebook, JupyterLab, or Google Colab.

Install the required Python packages if necessary:

pip install pandas numpy matplotlib yfinance

Then open the ".ipynb" file and run the cells sequentially.

Disclaimer

This project is intended for educational and research purposes only. Historical backtesting does not guarantee future investment performance and this project should not be considered financial advice.

Author

Naitik Kumar Singh
