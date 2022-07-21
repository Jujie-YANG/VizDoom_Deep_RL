# Weekly Group Meeting(GM) Logs

Below are logs of group meetings.

## Summary 7.5 GM1:

1. 7号周四 北京时间21:00-22:00 英国时间14:00-15:00 美国时间9:00-10:00 先去office hour问问TA 然后看看有没有什么新启发
2. 7号周四 北京时间22:00-23:00 英国时间15:00-16:00 美国时间10:00-11:00 小组zoom会议
3. 周四会议前 大家去网上找找Deep_RL开源的代码 好做的小项目 然后发群里 供大家参考 以便这周四集中讨论

## Summary 7.7 GM2:

1. Environment定为VizDoom 使用Pytorch 大家自己先玩玩～
2. 下一次Meeting定为 7.12下周二 北京时间21:00-22:00 英国时间14:00-15:00 美国时间9:00-10:00

## Summary 7.12 GM3:

### Task Allocation：

- Ludens:
  1. Take his own jobs regarding behavioral cloning
- The other three:
  1. Watch this [Youtube tutorial](https://www.youtube.com/watch?v=eBCU-tqLGfQ&t=9491s&ab_channel=NicholasRenotte) using PPO algorithm on first three scenarios (Basic, Corridor, Centre)

     **Note: Once you have already watched this tutorial before this Saturday, please speak up on WeChat and provide any ideas and thoughts!**
  2. Search for any materials on which algorithms included are directly implemented on VizDoom environment and then post links you found on WeChat for others to see and discuss on

### Scheduled time for next GM：

7.16 This Saturday (right after lecture) 北京时间18:00-19:30 英国时间11:00-12:30 美国时间6:00-7:30

## Summary 7.16 GM4:

### Work Progress

- Ludens:

    Mainly met two problems so far:

    1. 鼠标键盘人工操作游戏 出现严重卡顿，导致无法正常记录expert behaviors
    2. 训练结果停留原地 (probably due to high level difficulty of the chosen scenario)

    Corresponding possible solutions:

    1. Use command lines to operate the game
    2. Try basic scenario first (Or similarly, degrade the difficulty level of your chosen scenario)

- The other three:

    1. Already found some algorithms implemented on VizDoom
    2. Next urgent step is to run them all on our own and **ensure the results will be convergent**
    3. Following that, consider some metrics we can analysis to better accomplish our group report (Please refer to [our group report on LaTex](https://www.overleaf.com/project/62d29bef88402034435591ec))


### Scheduled time for next GM：
7.21 Next Thursday 北京时间19:00-20:00 英国时间12:00-13:00 美国时间7:00-8:00


## Summary 7.21 GM5:
### Work Progress:
- Ludens:
  1. 现有的模型跑得很成功，很快收敛
  
- Others:
  1. Mainly focus on implementing three algorithms ([PPO](https://www.youtube.com/watch?v=eBCU-tqLGfQ&t=9491s), [Double Q](https://github.com/boubnanm/Deep-Reinforcement-Learning-applied-to-DOOM) and [DQN in the official website](https://github.com/mwydmuch/ViZDoom/blob/master/examples/python/learning_pytorch.py)) in the basic scenario 
  2. Give up other algorithms

### Next Step:
- Ludens:
  1. 加上tensorboard，看一下有什么metric可以与其它三个基础algorithms对比 (Tensorboard 能多display params就多加一些params，到时候好和Cornor跑的对比)
  2. Record a video (and better convert to a gif) of 20 episodes running on the trained saved model 

- Others:
  1. 简化algorithms that run very slowly (Ludens can give any suggestions on how to simplify those two algorithms([Double Q](https://github.com/boubnanm/Deep-Reinforcement-Learning-applied-to-DOOM) and [DQN in the official website](https://github.com/mwydmuch/ViZDoom/blob/master/examples/python/learning_pytorch.py)) regarding the specific code. Ludens给的建议很好，有可能是模型太大，用在basic这个scenario有点大材小用，比如可能层数太多，跑得很慢)
  2. Increase the training episodes of Double Q to 100,000 (100k) (If the result is still not going well)
  3. add a tensorboard for the DQN algorithm and then retrain DQN (Tensorboard 能多display params就多加一些params，到时候好和Ludens跑的对比)
  4. Record three videos (and better convert to gif(s)) of 20 episodes running on three trained model

  5. Extra Work: (Compare the performance of PPO algorithms based on different params)
      1. learning rate (lr): 0.001, 0.0001 and 0.00001
      2. resolution: 320*240 -> 45*30? (160,120 1280*720) - [Check available RES here](https://github.com/mwydmuch/ViZDoom/blob/0e6d1ad9bc6b4d0b5b5b2dcc8f540a7c34863515/src/lib/ViZDoomGame.cpp)
      3. Any other params if possible?


### Scheduled time for next GM：
7.22 This Friday 北京时间19:00-20:00 英国时间12:00-13:00 美国时间7:00-8:00