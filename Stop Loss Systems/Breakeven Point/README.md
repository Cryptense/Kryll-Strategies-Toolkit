[Back to *Stop Loss Systems*](../README.md)


# Incorporating Trading Fees into Your Breakeven Point

## How the Bot Works

This bot aims to optimize trading strategies by factoring in trading fees while setting up stop-loss and breakeven mechanisms. The main principle revolves around considering fees in the breakeven point calculation, ensuring an accurate estimation of the point at which a trade moves from unrealized loss to unrealized gain. 

For example, if you buy an asset at 100€ and the transaction fees are 1%, then your real entry price is 101€. Therefore, to reach breakeven, the asset price needs to reach 101€, not 100€.

This approach becomes particularly beneficial in volatile markets, where a seemingly profitable trade can quickly turn into a loss. Implementing a dynamic breakeven point and stop-loss, incorporating transaction fees, can enhance the trade's profitability and risk management.

## Setup

The bot implements a strategy that accumulates BTC every 48 hours, provided we are on a downtrend based on a 2-hour SuperTrend indicator. Once our ROI exceeds 2%, we take 25% of our profits and cut our position if the SuperTrend turns bearish or if the current price hits our breakeven level.

Here's how you can set up the bot:

1. **Updating the Breakeven Point**: After each purchase, the bot updates the `break_even` pivot point. This is calculated as the average purchase price plus 0.5% trading fees (0.25% on purchase and 0.25% on sale).

2. **Breakeven Test Block Setup**: Once the strategy shows a 2% profit, the bot checks whether the asset price has fallen below (or is equal to) our `break_even` price. If true, the bot exits the trade.

This setup led to generating a return of over 34% on BTC between June 2022 and June 2023 in a bear market scenario.

## F.A.Q.

### How to import a Kryll file?

[Here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-) is an explanation on how to do so. This strategy will also be available on [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

### How does this bot help improve my trading strategy?

The bot improves your strategy by accurately calculating your breakeven point, considering transaction fees. This allows you to limit potential losses and exit trades at the right time, especially in volatile markets.

### How does the bot handle the breakeven point?

After each purchase, the bot updates the breakeven point, calculated as the average purchase price plus trading fees. Once the strategy shows a 2% profit, the bot checks whether the asset price has fallen below (or is equal to) our breakeven price. If true, the bot exits the trade.

### Can I use this bot for other assets apart from BTC?

Yes, while the bot is demonstrated using BTC, you can customize it to work with other assets as per your trading strategy.

> *Remember that using risk management strategies such as the breakeven point can help optimize your trading operations, but it does not guarantee profits. Always be mindful of the risks inherent in the financial markets.*
