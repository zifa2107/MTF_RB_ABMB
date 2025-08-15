# Consolidated Backtesting
## stop-loss and take-profit check
-add new condition for average down price before rolling sl (Buy)
 exit_reason = "average down"
 exit_price = average price
-add average up price condition before rolling sl (Sell)
 exit_reason = "average up"
 exit_price = average price
-average down and average up formula from tp and sl 

# Order Execution
## load latest signal data
-clean live data before execute
-calculate the difference between previous and current
-if same signal overload, exit/ignore

-currently only send market order, need to add send limit order function
-create for long and short (comment for short)
