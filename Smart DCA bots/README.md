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

## F.A.Q.

### How to import a Kryll file?

[Here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-) is an explanation on how to do so. This strategy will also be available on [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

### What's the minimum recommended amount to start the strategy ?

Due to the minimum purchase limits set by most exchanges (around $10), this strategy should be started with a little more than $500 to ensure it can make 50 orders.

> *Also, be mindful of the market conditions and your personal risk tolerance when setting up this strategy. While Smart DCA can help mitigate some risks associated with market volatility, it doesn't guarantee profits. As always with investing, there's a risk that you could lose money.*