![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

## ALE/Pong-v5 with DQN

[![ru](https://img.shields.io/badge/README_на_русском-2A2C39?style=for-the-badge&logo=github&logoColor=white)](README.ru.md)  

This code uses a training environment such as **ALE/Pong-v5**. A neural network architecture based on fully connected layers is implemented, and the classes `NNModel` and `DQN` are defined to implement the prediction and target networks, the replay buffer, the ε-greedy strategy, weight synchronization, and the learning step. The agent's training cycle with the ε-greedy strategy and gradual reduction of ε is implemented, as well as a graph showing the reward dynamics over episodes.

Let's understand the basic concepts of the code:

**ε-greedy strategy (epsilon-greedy)** is a method of balancing between exploration and exploitation in reinforcement learning. Before each action, the agent chooses a random action to explore the environment with a probability of ε (e.g., 10%), and chooses the best known action to maximize the current reward with a probability of (1-ε). Thus, the single parameter ε sets a simple and effective trade-off between learning new things and exploiting what is known.

**DQN (Deep Q-Network)** is a hybrid method that trains a deep neural network to predict future rewards (Q-values) for different actions, allowing the agent to make effective decisions based on complex input data, such as game pixels. Its key idea is to stabilize unstable learning by using **experience replay** (random sampling from memory) and **target network** (a separate network for calculating reference values).

The final part of the notebook provides an analysis of the agent's behavior and an output.

> I strongly recommend running the code in **Google Colab** with
> the use of **T4 GPU**!

<div  align="center">

![enter image description here](https://ale.farama.org/_images/pong.gif)

</div>