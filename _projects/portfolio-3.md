---
title: "Comparison of Atari RL Pruning Algorithms"
excerpt: "DQN vs. PPO and Sparsity Levels <br/><img src='/images/atari.gif'>"
collection: projects
---

Investigated a single-step, midway training pruning strategy to enhance the efficiency of reinforcement learning models applied to Space Invaders. Systematically compared no pruning, random unstructured pruning, and L1 unstructured pruning across two distinct algorithms, Proximal Policy Optimization (PPO) and Deep Q-Networks (DQN), with pruning rates up to 80%. The results, evaluated primarily by mean episodic return, demonstrated that pruning had a minimal impact on final performance, suggesting that a significant portion of network weights are non-essential and can be removed for efficiency gains without a large performance cost.

[Report Link](https://drive.google.com/file/d/19SaqYqnkqWqxAV2lxkQ6414x156vN32J/view?usp=sharing)
