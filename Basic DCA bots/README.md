[Back to menu](../README.md)
# Basic Dollar Cost Averaging bot

## How does the bot work?

Dollar Cost Averaging is a strategy in which an individual invests a fixed amount of money at regular intervals, thus buying more assets when prices are low and less when they are high. This technique aims to mitigate the risk of market fluctuations and impulsive investment decisions.

With the Kryll platform, this DCA strategy can be implemented using just four blocks: a calendar block, an AND block, a Buy block, and a Wait block.

## Setup in Kryll.io
You can import the .kryll file in [Kryll.io](https://platform.kryll.io) or follow these steps in the editor:

1. **Set Up a Calendar Block**: Set the calendar block to initiate a buy order every Friday at 00:00.

2. **Add an AND Block**: Attach this block to the calendar block. It will be used to check the balance before executing the buy order.

3. **Create a Balance Block**: This block is used with the AND block to verify that there are sufficient funds available to perform the buy operation.

4. **Implement a Buy Block**: Configure this block to use 2% of your starting capital for each purchase. This will allow for 50 purchases throughout the year, evenly distributed across each Friday.

5. **Include a Wait Block**: This block causes the strategy to pause for one day after each purchase before it begins again.

<figure style="text-align: center;">
   <img src="https://blog.kryll.io/content/images/2023/07/image-7.png" alt="alt text">
   <figcaption>Basic DCA strategy buying every friday</figcaption>
</figure>

## F.A.Q.

### How do I import a Kryll file?

You can find a detailed guide on how to import a Kryll file [here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-). This strategy will also be available on the [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

### What's the minimum recommended amount to start the DCA strategy?

Due to the minimum purchase limits set by most exchanges (around $10), it is recommended to start this strategy with a little more than $500. This ensures that the bot can make the intended 50 orders throughout the year.

### Why does the DCA bot buy on Fridays?

Based on a study conducted by the Kryll team, Friday might be the best day to invest in Bitcoin. You can read more about the study [here](https://blog.kryll.io/best-day-to-buy-bitcoin/).


> *Also, be mindful of the market conditions and your personal risk tolerance when setting up this strategy. While DCA can help mitigate some risks associated with market volatility, it doesn't guarantee profits. As always with investing, there's a risk that you could lose money.*
