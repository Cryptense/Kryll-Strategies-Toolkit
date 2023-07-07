[Back to *Going Beyond*](../README.md)

# Managing Function Returns for Improved Navigation

## How does the bot work?

Building on the concept of functions within your bot, you can further enhance your strategy by simulating behavior akin to the CALL and RET instructions in assembly language. In this context, the CALL instruction is used to call a function, while the RET instruction is utilized to return to the point from where the function was initially called.

By leveraging a variable to record the location from where you call a "function", and using the "Variables Test" block post the execution of the function, you can guide your bot back to the previously recorded location. This way, you can manage your function returns and streamline the navigation within your bot strategy.

## Setup in Kryll.io

You can import the .kryll file in [Kryll.io](https://platform.kryll.io) or follow these steps in the editor:

1. **Create a variable to track the function call location**: Before calling a function, record the location using a variable.

2. **Direct your bot to the function**: Use the "GoTo" block to navigate your bot to the desired function.

3. **Return to the calling location**: After executing the function, use the "Variables Test" block to guide your bot back to the recorded location.

Remember, this approach requires meticulous planning for setting up and managing the function returns, but it greatly enhances the organization and flow of your bot strategy.

<figure style="text-align: center;">
   <img src="https://blog.kryll.io/content/images/2023/07/image-32.png" alt="alt text">
   <figcaption>Functions with returned value in Kryll</figcaption>
</figure>

## F.A.Q.

### How do I import a Kryll file?

You can find a detailed guide on how to import a Kryll file [here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-). This strategy will also be available on the [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

### What does "managing function returns" mean?

Managing function returns involves tracking the location from where a function is called and returning to that location once the function execution is complete. This can be achieved by using a variable to record the calling location and then using the "Variables Test" block to navigate back to the recorded location.

### Do I need any specific knowledge to implement function return management in my Kryll bot?

While no specific prerequisite knowledge is needed, familiarity with the concept of functions in programming, as well as the use of variables and "GoTo" and "Variables Test" blocks in Kryll, will be beneficial. Also, meticulous planning is needed to effectively set up and manage the function returns within your bot strategy.
