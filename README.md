# DQN-AgentNavigation
A Deep Q-Learning Network trained for solving an environment navigation problem in Unity

#### DQN Improvement Used
Double Q Network

### Environment Details

The goal of this environment is to train an agent to navigate and collect bananas in a large, square world.

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right. 


| Random agent             |  Trained agent |
:-------------------------:|:-------------------------:
![alt-text](https://github.com/convexalpha/DQN-AgentNavigation/blob/main/assets/randomagentgif.gif)  |  ![alt-text](https://github.com/convexalpha/DQN-AgentNavigation/blob/main/assets/samplegif.gif)  

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.


### Instructions

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file in this folder, unzip (or decompress) the file and then write the correct path in the argument for creating the environment under the notebook `Navigation.ipynb`:

```python
env = env = UnityEnvironment(file_name="Banana_Windows_x86_64/Banana.exe")

```
#### Required Dependencies:
    Python 3.6
    Unity Agents
    PyTorch
    Numpy
    Matplotlib
    Jupyter (Optional, python files are provided if you wish to run from command line)
    
## Running
Run the cells in the notebook `Navigation.ipynb` to train an agent that solves our required
task of collecting bananas.
