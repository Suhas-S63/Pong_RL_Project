# Pong Reinforcement Learning Agent

## Showcase:
![PongRLGif](https://github.com/Suhas-S63/Pong_RL_Project/blob/main/PongRLGif.gif)

## Overview
This project implements a **Reinforcement Learning (RL) agent** using the **Deep Q-Network (DQN)** algorithm to play the classic Pong game. The agent learns by interacting with the environment, improving its ability to hit the ball and score points. 

The agent is trained using **Prioritized Experience Replay (PER)**, an extension to standard experience replay that prioritizes more important experiences. In addition, the **reward function** has been shaped to encourage the agent to improve its paddle positioning and ball-hitting accuracy, leading to better performance over time.

## Project Features:
- **Pong Game**: The agent plays a variation of Pong where the left paddle is controlled by the RL agent, and the right paddle is controlled by a simple AI.
- **Deep Q-Network (DQN)**: Uses a neural network to approximate the Q-values for each state-action pair.
- **Prioritized Experience Replay (PER)**: Optimizes training by focusing on experiences with large TD-errors.
- **Shaped Reward Function**: Rewards the agent for hitting the ball accurately and keeping the paddle in an optimal position.
- **Exploration vs. Exploitation**: The agent uses epsilon-greedy action selection, gradually shifting from exploration to exploitation.


## Game Description:
In the Pong game, there are two paddles and a ball. The agent controls the left paddle, and the goal is to hit the ball back to the opponent (right paddle). The agent earns a reward when it successfully hits the ball or prevents the ball from going past it. The right paddle is controlled by a simple AI, which attempts to follow the ball’s position.



## Improvements:
1. **Shaped Reward Function**: The reward system is designed to encourage the agent to hit the ball accurately and maintain a good paddle position.
2. **Prioritized Experience Replay**: The agent samples experiences based on the temporal-difference error, focusing on the most critical experiences for learning.
3. **Epsilon Decay**: The exploration rate gradually decays over time, transitioning the agent from exploration to exploitation.
