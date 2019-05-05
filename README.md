[//]: # (Image References)

[image1]: https://github.com/GeraudMM/Collab_Compet-with-D.R.L./blob/master/firstPage.PNG

# Collab-Compet with Deep Reinforcement Learning
In this project, we are teaching a DDPG agent to play tennis against himself in a Unity environment.

![Agent playing][image1]

# Continuous Control with Deep Reinforcement Learning

For this project, we work with the Tennis environment. The goal is to implement a deep reinforcement learning algorithm that can deal with continuous action space and multi-agent training.


### Environment
In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
This yields a single score for each episode.
The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.

### Files
The `model.py` and `ddpg_agent.py` files are from the folder on ddpg-pendulum made by Udacity.

The `Tenis.ipynb` notebook is the part where we can train and watch a "smart" agent evolving in the Unity environment.

The `checkpoint_actor.pth` and `checkpoint_critic.pth` files are saving of the weights of the locals actor and critic. Those can be downloaded to watch a "smart" agent.

The 'Report.pdf' file explains how the algorithm works and contains different training examples.

### Getting Started
1. Set up the Python environment:

    Follow the instructions in the Udacity [DRLND Github repository](https://github.com/udacity/deep-reinforcement-learning/#dependencies) to set up the Python environment. 

2. Download the Unity environment from one of the links below that matches your operating system:

    - **_Tenis Environment_**
      - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
      - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
      - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
      - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)
      - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux_NoVis.zip) NO Visual version

    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) (version 1) or [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) (version 2) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

2. Place the file in the DRLND GitHub repository, in the `Collab-Compet-with-D.R.L./` folder, and unzip (or decompress) the file. 

### Instruction
Follow the instruction in the `Tennis.ipynb` notebook to begin the training of the DDPG Agent. 
Check also the `Report.pdf` for explaination on the algorithm.
