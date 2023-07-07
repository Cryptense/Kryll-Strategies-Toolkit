[Back to menu](../README.md)

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

<figure style="text-align: center;">
   <img src="https://blog.kryll.io/content/images/2023/07/image-12.png" alt="alt text">
   <figcaption>For loop in Kryll</figcaption>
</figure>

## F.A.Q.

### How do I import a Kryll file?

You can find a detailed guide on how to import a Kryll file [here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-). This strategy will also be available on the [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

### What is a 'for' loop and how is it used in trading bots?

A 'for' loop is a control structure used in programming to perform a block of code a specific number of times. In trading bots, it can be used to perform repetitive actions, such as systematically buying at every bullish signal. On the Kryll platform, 'for' loops can be emulated using 'Variables Operation' and 'Variables Test' blocks.

### How can I set up a 'for' loop in my trading bot on Kryll?

To set up a 'for' loop in a Kryll trading bot, start by initializing a variable using the 'Variable Operation' block in 'Assignment' mode. Then, use a 'Variables Test' block and another block (e.g., a SuperTrend block) to create an AND condition. If the condition is valid, the bot performs a certain action (like buying). After executing the action, increment the variable using another 'Variable Operation' block in 'Operation' mode. Finally, connect the output of this operation to the 'Variables Test' block to create a loop for the action. As long as the variable remains less than or equal to a specified value (e.g., 20), the action will be repeated.

### What are the benefits of using a 'for' loop in my trading bot?

Using a 'for' loop in your trading bot allows you to execute specific actions in an iterative and controlled manner. This can be particularly useful for accomplishing repetitive actions, such as buying at every bullish signal, and for controlling the progress of your strategy with increased precision.

> *Also, remember that trading strategies can carry risk. While loops and other tools can help manage repetitive actions, they do not guarantee profits. Always be mindful of your risk tolerance when setting up trading strategies.*
