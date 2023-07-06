[Back to menu](../README.md)

# Using Win/Loss Ratio for Decision Making

## How does the bot work?

The win/loss ratio is a useful metric in assessing the effectiveness of a trading bot. This ratio, which is the total number of winning trades to losing trades, can help refine decision-making in a bot's operations. For instance, if you have made 80 winning trades and 20 losing trades, your win/loss ratio is 80/20 = 4. This implies that for every losing trade, you average 4 winning trades. 

In this strategy, we will use the win/loss ratio to adjust the behavior of our trading bot. Depending on the ratio, we may decide to take more risks or be more conservative, thereby balancing the risk in our trading strategy.

## Setup in Kryll.io

You can import the .kryll file in [Kryll.io](https://platform.kryll.io) or follow these steps:

1. **Create variables**: Initiate two variables, "winning_trades" and "losing_trades". Increment each of these variables each time a corresponding trade is made.

2. **Calculate the win/loss ratio**: Use the "Variable Operation" block to divide "winning_trades" by "losing_trades". This will provide the win/loss ratio.

3. **Adjust the trading strategy based on the ratio**: A high win/loss ratio may indicate the strategy is performing well, allowing for more risk-taking for potential higher gains. If the ratio is low, the strategy might need to be more conservative, reducing position sizes or targeting less risky trades.

For example, we could have 3 different risk modes:

- Low risk: Only use 40% of the starting capital if the strategy is not profitable.
- Medium risk: Use 60% of the starting capital if the strategy is profitable but the win/loss ratio is less than one.
- High risk: Use 80% of the available capital if the strategy is profitable and the win/loss ratio is greater than one.

This strategy allows us to adjust the level of risk based on the bot's performance (RoE and win/loss ratio). We can limit our risk when the strategy is underperforming and increase our risk appetite during profitable periods.

## F.A.Q.

### How to import a Kryll file?

[Here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-) is an explanation on how to do so. This strategy will also be available on [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

### What's the minimum recommended amount to start the strategy ?

Since this strategy does not buy nor sell small amounts of assets, you can start with Kryll minimal amount if you don't want to invest too much.

> *Always remember that using metrics such as the win/loss ratio is a part of risk management, but it doesn't guarantee profits. The financial markets are inherently risky and volatile, and there's always a chance you could lose money.*
