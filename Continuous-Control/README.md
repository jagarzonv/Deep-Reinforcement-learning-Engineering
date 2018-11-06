[//]: # (Image References)

[image1]: /report/videos/cc_1.gif  "One Trained Agent"
[image2]: /report/videos/cc_20.gif "Twenty Trained Agents"

# Project 2: Continuous Control

### Introduction

In this project agent is a two link arm wich end effector will be track an sphericall objetive in the space. The enviroment has two versions, first with one agent and the other one with 20 agents 

![Trained Algorithm with One Agent][image1]

![Trained Algorithm with Twenty Agents][image2]

A reward of + 0.01 is provided when a end effector reach a moving spherical volume in the space. A 0 reward is provided for end effector out of sphere volume.The goal of the agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. 

The state space has 33 dimensions and contains the agent's arm  velocity, angular velocities, position and rotation.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to torque applicable to two joints, Every entry in the action vector should be a number betwen -1 and +1 


The task is episodic, the agent must get an average score of +30 over 100 consecutive episodes.


### Getting Started

1. For run and explore the code firs preare your enviroment, in this case I use a local machine with Windows 10 OS with CORE i7 processor and Nvidia 960M GPU:

Download and install Anacoda for Windows 64-Bit and Python 3:
    - Anaconda: [click here](https://conda.io/docs/user-guide/install/windows.html)
Create a virtual enviroment with python 3.6 (I create a conda enviroment named ml-agents) and activate (all equirements will be installed inside the enviroment)
    - Anaconda enviroments: [click here](https://conda.io/docs/user-guide/tasks/manage-environments.html)
Download the repo of Unity ML-Agents Toolkit at:   
    - Unity ML-Agents Toolkit: [click here](https://github.com/Unity-Technologies/ml-agents)
and follow the install instructions (for example I create a conda enviroment named ml-agents):     
    - install: [click here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md)
Aditionally the project requeriments include Pytorch to train the Agent , save weights and run the enviroment with the agent actions, select and install.(if you dont have pip3 , pip also works )    
    - In my case Pytorch for Windows (64-bit) , PIP, python 3.6 and cuda 9 : [click here](https://pytorch.org/)
    - pip install torchvision is not necessary.
     
    
2. Clone or download this GitHub repository in your machine and unzip (or decompress) the file. 

3. Open your Jupyter Notebook, open the Continuous_Control.ipynb file and select the apropiate kernel (ml-agents).

4. Follow the instructions in `Continuous_Control.ipynb` and Run the cells for Train or Play the Agent and enviroment



### Run the Code

For run the code you can take 3 ways :

1 View the enviroment simulation with a basic  Agent with random behavior, play code cells asociated with Markdown ones named:

- 1. Start the Environment and Select the Enviroment for 1 agent or 20 agents
- 2. Examine the State and Action Spaces
- 3. Take Random Actions in the Environment

2 Train the Agent:

- 1. Start the Environment and Select the Enviroment for 1 agent or 20 agents
- 2. Examine the State and Action Spaces
- 3. Solve: Train the Agent with DDPG

3 Play a Trained Agent:

- 1. Start the Environment and Select the Enviroment for 1 agent or 20 agents
- 2. Examine the State and Action Spaces
- 3. Solve: Train the Agent with DDPG (only the first below cell where the agent is created)
- 4. Watch a Smart Agent! , you can load the trained model weights from weights folder , for one agent you should select checkpoint_actor_1.pth and checkpoint_critic_1.pth,  for 20 agents model select checkpoint_actor_20.pth and checkpoint_critic_20.pth


#### Resolve criteria

Option 1: Solve the One Agent Version
The task is episodic, and in order to solve the environment, your agent must get an average score of +30 over 100 consecutive episodes.

Option 2: Solve the Twenty Agents Version
The barrier for solving the second version of the environment is slightly different, to take into account the presence of many agents. In particular, your agents must get an average score of +30 (over 100 consecutive episodes, and over all agents)

#### Show the results


The performance of agent can see in youtube!, with one agent  [click here](https://youtu.be/laqf43ojRk4) , and for 20 agents   [click here](https://youtu.be/8D0T21vAAus)




### (Optional) Challenge: Crawl

After you have successfully completed the project, you might like to solve a more difficult continuous control environment, where the goal is to teach a creature with four legs to walk forward without falling.

Download the Unity Environment
To solve this harder task, you'll need to download a new Unity environment. You need only select the environment that matches your operating system.

Please do not submit a project with this new environment. You are required to complete the project with the Reacher environment that was provided earlier in this lesson, in The Environment - Explore.

(For AWS) If you'd like to train the agent on AWS (and have not enabled a virtual screen), then please use this link to obtain the "headless" version of the environment. You will not be able to watch the agent without enabling a virtual screen, but you will be able to train the agent. (To watch the agent, you should follow the instructions to enable a virtual screen, and then download the environment for the Linux operating system above.)