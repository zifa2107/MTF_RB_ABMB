## Consolidated Backtesting
### stop-loss and take-profit check
1. add new condition for average down price before rolling sl (Buy)
- exit_reason = "average down"
- exit_price = average price
2. add average up price condition before rolling sl (Sell)
- exit_reason = "average up"
- exit_price = average price
3. average down and average up formula from tp and sl 

## Order Execution
### load latest signal data
1. clean live data before execute
2. calculate the difference between previous and current
3. if same signal overload, exit/ignore

- currently only send market order, need to add send limit order function
- create for long and short (comment for short)

## References
1. https://www.mql5.com/en/articles/18985
2. https://www.mql5.com/en/articles/18971
