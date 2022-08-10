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
    - 'basic_scenario_PPO.ipynb' -- PPO model
    - 'basic_scenario_Duel_DQN.py' -- Dueling DQN model
    - 'basic_scenario_spectator_Duel_DQN.py' -- Imitation Learning using Dueling DQN model

- One log file of our group meetings: 'Group_meeting_logs.md', where we recorded the process of how we organize our project. 

### 3. How to run the code
- Load trained best model:
    - PPO: ```model.load('best_model/PPO_best_model_60000.zip')```
    - Dueling DQN: ```model.load('best_model/Duel_DQN_basic_scenario_best_model.pth')```
    - Imitation Learning using Dueling DQN: ```model.load(best_model/Spectator_Training_best_model.pth)```

## Other Explanations
- Dueling DQN model used (30,45) resolution, while PPO model is trained on (160,100) resolution

- Test Results for Spectator trained models: (Explanation to the Tensorboard file names)
    - P = Pre-Training epochs
    - S = Spectator Training epochs
    - N = Normal Training epochs

- If there is something wrong with loading the stored best model of 'best_model/PPO_best_model_60000.zip', there is a backup GoogleDrive link on Cornor's Google Drive: https://drive.google.com/file/d/1Pn1TMUw5bGvsFw_Ge_KQ9tImQm2ySZFb/view?usp=sharing

## Learning Materials
- ### Tutorials:
    - [Bilibili:【莫烦Python】强化学习 Reinforcement Learning](https://www.bilibili.com/video/BV13W411Y75P?p=31&vd_source=4e20016bd1355fe9ad9e32194a97d42a)
    - [莫烦official web: reinforcement learning](https://mofanpy.com/tutorials/machine-learning/reinforcement-learning/)

- ### Articles:
    - [Q-Learning vs. Dynamic Programming](https://www.baeldung.com/cs/q-learning-vs-dynamic-programming)
    - [Bellman Equation and dynamic programming](https://medium.com/analytics-vidhya/bellman-equation-and-dynamic-programming-773ce67fc6a7)