[//]: # (Image References)

[image1]: /report/videos/tennis.gif "Collab-Compet-Agents"



# Project 3: Collaboration and Competition

### Introduction

For this project, you will work with the [Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) environment.

![Trained Agent][image1]

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1.  If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01.  Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation.  Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. 


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

3. Open your Jupyter Notebook, open the Tennis.ipynb file and select the apropiate kernel (ml-agents).

4. Follow the instructions in `Tennis.ipynb` and Run the cells for Train or Play the Agent and enviroment



### Run the Code

For run the code you can take 3 ways :

1 View the enviroment simulation with a basic  Agents with random behavior, play code cells asociated with Markdown ones named:

- 1. Start the Environment
- 2. Examine the State and Action Spaces
- 3. Take Random Actions in the Environment

2 Train the Agent:

- 1. Start the Environment
- 2. Examine the State and Action Spaces
- 3. Solve: Train the Agent with DDPG

3 Play a Trained Agent:

- 1. Start the Environment
- 2. Examine the State and Action Spaces
- 3. Solve: Train the Agent with DDPG (only the first below cell where the agent is created)
- 4. Watch a Smart Agent! , you can load the trained model weights from weights folder ,select checkpoint_actor.pth and checkpoint_critic.pth


#### Resolve criteria

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

- After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
- This yields a single **score** for each episode.

The environment is considered solved, when the average (over 100 episodes) of those **scores** is at least +0.5.

For this project solution the average (over 100 episodes) of those scores is configured as 0.9 

#### Show the results


The performance of agents can see in youtube!, with one agent  [click here](https://www.youtube.com/watch?v=yaGT9DuBclI)



### (Optional) Challenge: Play Soccer

After you have successfully completed the project, you might like to solve the more difficult **Soccer** environment.

![Soccer][image2]

In this environment, the goal is to train a team of agents to play soccer.  

You can read more about this environment in the ML-Agents GitHub [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#soccer-twos).  To solve this harder task, you'll need to download a new Unity environment.  (**Note**: Udacity students should not submit a project with this new environment.)

You need only select the environment that matches your operating system:
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Soccer/Soccer_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Soccer/Soccer.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Soccer/Soccer_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Soccer/Soccer_Windows_x86_64.zip)

Then, place the file in the `p3_collab-compet/` folder in the DRLND GitHub repository, and unzip (or decompress) the file.  Next, open `Soccer.ipynb` and follow the instructions to learn how to use the Python API to control the agent.

(_For AWS_) If you'd like to train the agents on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Soccer/Soccer_Linux_NoVis.zip) to obtain the "headless" version of the environment.  You will **not** be able to watch the agents without enabling a virtual screen, but you will be able to train the agents.  (_To watch the agents, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)
