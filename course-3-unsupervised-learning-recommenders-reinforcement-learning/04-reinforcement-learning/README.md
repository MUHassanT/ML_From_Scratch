# Reinforcement Learning: Tabular Q-Learning to DQN

Two implementations from Andrew Ng's ML Specialization (Course 3):

**Part A — Tabular Q-Learning (NumPy from scratch)**
Q-learning on a simple grid-world environment. Covers the Bellman equation, 
epsilon-greedy exploration, and Q-value convergence.

**Part B — Deep Q-Network (PyTorch)**
Scales up to Lunar Lander's continuous state space using a neural network as 
a function approximator. Implements experience replay and target networks 
from scratch; uses PyTorch for the network/backprop.

**Result:** DQN reached an average reward of ~189 over the last 100 episodes 
(600 total), close to the standard "solved" threshold of 200.

## References

- Andrew Ng, ML Specialization — Course 3 (DeepLearning.AI / Coursera)
- Mnih et al., "Playing Atari with Deep Reinforcement Learning" (2013)