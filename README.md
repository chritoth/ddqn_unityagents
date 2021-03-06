[//]: # (Image References)

[image1]: img/trained_agent.gif "Trained Agent"

# Learning to collect bananas

### Project Overview

In this project we train an agent to pick up yellow bananas that are scattered throughout a square world. The agent
 must learn to navigate in its environment to reach yellow bananas (reward of +1 each) while avoiding to collect
 blue bananas (reward of -1 each). To solve this problem we employ the [Double Deep Q-Learning](https://www.aaai.org/ocs/index.php/AAAI/AAAI16/paper/viewPaper/12389) (DDQN) algorithm [1].
We describe our solution [here](report.pdf). 


![Trained Agent][image1]

## Environment Description

The agent can use four discrete actions in order to move within the environment, which are:
 move forward,
 - **`0`** - move forward.
 - **`1`** - move backward.
 - **`2`** - turn left.
 - **`3`** - turn right.

The state information contains the agent's velocity, as well as a ray-based representation of objects around it. The
 state space spans 37 dimensions.
 
To solve this environment, the agent has to get an average score of +13 across 100 consecutive episodes.

### Dependencies

Running the code in this repository requires a working Python 3.6 environment along with the packages *numpy*, *scipy
*, *matplotlib*, *pytorch*, and *unityagents*. One way to set up a proper environment is by following the
 instructions provided [here](https://github.com/udacity/deep-reinforcement-learning#dependencies).

Furthermore, the unity environment must be downloaded. The path to the unpacked environment folder must be updated
 accordingly in `Navigation_DDQN.ipynb`. Please refer to [this repository](https://github.com/udacity/deep-reinforcement-learning/tree/master/p1_navigation#getting-started) for download links and instructions.

### Instructions

Follow the instructions in `Navigation_DDQN.ipynb` to train an agent from scratch or simply watch a pretrained agent
 doing its job!

### References
[1] Van Hasselt, Hado, Arthur Guez, and David Silver. "Deep reinforcement learning with double q-learning." Thirtieth AAAI conference on artificial intelligence. 2016.
