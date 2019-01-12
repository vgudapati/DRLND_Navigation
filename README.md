[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"
[image2]: https://cdn-images-1.medium.com/max/1200/1*8b_wJNn0tC_7t6T7ID_OUQ.png "Rainbow"

# Project 1: Navigation

## Project Details

### Introduction

The objective of this project is to train an agent to navigate (and collect bananas!) in a large, square world.  

![Trained Agent][image1]

### Rewards
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  The goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

### State Space

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

### Solution Criteria

The task is episodic. The environment is considered solved when the agent gets an average score of +13 over 100 consecutive episodes.

## Getting Started

### Setup
1. Clone the repository from https://github.com/vgudapati/DRLND_Navigation.git

2. Setup the dependencies as described [here](https://github.com/udacity/deep-reinforcement-learning/blob/master/README.md).

3. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
4. Place the file in the DRLND GitHub repository, in the `DRLND_Navigation/` folder, and unzip (or decompress) the file.
 

### Instructions

Follow the instructions in `Navigation.ipynb` to train the agent and see the results!   

## Future work - improving agent's performance

The DQN implementation can be improved several ways for better performance.
1. One of the most effective so far I have seen is the rainbow algorithm as mentioned in the rainbow paper (https://arxiv.org/pdf/1710.02298.pdf). We can try individual algorithms. But the most effective one is the rainbow.

![Rainbow][image2]
2. Additionally, we can use systematic ways of tuning the neural network hyperparameters (such as learning rate) and their loss functions and optimizers and the network architectures themselves.

