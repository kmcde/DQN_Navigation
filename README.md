Project 1: Navigation

**Project Details**
Description - 
For this project, you will train an agent to navigate (and collect bananas!) in a large, square world.

Trained Agent

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

    0 - move forward.
    1 - move backward.
    2 - turn left.
    3 - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

**Getting Started**

All of the code is in PyTorch (v0.4) and Python 3. Additionally, the Unity ML-Agents Toolkit is used to keep track of the agents and the environment.

Step 1: Create (and activate) a new environment with Python 3.6.

    Linux or Mac:

conda create --name drlnd python=3.6
source activate drlnd

    Windows:

conda create --name drlnd python=3.6 
activate drlnd

Step 2: 
Install an older version of pytorch using conda

conda install pytorch==1.2.0 torchvision==0.4.0 -c pytorch

Step 3: 

Navigate to the included /python folder and install several dependancies 

git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .

Step 4:

Download the training environment from the Unity ML-Agents toolkit based on your operating system: 
https://github.com/udacity/deep-reinforcement-learning/tree/master/p1_navigation (see the 'getting started' section)

** Instructions **

The solution is in the Navigation.ipynb notebook.
Run all cells prior to the final cell to import libraries and to initialize the enviroment and agent.
The final cell will train the DQN using the supplied hyperparameters and stop after reaching the target average reward for the most recent 100 episode or reaching
the maximum number of episodes (whichever comes first). Additionally, a plot of the rewards by episode will be generated following the final episode.


** Files and Folders **

/python - includes requirements and dependancy-related files

model.py - contains the QNetwork class, which includes the structure of the underlying neural network

dqn_agent.py - contains the Agent and ReplayBuffer classes used in training and testing the DQN

Banana.x86_64 - contains the Linux version of the training environment from the Unity ML-Agents toolkit

Navigation.ipynb - trains and outputs result of the DQN agent

checkpoint.pth - weights of the DQN following task completion

Report.ipynb - provides a description of the implementation and results

