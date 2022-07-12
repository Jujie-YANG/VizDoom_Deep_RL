# DQN with Pytorch

## Materials
- [Deep Q-Network with Pytorch](https://unnatsingh.medium.com/deep-q-network-with-pytorch-d1ca6f40bfda)

- [Schooling Flappy Bird: A Reinforcement Learning Tutorial](https://www.toptal.com/deep-learning/pytorch-reinforcement-learning-tutorial). And its corresponding full code is [here](https://github.com/nevenp/dqn_flappy_bird).



## Possible Methods (Mainly compare various performance)
- ### Policy comparison
    - BlotzmannQPolicy vs EpsGreedyQPolicy

- ### Hyperparameter optimization

- ### Neural Network architecture 
    - Number of Layers

    - Optimizers (SGD vs Adam under Deep_RL): One interesting and dominant argument about optimizers is that SGD better generalizes than Adam. These papers argue that although Adam converges faster, SGD generalizes better than Adam and thus results in improved final performance.

    - Activation Function? (It is meaningless to change activation function.): ReLU activation function is widely used and is default choice as it yields better results. If we encounter a case of dead neurons in our networks the leaky ReLU function is the best choice. ReLU function should only be used in the hidden layers. 

- ### Algorithms (value-based vs policy based vs imitation?)
    ![rl_algorithms1](./src/rl_algorithms1.png)
    <img src="./src/rl_algorithms2.png" alt="rl_algorithms2" width=50%/>
    <img src="./src/rl_algorithms3.png" alt="rl_algorithms3" width=49%/>
    <!-- ![rl_algorithms2](./src/rl_algorithms2.png)
    ![rl_algorithms3](./src/rl_algorithms3.png) -->
