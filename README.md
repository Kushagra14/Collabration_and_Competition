# Tennis (Collabration_and_Competition)

In this project Reinforcement Learning agent will Continously Reach the ball . Below is the snapshot of the game:

![Tennis](images/tennis.gif)


### Description
In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, agents get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,
After each episode, adding the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. This project takes the maximum of these 2 scores.
    This yields a single score for each episode.

The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.


### Dependencies
1. Python 3
2. Pytorch
3. Jupyter-notebook
4. Untiy Environment

### Setting up the environment

The environment can be downloaded from one of the links below for all operating systems

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)
- _For AWS_: To train the agent on AWS (without [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) to obtain the "headless" version of the environment.  The agent can **not** be watched without enabling a virtual screen, but can be trained.  (_To watch the agent, one can follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

### Installation Guide
1. Clone this repository on your local machine
   ```git clone https://github.com/Kushagra14/Collabration_and_Competition.git```
2. Open the project using jupyter-notebook
3. [Shift + Ent] to execute every cell. This particular code will start learning neural network and will run one episode in backgorund
4. You can also load the weights provided in this repositroy using code below:
   ```device = torch.device('cpu')
      model = TheModelClass(*args, **kwargs)
      model.load_state_dict(torch.load(PATH, map_location=device))

    ```
    [Using pytorch to load weights in your algorithm](https://pytorch.org/tutorials/beginner/saving_loading_models.html)
    

