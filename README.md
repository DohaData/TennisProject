# TennisProject

## Project Details
The project consists of solving the Tennis environment which consists of two agents that hit a ball over the next. The task is episodic.
- State Space: consists of 8 continuous variables corresponding to the position and velocity of the ball and the racket  
- Action space: consists of 2 continuous variables between -1 and 1 corresponding to the movement toward (or away from) the net, and jumping 
- Reward: The agent receives a reward of +0.1 when he hits the ball over the next and -0.1 when he lets the ball hits the ground or hits the ball out of bounds.

 The score is computed at the end of each episode by taking the max of the rewards accumulated by each agent. The environment is considered solved when the average score is higher than 0.5 on average for 100 episodes. 

## Repository Structure
This repository is composed of:
- Actor weights: actor_checkpoint.pth
- Critic weights: critic_checkpoint.pth
- Project report: Report.pdf
- Project main notebook: Tennis.ipynb

## Getting Started
In the Tennis.ipynb:
- Install the dependencies by running the first cell of the notebook in Start the Environment section.
- Start the environment by running the second cell.

## Instructions
The Tennis.ipynb is composed of multiple sections:
1. Start the Environment: to start the environment
2. Examine the State and Action Spaces: to examine the State and Action spaces
3. Utilities function to retrieve the state, reward and done when executing an action in the environment
4. Agent dependencies and hyperparameters to finetune when training
5. Critic and Actor models architectures
6. Replay buffer for past experiences: to store experiences and sample training batches
7. Ornstein-Uhlenbeck process noise
8. Deep Deterministic Policy Gradient agent model: agent class
9. Agent training function: agent training function definition
10. Agent training results: to run the training function and retrieve the agent scores
11. Agent training scores plot: plot the agent scores

To run the training function, you can execute the notebook cells in order until section 9 included.
To finetune the agent hyperparameters, you can change section 4 values.
Running section 10 will output a plot showing agents average scores obtained through training.

