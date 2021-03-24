# Udacity-TV-Script-Project

The Jupyter-Notebook-File [dlnd_tv_script_generation.ipynb](dlnd_tv_script_generation.ipynb) includes my
solution to the Generate-TV-Scripts-Project in the Deeplearning-Nanodegree. 

## General Task

The task is to use a neural network to generate an artificial Seinfeld TV script. 

## Approach

The idea is to attack this task by training a recurrent neural network feeding it a dataset of Seinfeld
TV scripts from nine seasons. After training, the functionality of the model will be as follows: After
inputting a word to the model, it will generate a whole script of a specified length word by word.

All of the code is written in python and the pytorch library is used to implement the recurrent neural
network.

## Architecture of the Model and Hyperparameters

The network is a recurrent neural network consisting of two hidden layers with LSTM cells, an embedding
layer at the beginning and a fully connected layer at the end. The optimizer for the backpropagation
process is an Adam optimizer. 

Here are the chosen hyperparameters:

* Sequence Length: 10
* Batch Size: 128
* Embedding Dimension: 400
* Dimension of hidden States: 256
* Epochs: 15
* Learning Rate: 0.001


