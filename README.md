# Teach AI to Play Video Games through Imitation Learning: Deep Reinforcement Learning on ViZDoom

## Abstract
Reinforcement learning is an area of machine learning concerned with how intelligent agents ought to take actions in an environment in order to maximize the notion of cumulative reward. In environments where rewards are sparse, manual methods are necessary. However, manually designing a reward function that satisfies the desired behavior can be very complicated. A useful solution is Imitation Learning (IL). This report proposes two reinforcement learning algorithms used on basic scenarios of ViZDoom video game and leverage IL to improve the performance of one of the model(Dueling DQN).

## Introduction
### Environment
In this project, we chose the basic scenario of ViZDoom as the experiment environment. 

ViZDoom is an AI research platform based on the classical First Person Shooter game Doom. ViZDoom allows developing AI bots that play Doom using only the visual information (the screen buffer). It is primarily intended for research in machine visual learning, and deep reinforcement learning in particular. More information about ViZDoom can be found on [the official website](http://vizdoom.cs.put.edu.pl/) and [its corresponding GitHub](https://github.com/mwydmuch/ViZDoom).
### Framework
PyTorch and we used Tensorboard on Tensorflow to observe the results

### Two experiments (Models/Algorithms)
- PPO
- Dueling DQN

## Instructions
### 1. Requirements:
- Successfully install all packages that are used in each running file, including ViZDoom, PyTorch, Tensorboard. For the instruction of how to install ViZDoom, please see [the official GitHub repo](https://github.com/mwydmuch/ViZDoom)

### 2. The structure of the folders
- Three main running files:
    - 'basic_scenario_PPO.ipynb' PPO model
    - 'basic_scenario_Duel_DQN.py' Dueling DQN model
    - 'basic_scenario_spectator_Duel_DQN.py' Imitation Learning using Dueling DQN model

- One log file of our group meetings: 'Group_meeting_logs.md'



### 3. How to run the code

- Duel DQN
    1. 

- PPO 
    1. run trained best model:
        ```model.load('best_model/PPO_best_model_60000.zip')```




## Other Explanations
- PPO_best_model_60000_GoogleDrive_link on Cornor's Google Drive: https://drive.google.com/file/d/1Pn1TMUw5bGvsFw_Ge_KQ9tImQm2ySZFb/view?usp=sharing 



- basic_scenario_spectator_Duel_DQN and basic_scenario_Duel_DQN is trained on (30,45) resolution, while basic_scenario_PPO is trained on (160,100) resolution

- Test Results for Spectator trained models: (Tensorboard file names)
    - P = Pre-Training epochs
    - S = Spectator Training epochs
    - N = Normal Training epochs


[How to teach AI to play Games: Deep Reinforcement Learning](https://towardsdatascience.com/how-to-teach-an-ai-to-play-games-deep-reinforcement-learning-28f9b920440a)