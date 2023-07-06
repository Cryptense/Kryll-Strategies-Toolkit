# Kryll Trading Bot: Adaptive Stop-Loss for Leveraged Trading

## How does the bot work?

Applying different levels of leverage in your trades alters the risk-reward dynamic. An adaptive stop-loss mechanism can be implemented to manage this risk more effectively. This mechanism adjusts the stop-loss level according to the leverage being used, ensuring a consistent risk management strategy across different levels of leverage.

Specifically, if we want to develop a bot that follows SuperTrend signals on a 6-hour timeframe, aiming for a 10% profit-taking and a 5% stop-loss with a maximum risk of 1% of the capital, a static stop-loss does not maintain this risk level when leverage is applied. 

To maintain the 1% risk level regardless of leverage, an adaptive stop-loss that adjusts according to the leverage is necessary.

## Setup in Kryll.io

You can import the .kryll file in [Kryll.io](https://futures.kryll.io) or follow these steps in the editor:

1. **Initialize the `STOP_VALUE` variable**: Adjust the value of the stop-loss according to the leverage being used, i.e., 5% divided by the leverage (0.05 / leverage).

2. **Calculate the `stop_gap`**: This is the potential loss amount that would trigger the stop-loss. It's calculated as `STOP_VALUE` multiplied by the asset price.

3. **Determine the `stop_loss` value**: This is the price that would trigger the stop-loss. It's calculated as purchase price minus `stop_gap`.

By employing these steps, the stop-loss adapts to the leverage, ensuring the risk is limited to 1% of the capital per trade, as opposed to 1% multiplied by the leverage.

## F.A.Q.

### How to import a Kryll file?

[Here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-) is an explanation on how to do so. This strategy will also be available on [Kryll.io's Marketplace](https://futures.kryll.io/marketplace).

> *Always remember that while leveraging can potentially increase profits, it also magnifies losses. Always be mindful of the risks inherent in the financial markets.*
