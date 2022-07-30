# VizDoom_Deep_RL

## Introduction

ViZDoom is an AI research platform based on the classical First Person Shooter game Doom. This repo is used to learn Deep_RL. Environment is VIZDoom video shooting game. The framework is PyTorch.
ViZDoom allows developing AI bots that play Doom using only the visual information (the screen buffer). It is primarily intended for research in machine visual learning, and deep reinforcement learning in particular.
In this project, we are mentioned about four algorithms, i.e., PPO(Proximal Policy Optimization algorithm), DQN(deep Q-network), Double Q(Deep Weighted Q-Learning algorithm/Weighted DQN), and spectator related algorithm, and figure out which algorithm is the most suitable method for performing deep reinforcement learning about VizDoom.

## instructions

### 1. How to run the code
- Duel DQN
    1. 

- PPO 
    1. run trained best model:
        ```model.load('best_model/PPO_best_model_60000.zip')```

#### The structure of the folders

### 2. requirements

The requirement about PPO is already included in the .ipynb file; Need to install pytorch, tensorboard, ... as the precondition.



## Others/Extra
PPO_best_model_60000_GoogleDrive_link on Cornor's Google Drive: https://drive.google.com/file/d/1Pn1TMUw5bGvsFw_Ge_KQ9tImQm2ySZFb/view?usp=sharing 


## Explanation
- basic_scenario_spectator_Duel_DQN and basic_scenario_Duel_DQN is trained on (30,45) resolution, while basic_scenario_PPO is trained on (160,100) resolution

- Test Results for Spectator trained models: (Tensorboard file names)
    - P = Pre-Training epochs
    - S = Spectator Training epochs
    - N = Normal Training epochs
