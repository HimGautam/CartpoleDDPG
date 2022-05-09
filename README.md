## CartpoleDDPG

This project is my own implementation of DDPG algorithm from the paper [Continuous control with deep reinforcement learning](https://arxiv.org/pdf/1509.02971).

![CartpoleDDPG](https://user-images.githubusercontent.com/70597091/167424335-9094fcd6-f9ac-4841-bbe8-926b6f543cc5.gif)

## Overview

This project solves the control problem of CartPole balancing by using DDPG algorithm. It benefits from the DQN method and Actor Critic method to find the best policy for the task at hand. 

It uses a deterministic policy network, thus a gaussian noise is added to the action values to facilitate exploration. In the original DDPG paper, authors have used Ornstein-Uhlenbeck process for exploration. However, later analysis of the algorithm revealed that a simple gaussian noise also works fine.

## Requirements

This project requires following dependencies:
1) Jupyter Notebook
2) Python
3) Open AI Gym
4) Numpy
5) Tensorflow

## Trying Out

For trying out this project, just download the weights of actor and critic networks from this repo. Then, load the weights to their respective networks and run the cell with ```# Testing``` comment on it.
