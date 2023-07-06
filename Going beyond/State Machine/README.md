[Back to *Going Beyond*](../README.md)

# Implementing State Machines for Enhanced Control

## Introduction

In programming, a state machine is a design pattern allowing an object to alter its behavior based on its current internal state. This concept can be implemented in your Kryll bot to achieve enhanced control over the bot's operation.

You can conceptualize a state machine as a navigational system. It involves a starting point (initial state), a destination (final state), and several intermediate steps (other states). At each step, a direction is determined based on the current state and prevailing conditions.

## How does it work in Kryll?

In a Kryll bot, you can represent the bot's current state using a variable, for instance, 'status'. By using "Operation on Variable" and "Test on Variables" blocks, you can control the execution flow of your bot based on this state variable.

This setup acts like a large switching system (akin to the switch/case structure in traditional programming), where each possible path signifies a state of your bot. Hence, the bot's behavior will change depending on its current state and market conditions.

## Setting up in Kryll.io

You can import the .kryll file in [Kryll.io](https://platform.kryll.io) or follow these steps in the editor:

1. **Create a state variable**: Create a variable to represent the current state of your bot.

2. **Set up "Operation on Variable" blocks**: Utilize these blocks to change the state of your bot based on different conditions.

3. **Use "Test on Variables" blocks**: Use these blocks to control the execution flow of your bot depending on the current state.

## F.A.Q.

### How to import a Kryll file?

[Here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-) is an explanation on how to do so. This strategy will also be available on [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).
