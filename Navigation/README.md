[//]: # (Image References)

[image1]: /report/videos/readme_gif1.gif "Own Trained Agent"

# Project 1: Navigation

### Introduction

In this project an agent navigate (and collect bananas!) in a square enviroment.  

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. The goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, the agent must get an average score of +13 over 100 consecutive episodes.


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

3. Open your Jupyter Notebook, open the Navigation.ipynb file and select the apropiate kernel (ml-agents).

4. Follow the instructions in `Navigation.ipynb` and Run the cells for Train or Play the Agent and enviroment



### Run the Code

For run the code you can take 3 ways :

1. wiew the enviroment simulation with a basic  Agent with random behavior, play code cells asociated with Markdown ones named:

- 1. Start the Environment
- 2. Examine the State and Action Spaces
- 3. Take Random Actions in the Environment

2 Train the Agent:

- 1. Start the Environment
- 2. Examine the State and Action Spaces
- 3. Solve: Train the Agent with DQN

3 Play a Trained Agent:

- 1. Start the Environment
- 2. Examine the State and Action Spaces
- 3. Solve: Train the Agent with DQN (only the first below cell where the agent is created)
- 4. Watch a Smart Agent!





### (Optional) Challenge: Learning from Pixels

If you're looking for an additional challenge, you have come to the right place!  In the project, the agent learned from information such as its velocity, along with ray-based perception of objects around its forward direction.  A more challenging task would be to learn directly from pixels!

To solve this harder task, you'll need to download a new Unity environment.  This environment is almost identical to the project environment, where the only difference is that the state is an 84 x 84 RGB image, corresponding to the agent's first-person view.  (**Note**: Udacity students should not submit a project with this new environment.)

You need only select the environment that matches your operating system:
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana_Windows_x86_64.zip)

Then, place the file in the `p1_navigation/` folder in the DRLND GitHub repository, and unzip (or decompress) the file.  Next, open `Navigation_Pixels.ipynb` and follow the instructions to learn how to use the Python API to control the agent.

(_For AWS_) If you'd like to train the agent on AWS, you must follow the instructions to [set up X Server](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above.
