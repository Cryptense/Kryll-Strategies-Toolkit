[Back to *Going Beyond*](../README.md)

# Managing Function Returns for Improved Navigation

## How does the bot work?

Building on the concept of functions within your bot, you can further enhance your strategy by simulating behavior akin to the CALL and RET instructions in assembly language. In this context, the CALL instruction is used to call a function, while the RET instruction is utilized to return to the point from where the function was initially called.

By leveraging a variable to record the location from where you call a "function", and using the "Test on Variables" block post the execution of the function, you can guide your bot back to the previously recorded location. This way, you can manage your function returns and streamline the navigation within your bot strategy.

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

### How to import a Kryll file?

[Here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-) is an explanation on how to do so. This strategy will also be available on [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).
