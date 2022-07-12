# Possible project directions and corresponding materials

## YOLOv5
These tutorials all show how to perform an end-to-end object detection project on a custom dataset using YOLOv5 
- [The practical guide for Object Detection with YOLOv5 algorithm](https://towardsdatascience.com/the-practical-guide-for-object-detection-with-yolov5-algorithm-74c04aac4843)

- [YOLOv5, End-to-End object detector project on custom dataset](https://towardsdatascience.com/yolov5-end-to-end-object-detector-project-on-custom-dataset-5d9cc2c95921)

- [Detecting objects in urban scenes using YOLOv5](https://towardsdatascience.com/detecting-objects-in-urban-scenes-using-yolov5-568bd0a63c7)


## GAN
### 1. SemanticGAN
[Semantic Segmentation with Generative Models (semanticGAN): Semi-Supervised Learning and Strong Out-of-Domain Generalization](https://nv-tlabs.github.io/semanticGAN/)
This novel framework uses a GAN that captures the joint image-label distribution and is trained efficiently using a large set of unlabeled images supplemented with only few labeled ones.

### 2. StyleGAN
- [StyleGAN — Official TensorFlow Implementation](https://github.com/NVlabs/stylegan)
This repository contains the official TensorFlow implementation of the following paper: [A Style-Based Generator Architecture for Generative Adversarial Networks](https://paperswithcode.com/method/stylegan)
- [StyleGAN2-ADA — Official PyTorch implementation](https://github.com/NVlabs/stylegan2-ada-pytorch)

- [Analyzing how StyleGAN works: style incorporation in high-quality image generation](https://towardsdatascience.com/analyzing-how-stylegan-works-style-incorporation-in-high-quality-image-generation-80a29227075b)
This blog focus on style incorporation via adaptive instance normalization.

### 3. CartoonGAN
- [Cartoon GAN (GitHub Resource Code)](https://github.com/FilipAndersson245/cartoon-gan)

- [CartoonGAN: Generative Adversarial Networks for Photo Cartoonization](https://openaccess.thecvf.com/content_cvpr_2018/papers/Chen_CartoonGAN_Generative_Adversarial_CVPR_2018_paper.pdf)

- [Generative Adversarial Networks for photo to Hayao Miyazaki style cartoons](https://arxiv.org/pdf/2005.07702.pdf) 
This paper takes on the problem of transferring the style of cartoon images to real-life photographic images by implementing previous work done by CartoonGAN. (Cartoon, Anime, Generative Adversarial Networks ,Style Transfer)

## Pettingzoo
PettingZoo is a Python library for conducting research in multi-agent reinforcement learning, akin to a multi-agent version of Gym.
- [Official pettingzoo website with comprehensive documentation](https://www.pettingzoo.ml/)
- [Pettingzoo GitHub repo](https://github.com/Farama-Foundation/PettingZoo)

- [Using PettingZoo with RLlib for Multi-Agent Deep Reinforcement Learning](https://towardsdatascience.com/using-pettingzoo-with-rllib-for-multi-agent-deep-reinforcement-learning-5ff47c677abd)
This is a blog tutorial on using PettingZoo multi-agent environments with the RLlib reinforcement learning library.




## Robots doing dexterous operations
- [Deep Reinforcement Learning with Adaptive Hierarchical Reward for Multi-Phase Multi-Objective Dexterous Manipulation](https://arxiv.org/ftp/arxiv/papers/2205/2205.13441.pdf)
Adaptive Hierarchical Reward Mechanism (AHRM) is to guide the Deep Reinforcement Learning (DRL) agent to learn manipulation tasks with multiple prioritized objectives.

- [Learning Dexterity](https://openai.com/blog/learning-dexterity/)
A system called Dactyl trained by OpenAI to manipulate physical objects with unprecedented dexterity. Dactyl learns to solve the object reorientation task entirely in simulation without any human input. 





## Deepstyle
DeepStyle is the custom deep learning framework that has the ability to generate high fashion clothing items.
- [Large-scale Fashion (DeepFashion) Database](https://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) This is the DeepFashion database, a large-scale clothes database.



- [DeepStyle (Part 1): Using State-of-the-Art Deep Learning to Generate Realistic High Fashion Clothing and Style.](https://towardsdatascience.com/deepstyle-f8557ab9e7b)
- [DeepStyle (Part 2 ): The Fashion GAN](https://towardsdatascience.com/deepstyle-part-2-4ca2ae822ba0)



## Intelligent Tutoring System (ITS)
### 1. Knowledge Tracing
Knowledge Tracing is the task of modelling student knowledge over time so that we can accurately predict how students will perform on future interactions. Improvement on this task means that resources can be suggested to students based on their individual needs, and content which is predicted to be too easy or too hard can be skipped or delayed.
- [A comprehensive summary of Knowledge tracing in Kaggle](https://www.kaggle.com/competitions/riiid-test-answer-prediction/discussion/201481#1102712)
Knowledge Tracing (KT) is the art of modeling the knowledge of a student as she interacts with her course work. It is a core part of Intelligent Tutoring Systems (ITS) which aim to provide a personalized learning experience to students. The data for Knowledge Tracing (KT) comes from 'interactions' which happen when the students perform 'exercise's, and this allows the prediction of their performance on future exercises. Interactions contains the student 'response's. These are binary values indicating whether the student answered the exercise correctly or not and the student's knowledge is updated accordingly. In certain models, exercises are tagged to 'Knowledge-concepts' or 'Skill-tags' by domain experts and these additional tags help the models perform better. So KT is all about: Student interactions (exams) -> Knowledge model(skill proficiency) --> Prediction (on new exams)


- [Paperswithcode: Knowledge Tracing](https://paperswithcode.com/task/knowledge-tracing)

- [Knowledge Tracing: A Survey](https://arxiv.org/pdf/2201.06953.pdf)

- [Concept-Aware Deep Knowledge Tracing and Exercise Recommendation in an Online Learning System](https://files.eric.ed.gov/fulltext/ED599194.pdf) This paper proposes a personalized exercise recommendation system for online self-directed learning.

### 2. Instructional Sequencing 
Instructional sequencing in Intelligent Tutoring Systems (ITS) refers to the pedagogical policy governing tutor decisions such as choosing the next topic, activity, problem, or feedback to help users learn. 

- [Deep Reinforcement Learning to Simulate, Train, and Evaluate Instructional Sequencing Policies](https://rl4ed.org/edm2021/files/spotlights/RL4ED_EDM21_h_11.pdf)(The data for this paper comes from the version of RoboTutor used during the last 3 months of the XPRIZE field evaluation.) 

- [Using Deep Reinforcement Learning to Train and Evaluate Instructional Sequencing Policies for an Intelligent Tutoring System](https://openreview.net/forum?id=eIPsmKwTrIe&referrer=[the%20profile%20of%20David%20Mostow](/profile?id=~David_Mostow1)) This paper presents a Deep Reinforcement Learning framework that can be used by Intelligent Tutoring System to learn an instructional policy that maximizes student learning gains.


### 3. Other subfields
- [Leveraging Deep Reinforcement Learning for Pedagogical Policy Induction in an Intelligent Tutoring System](https://files.eric.ed.gov/fulltext/ED599215.pdf) Much of the prior DRL work took the online learning approach. However, given the challenges of
building accurate simulations for modeling student learning, we investigated applying DRL to induce a pedagogical policy through an offline approach.


## Other project orientations
### 1. Chip Design
- [Chip Design with Deep Reinforcement Learning](https://ai.googleblog.com/2020/04/chip-design-with-deep-reinforcement.html )
we pose chip placement as a reinforcement learning (RL) problem, where we train an agent (i.e, an RL policy) to optimize the quality of chip placements.

### 2. Topology 
- [Network Topology Optimization via Deep Reinforcement Learning](https://arxiv.org/pdf/2204.14133.pdf)This paper proposes a novel deep reinforcement learning (DRL) algorithm, called Advantage Actor Critic-Graph Searching (A2C-GS), for network topology optimization.


## Transformer and RL
[How Transformers Are Making Headway In Reinforcement Learning](https://analyticsindiamag.com/how-transformers-are-making-headway-in-reinforcement-learning/)


## Extra materials
- [Deep Reinforcement Learning](https://arxiv.org/pdf/2201.02135.pdf)
- [XLVIN: eXecuted Latent Value Iteration Nets](https://arxiv.org/abs/2010.13146)
Value Iteration Networks (VINs) have emerged as a popular method to incorporate planning algorithms within deep reinforcement learning, enabling performance improvements on tasks requiring long-range reasoning and understanding of environment dynamics. 
- [TensorFlow Research Models](https://github.com/tensorflow/models/tree/master/research) https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_v4.py


- [Sheaf Neural Networks with Connection Laplacians](https://arxiv.org/abs/2206.08702)
A Sheaf Neural Network (SNN) is a type of Graph Neural Network (GNN) that operates on a sheaf, an object that equips a graph with vector spaces over its nodes and edges and linear maps between these spaces.


- [Top 20 Reinforcement Learning Libraries You Should Know](https://machinelearningknowledge.ai/reinforcement-learning-libraries-you-should-know/)
Lecturer Recommendation: RLLib. [This is the documentation of RLLib](https://docs.ray.io/en/master/rllib/rllib-env.html), which is a reinforcement learning library that provides high scalability and a unified API for a variety of RL applications, and it also has inbuilt support for OpenAI Gym environments.

- [A repo containing a curated list of awesome Deep RL resources.](https://github.com/kengz/awesome-deep-rl)

- [Graph Deep Learning - Benchmarking-GNNs](https://github.com/graphdeeplearning/benchmarking-gnns)