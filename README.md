# VizDoom_Deep_RL
##Introduction
ViZDoom is an AI research platform based on the classical First Person Shooter game Doom. This repo is used to learn Deep_RL. Environment is VIZDoom video shooting game. The framework is PyTorch. 

## Notes
- https://github.com/mwydmuch/ViZDoom/blob/master/scenarios/README.md 

## Basic Environment
REWARDS:
killing the monster = +101
miss shooting the monster (waste ammo) = -5
living (every move) = -1

### Steps
1. Getting VizDoom Up and Running
2. Converting it to a Gym Environment
    
    Pre-processing:

    - Wrap our framework or wrap our vizdoom enviroment inside of the openAI gym framework: In order to ai the game, we are going to need to get it into an open-ai gym environment. We can wrap it inside the environment using the openAI gym base class. This will give us a bunch more flexibility when it comes to pre-processing and working with the game frames and rewards.

    - grayscale the game observations and cut out the game info bar at the bottom, which can help train the model faster as there are less pixels to process. (Use OpenCV to process image)

    - non rendered environment

3. View Game State
4. Setup Callback
PPO: pip install stable-baselines3[extra] mroe info to see [website]()
5. Train Model


- PPO: why always use MSE loss? Cross-entropy loss, or log loss, measure the performance of a classification model whose output is a probability value between 0 and 1. It is preferred for classification, while mean squared error (MSE) is one of the best choices for regression. This comes directly from the statement of your problems itself.

- Gym removed GoalEnv many releases ago. SB3 is still using a very old version of Gym, the PR to bump it is here: DLR-RM/stable-baselines3#780

- tensorboard: If you see approx_kl function and policy_gradient_loss going to almost zero really really quickly, that's an indicator that your model isn't actually learning all that well and it's effectively just taking the same action every single time. It also indicates that there's no divergence from the previous policy to the current policy(mainly looking at the approx_kl function). -- then we need to change hyper parameters like n_step(batch_size) 256 -> 2048 to effectively get better training (we shouldn't see episode reward mean just tank and stableize there. It should effectively flutuate a little bit and you definitely shouldn't be seeing the policy gradient loss is trending towards zero)

cd PPO_n
tensorboard --logdir=.

- approx_kl: this is a metric of how different our old policy is from or how different our new policy is from the old policy so you want to see this graph increases and then comes back down. And if you increase too much, it's going to get clipped so you can see that clip fraction is increasing up there

- reward mean increase: very good 

- explained_variance: value:0.7738 which is good sign which means that our critic is able to accurately or closer to accurately predict what the future sum of returns is going to be given the current state in action

- policy_gradient_loss is sort of fluctuated and you can see that it's increased as value_loss decrease: good sign. Because our critic is better able to predict its discount of future sum of rewards and the ability to determine advantage is decreasing

6. Test the Model


## Defend the center 
More info, refer to https://github.com/mwydmuch/ViZDoom/blob/master/scenarios/README.md 
