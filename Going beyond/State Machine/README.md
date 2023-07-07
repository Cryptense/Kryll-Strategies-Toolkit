[Back to *Going Beyond*](../README.md)

# Implementing State Machines for Enhanced Control

## Introduction

In programming, a state machine is a design pattern allowing an object to alter its behavior based on its current internal state. This concept can be implemented in your Kryll bot to achieve enhanced control over the bot's operation.

You can conceptualize a state machine as a navigational system. It involves a starting point (initial state), a destination (final state), and several intermediate steps (other states). At each step, a direction is determined based on the current state and prevailing conditions.

## How does it work in Kryll?

In a Kryll bot, you can represent the bot's current state using a variable, for instance, 'status'. By using "Variable Operation" and "Variables Test" blocks, you can control the execution flow of your bot based on this state variable.

This setup acts like a large switching system (akin to the switch/case structure in traditional programming), where each possible path signifies a state of your bot. Hence, the bot's behavior will change depending on its current state and market conditions.

## Setting up in Kryll.io

You can import the .kryll file in [Kryll.io](https://platform.kryll.io) or follow these steps in the editor:

1. **Create a state variable**: Create a variable to represent the current state of your bot.

2. **Set up "Variable Operation" blocks**: Utilize these blocks to change the state of your bot based on different conditions.

3. **Use "Variables Test" blocks**: Use these blocks to control the execution flow of your bot depending on the current state.

<figure style="text-align: center;">
   <img src="https://blog.kryll.io/content/images/2023/07/Capture-d-e-cran-2023-07-06-a--12.28.55.png" alt="State Machines in a Kryll bot">
   <figcaption>Simple state machine in Kryll</figcaption>
</figure>

## F.A.Q.

### How do I import a Kryll file?

You can find a detailed guide on importing a Kryll file [here](https://github.com/Cryptense/Kryll-Strategies-Toolkit/tree/main#how-to-use-a-kryll-file-). This strategy will also be available on the [Kryll.io's Marketplace](https://platform.kryll.io/marketplace).

### What is a state machine?

A state machine is a design pattern in programming where an object changes its behavior based on its current internal state. It can be conceptualized as a navigational system with an initial state (starting point), a final state (destination), and several intermediate states (other steps). In Kryll bot, the bot's behavior changes depending on its current state and market conditions.

### Is there any requirement or prerequisite for implementing a state machine in a Kryll bot?

There is no specific prerequisite for implementing a state machine in a Kryll bot. However, a basic understanding of how state machines work, and familiarity with "Variable Operation" and "Variables Test" blocks in Kryll, will be helpful in setting up your state machine.