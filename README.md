# Quant_Backtesting_Models

MACD:

**Overarching Strategy:** The Moving Average Convergence Divergence (MACD) is a technical analysis tool that uses momentum to find opportunities to buy/sell. Academic Papers like Jegadesh & Titman (Implemented in a different repo, soon to be linked) have proved that momentum still works and I wanted to extend this to see if MACD also produces returns. We are looking at the exponential moving average and whenever it flips from positive to negative we sell, and when it flips from negative sentiment to positive sentiment we buy.



**Some Assumptions that are made: **

1. Buying and Selling are cut off such that they are 1:1 to not deal with the implications of Shorting & costs.  
2. Starting with 10,000 of capital, on a buy signal you will buy as much as you can and sell everything.

TODO/Additional Considerations
1. Adjusting the buy signal based on duration/intensity of switches
2. Trading costs are not incorporated
3. I assume we can easily short stocks without problem, and that the eventual buy pair cancels out the short leg.
4. How does this strategy perform during times of intense volatility?
