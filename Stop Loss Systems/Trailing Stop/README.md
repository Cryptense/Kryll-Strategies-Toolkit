# Kryll Trading Bot: Implementing Trailing Stop for Optimized Trading

## How does the bot work?

A trailing stop is a dynamic strategy that aims to maximize profits and minimize losses in trading operations. Unlike a standard stop-loss, which remains static, a trailing stop moves with market trends. Specifically, it adjusts upwards with each realized profit. In other words, each time a profit is made, the stop-loss level moves up to the level of the previous profit (or to the breakeven point after the first profitable trade). This ensures that profits are secured and risk is minimized if the market reverses.

In this strategy, we will implement a trailing stop on Kryll's platform, allowing for more flexibility in trade management, optimizing profits during bull markets, and protecting capital during market downturns.

## Setup in Kryll.io

You can import the .kryll file in [Kryll.io](https://platform.kryll.io) or follow these steps in the editor:

1. **Create a variable for the trailing stop**: Create a variable, let's name it "trailing_stop". This will contain the value of the current stop-loss level.

2. **Update the trailing stop**: Before each profit realization, update the trailing_stop variable with the value of the previous order. Add a safety margin to account for fees (2 x 0.25% in this example). This raises the stop-loss to the value of the previous profit.

This tiered effect allows the stop-loss level to follow a stair-step motion, making it a dynamic trailing stop.

## F.A.Q.

### How to import a Kryll file?

[Here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-) is an explanation on how to do so. This strategy will also be available on [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

> *Remember that using risk management strategies such as the trailing stop can help optimize your trading operations, but it does not guarantee profits. Always be mindful of the risks inherent in the financial markets.*