# Advance_AI
Project
Aim:
This program employs the Q-Learning algorithm to tackle a reinforcement learning task within the OpenAI Gym environment.

During each of the 100,000 episodes of the primary loop, the agent selects an action using an epsilon-greedy policy. If a random number is less than the exploration rate (epsilon), the agent picks an action at random from the action space; otherwise, it chooses the action with the highest anticipated reward based on the Q-table. The Q-table is initialized with zeros and updated using the Bellman equation:

Q(s,a) = (1 - alpha) * Q(s,a) + alpha * (r + gamma * max(Q(s', a')))

Here, s represents the present state, a is the chosen action, s' denotes the next state, r is the reward, alpha is the learning rate, gamma is the discount factor, and max(Q(s', a')) is the highest anticipated reward for the next state.

The variables all_epochs and all_penalties are employed to log the number of steps and penalties (negative rewards) during each episode. These variables are then plotted using the matplotlib library once the training is completed.


This is a program that employs the Q-Learning algorithm to solve a reinforcement learning problem in the OpenAI Gym environment. The main loop runs for 100,000 episodes, and in each episode, the agent selects an action using an epsilon-greedy policy. If the random number is less than the exploration rate, the agent selects a random action; otherwise, it selects the action with the maximum expected reward from the Q-table. The Q-table is initialized with zeros, and its entries are updated using the Bellman equation. The variables all_epochs and all_penalties are used to record the number of steps and penalties for each episode, and they are plotted using matplotlib at the end of the training. The Q-table is initialized with zeros and updated using the Bellman equation:

Q(s,a) = (1 - alpha) * Q(s,a) + alpha * (r + gamma * max(Q(s', a')))

Here, s represents the present state, a is the chosen action, s' denotes the next state, r is the reward, alpha is the learning rate, gamma is the discount factor, and max(Q(s', a')) is the highest anticipated reward for the next state.

The variables all_epochs and all_penalties are employed to log the number of steps and penalties (negative rewards) during each episode. These variables are then plotted using the matplotlib library once the training is completed.

code evaluates the performance of an agent trained using Q-learning on an OpenAI Gym environment.

The code runs the agent for a specified number of episodes (in this case, 100) and computes the average number of timesteps and penalties (negative rewards) per episode. In each episode, the agent selects actions based on the learned Q-values and transitions to the next state according to the environment dynamics. If the agent receives a negative reward, it incurs a penalty.

The output of the code shows the average timesteps and penalties per episode for the evaluated agent.
https://github.com/nishank20/Advance_AI/blob/main/advance%20ai%20project.mov

The goal of my other project is to develop an intelligent system that can play Tic-Tac-Toe optimally using reinforcement learning. The project consists of two phases: the training phase, where two AI agents play against each other, and the test phase, where the trained AI model competes against a human player. The chosen approach is reinforcement learning, which consists of three components: State, Action, and Reward. The model is rewarded based on the action it takes in a given state. Thus, we first train the model and then evaluate its performance against a human player.





