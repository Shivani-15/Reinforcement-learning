# Reinforcement Learning Algorithms for Gaming Environments

This repository contains implementations of various reinforcement learning algorithms applied to different gaming environments. The algorithms implemented here are Deep Q-Network (DQN) and Double Deep Q-Network (DDQN) for the Atari Breakout environment, and Policy Gradient, Policy Gradient with Reward-to-Go, and Policy Gradient with Baseline for the Cart Pole environment.

## Atari Breakout Environment

### Deep Q-Network (DQN)

Deep Q-Network is a popular off-policy reinforcement learning algorithm used for training agents in discrete action spaces. In this implementation, we use DQN to train an agent to play the Atari Breakout game. The agent learns to predict Q-values for each action and uses an experience replay buffer to stabilize and improve training.

### Double Deep Q-Network (DDQN)

Double Deep Q-Network is an improvement over the original DQN algorithm that addresses the overestimation bias issue in Q-value estimation. It uses two sets of network parameters to decouple the action selection and Q-value estimation, leading to more stable and accurate training. We apply the DDQN algorithm to the Atari Breakout environment to demonstrate its effectiveness.

## Cart Pole Environment

### Policy Gradient

Policy Gradient is an on-policy reinforcement learning algorithm used for training agents in both discrete and continuous action spaces. In this implementation, we use Policy Gradient to train an agent to balance a pole on a cart in the Cart Pole environment. The agent directly learns a policy to map states to actions through gradient ascent on expected rewards.

### Policy Gradient with Reward-to-Go

Policy Gradient with Reward-to-Go is an extension of the original Policy Gradient algorithm. Instead of using the total discounted rewards, this variant uses reward-to-go, which is the sum of future rewards starting from the current time step. This modification often leads to better convergence and performance in episodic environments. We apply this algorithm to the Cart Pole environment to showcase its advantages.

### Policy Gradient with Baseline

Policy Gradient with Baseline is another variation of the original Policy Gradient algorithm. It introduces a learned baseline function to reduce the variance of policy gradients and improve training stability. By subtracting the baseline from the total rewards, the algorithm focuses on the advantage of each action, leading to more efficient learning. We implement this algorithm in the Cart Pole environment to observe its benefits.

## Requirements

To run the notebooks and experiments in this repository, you will need the following dependencies:

- Python 3.x
- Jupyter Notebook
- OpenAI Gym
- PyTorch
- NumPy
- Matplotlib

Please refer to the individual notebooks for more details on how to install and set up the required libraries.

## How to Use

To get started with using the implementations, follow these steps:

1. Clone the repository to your local machine:

```
git clone https://github.com/your-username/your-repo.git
```

2. Navigate to the directory:

```
cd your-repo
```

3. Open the Jupyter Notebook environment:

```
jupyter notebook
```

4. Access the respective notebooks for the algorithms you are interested in:

   - `dqn_atari_breakout.ipynb`
   - `ddqn_atari_breakout.ipynb`
   - `policy_gradient_cart_pole.ipynb`
   - `policy_gradient_reward_to_go_cart_pole.ipynb`
   - `policy_gradient_baseline_cart_pole.ipynb`


