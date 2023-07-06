# Creating a 'for' Loop with Trading Bots on Kryll

## How does the bot work?

In programming, 'for' loops are used to perform repetitive actions. Now, thanks to the 'Variables Operation' and 'Variables Test' blocks on Kryll, you can emulate these loops in your trading bots. This addition allows for greater customization of our strategies by executing specific actions in an iterative and controlled manner.

This bot is designed to systematically buy the next 20 bullish SuperTrend 4h signals with 5% of the starting capital at each iteration, provided the positions don't accumulate a 10% gain. This action will be repeated 20 times, essentially creating a 'for' loop.

## Setup in Kryll.io

You can import the .kryll file in [Kryll.io](https://platform.kryll.io) or follow these steps in the editor:

1. **Initialize a variable**: Start by using the 'Variable Operation' block in 'Assignment' mode to initialize a variable, which we will call 'counter', to 0.

2. **Create an AND condition**: Use a SuperTrend block and a 'Variables Test' block to check if the 'counter' is less than 20.

3. **Implement the desired action**: If the above combination of blocks is valid (i.e., we have a buy signal), we can proceed to buy or perform any other action you want to repeat.

4. **Increment the counter**: After executing the action, use another 'Variable Operation' block in 'Operation' mode to increment 'counter' by 1.

5. **Create the loop**: Finally, connect the output of this operation to the 'Variables Test' block to create a loop for the action.

With this setup, as long as 'counter' is less than or equal to 20, the action we have defined will be repeated. This method can be particularly useful for accomplishing repetitive actions and for controlling the progress of your strategy with increased precision.

## F.A.Q.

### How to import a Kryll file?

[Here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-) is an explanation on how to do so. This strategy will also be available on [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

> *Also, remember that trading strategies can carry risk. While loops and other tools can help manage repetitive actions, they do not guarantee profits. Always be mindful of your risk tolerance when setting up trading strategies.*
