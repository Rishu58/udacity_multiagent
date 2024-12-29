# Navigation
This project is part of the Deep Reinforcement Learning Nanodegree Program, by Udacity.
The goal in this project is to create and train two agent to play tennis.


# Understanding the environment
In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
This yields a single score for each episode.
The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.



# Running the code

To successfully run the code, you need to ensure that the following files are in place:

Download the depandicies from requirement.txt file.

1. **Tennis.ipynb** - This is the primary notebook where the final implementation is done. Start running the code here.
2. **DDPG.py** - This file contains all the necessary methods required for the code to function properly. Ensure it is imported into the notebook. It also has replay buffer.
3. **Model_1.py** - It has actor ( Layer_1 (state_dim, 200), Relu, layer_2(200,150),Relu, layer_3(150,action size), Tanh )and critic (Layer_1 (state_dim, 400), Relu, layer_2(400+action_size,300),Relu, layer_3(150,1) 

Here is the final result which you can expect result.


<img width="584" alt="Screenshot 2024-12-29 at 4 43 21 PM" src="https://github.com/user-attachments/assets/1fd94ae2-f6b3-4f8b-ad0a-e7f929f55ad7" />





