# AI-Flappy-Bird

## About
Created the popular game Flappy Bird using pygame and then implemented the NEAT algorithm to create an AI that learns how to play the game. 

## Libraries Required: 
pygame, neat 

## How to run? 
Simply run the **flappy_bird.py** file using the command `python3 flappy_bird.py`

## How it works?
Neural Network Setup:
- Inputs: Bird Y, Top Pipe, Bottom Pipe
- Outputs: Jump or not
- Activation Function: tanh
- Population Size (To start with): 20 
- Fitness Function: How far the bird goes 
- Max generations: 30

The first generation is a set of 20 birds acting randomly. Future generations keep getting better as they are made from the best performing birds from the previous generations. From my testing of the program, a bird which can play the game indefinitely without losing can usually be found by the **4th Generation**. Since this is a rather simple game, one can actually find a "winner" bird in the first generation itself if the Population Size is increased but then you never see the algorithm in action on your console so I decided to reduce the Population size. 
