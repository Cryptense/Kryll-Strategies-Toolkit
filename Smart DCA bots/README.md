[Back to menu](../README.md)

# Smart Dollar Cost Averaging bot

## How does the bot work?

Smart Dollar Cost Averaging (DCA) involves adapting the investment pace according to market conditions. It aims to invest at a fixed date only if the Bitcoin price is lower than our average purchase price, helping to avoid over-investing during rebound phases. It's an enhanced version of the standard DCA strategy that takes into account market conditions to optimize the investment decisions.

This smart DCA strategy can be implemented on the Kryll platform by using the variables feature to configure your trading algorithm to react to market fluctuations.

This approach allows us not only to significantly increase the performance of the strategy in terms of return on investment, but also to significantly reduce the drawdown of our bot.

## Setup in Kryll.io
This strategy is very similar from the Basic DCA one.

You can import the .kryll file in [Kryll.io](https://platform.kryll.io) or follow these steps in the editor:

1. **Set Up a Calendar Block**: Set the calendar block to initiate a buy order every Friday at 00:00.

2. **Add an AND Block**: Attach this block to the calendar block. It will be used to check the balance before executing the buy order.

3. **Create a Balance Block**: This block is used with the AND block to verify that there are sufficient funds available to perform the buy operation.

4. **Implement a Buy Block**: Configure this block to use 2% of your starting capital for each purchase. This will allow for 50 purchases throughout the year, evenly distributed across each Friday.

5. **Include a Wait Block**: This block causes the strategy to pause for one day after each purchase before it begins again.

6. **Add a Variable Test block**: This block will allow us to validate the purchase only if the price is strictly lower than the average price we have bought at so far.

<figure style="text-align: center;">
   <img src="https://blog.kryll.io/content/images/2023/07/image-10.png" alt="alt text">
   <figcaption>Smart DCA strategy on Kryll</figcaption>
</figure>

## F.A.Q.

### How do I import a Kryll file?

You can find a comprehensive guide on importing a Kryll file [here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-). This strategy is also available on the [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

### What is the minimum recommended amount to start the strategy?

Due to the minimum purchase limits set by most exchanges (around $10), it's recommended to start this strategy with at least $500. This ensures that the bot can make 50 orders over the year.

### What is the difference between Smart DCA and standard DCA?

While standard Dollar Cost Averaging (DCA) invests a fixed amount at regular intervals regardless of the asset's price, Smart DCA adjusts the investment according to market conditions. Specifically, it invests only when the Bitcoin price is lower than the average purchase price, helping to optimize investment decisions and avoid over-investing during rebound phases.

### How does the Smart DCA strategy reduce the bot's drawdown?

By investing only when the Bitcoin price is lower than the average purchase price, the Smart DCA strategy avoids over-investing during periods of price rebounds. This strategy can significantly reduce drawdowns or declines in the bot's account value, thus preserving the capital.

### How often does the Smart DCA strategy execute trades?

The strategy is set to execute a trade every Friday at 00:00, provided that there are sufficient funds available, and the current Bitcoin price is lower than the average purchase price. This equates to around 50 trades per year.

### What does the Variable Test block do in the Smart DCA strategy?

The Variable Test block validates a purchase only if the current price of Bitcoin is strictly lower than the average price at which we've bought Bitcoin so far. This ensures the strategy adheres to the principle of buying low, a key element of the Smart DCA strategy.

> *Also, be mindful of the market conditions and your personal risk tolerance when setting up this strategy. While Smart DCA can help mitigate some risks associated with market volatility, it doesn't guarantee profits. As always with investing, there's a risk that you could lose money.*