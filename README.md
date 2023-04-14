# Piotroski Score Backtest using Tesla Stock and IEX Cloud API
https://commonstock.com/post/60cc5409-2e45-45f5-bed6-307b932ffb9b

## Requirements

- Python 3.6+
- pandas
- requests
- matplotlib

## Usage

1. Replace `YOUR_API_KEY` in the code with your actual IEX Cloud API key.
2. Adjust the `stock`, `start_date`, and `end_date` variables in the `main()` function as needed.
3. Run the code to see the final portfolio value and the stock price chart with buy signals.

## Key Functions

- `get_financial_data(stock, statement_type)`: Retrieves financial data from the IEX Cloud API.
- `get_price_data(stock, start_date, end_date)`: Retrieves historical price data from the IEX Cloud API.
- `calculate_profitability_factors(financial_data, financial_data_prev)`: Calculates the profitability factors of the Piotroski Score.
- `backtest_profitability_factors(price_data, financial_data)`: Runs the backtest using the profitability factors and returns the final portfolio value and buy points.
- `plot_stock_with_buy_signals(price_data, buy_points)`: Plots the stock prices with buy signals.

## License

MIT License. See [LICENSE](LICENSE) for more information.
