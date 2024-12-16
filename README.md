# Flappy Bird Deep Q-Learning Agent

This repository contains an implementation of a Deep Q-Learning (DQN) agent that learns to play **Flappy Bird** in a Gymnasium environment. The project uses reinforcement learning techniques to train an agent to optimize its behavior in the game.

## Project Overview

This project involves training a **Deep Q-Learning Agent** to play **Flappy Bird** using the Gymnasium library, which is a toolkit for developing and comparing reinforcement learning agents. The agent learns to maximize the rewards from the game by interacting with the environment, trying different actions, and learning the optimal strategy over time.

### Main Techniques Used:

- **Deep Q-Learning (DQN):** Combines Q-learning with deep neural networks. A neural network is used to approximate the Q-function, which traditionally was stored in a table for small environments. DQN allows the agent to scale to much larger state spaces, like video games.
- **Experience Replay:** This technique stores past experiences (state, action, reward, next state) in a memory buffer and samples from this buffer to train the agent. It breaks correlations between consecutive samples, improving the training efficiency.
- **Target Networks:** DQN uses two networks - a policy network and a target network. The policy network chooses the actions, and the target network is used to calculate the Q-values for training.
- **Double DQN:** This variant of DQN addresses the problem of overestimation of Q-values. Double DQN uses a decoupled policy for action selection and target generation, which results in more stable and less biased updates.

## Environment Setup

Ensure you have Python installed (preferably Python 3.7 or higher) before setting up the environment.

### Install Required Libraries

Create a virtual environment and install the dependencies by running:

```bash
pip install -r requirements.txt
