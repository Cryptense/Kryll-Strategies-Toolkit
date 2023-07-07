[Back to menu](../README.md)

# Incorporating Functions for Greater Flexibility

## How does the bot work?

A key concept in programming, and now possible with Kryll's variable and "GoTo" blocks, is the creation of "functions" within your bot. These are essentially sections of code designed to perform specific tasks and can be called upon multiple times throughout your bot's operation. This allows for code reuse, making your bot more organized, readable, and easier to maintain.

For instance, you can define a portion of your bot to update your stop-loss. Whenever certain conditions are met (such as after each trade), the bot can be directed to this portion to update the stop-loss. This updated variable can then be used elsewhere in your bot to guide trading decisions.

## Setup in Kryll.io

You can import the .kryll file in [Kryll.io](https://platform.kryll.io) or follow these steps in the editor:

1. **Create a designated section for a specific task**: This "function" could be for updating a stop-loss, calculating a moving average, or any other specific task. You will need to use a combination of the "Variable Operation" and "GoTo" blocks to define this section.

2. **Direct your bot to the function**: When the conditions for performing the specific task are met, use the "GoTo" block to navigate to the function.

3. **Use the results of the function**: After the function is executed, the bot can then use the updated variables in other parts of the bot to inform trading decisions.

Remember that setting up "functions" in your bot will require careful planning and organization. However, once established, they can simplify your bot's operation, leaving you to focus on fine-tuning your trading strategies.

<figure style="text-align: center;">
   <img src="https://blog.kryll.io/content/images/2023/07/image-31.png" alt="alt text">
   <figcaption>Function-like flow in Kryll</figcaption>
</figure>

## F.A.Q.

### How do I import a Kryll file?

You can find a detailed guide on how to import a Kryll file [here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-). This strategy will also be available on the [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

### What is a "function" in the context of a Kryll bot?

In the context of a Kryll bot, a "function" is a designated section of the bot that is set up to perform a specific task. These functions are akin to functions in traditional programming, enabling code reuse for more organized and manageable bots. You can define functions to perform tasks like updating a stop-loss, calculating a moving average, or any other specific task.

### Do I need any specific skills to implement functions in my Kryll bot?

Creating functions in your Kryll bot requires a basic understanding of the concept of functions in programming and the use of the "Variable Operation" and "GoTo" blocks in Kryll. Moreover, setting up functions requires careful planning and organization to ensure that your bot operation is streamlined and effective.
