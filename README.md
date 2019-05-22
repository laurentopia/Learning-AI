# Learning-AI

## Setup on windows 10
https://towardsdatascience.com/tensorflow-gpu-installation-made-easy-use-conda-instead-of-pip-52e5249374bc
The summary:
- download anaconda https://repo.anaconda.com/archive/Anaconda3-2019.03-Windows-x86_64.exe
- launch Anaconda Prompt
- "conda create --name tf_gpu tensorflow-gpu"
- "conda activate tf_gpu"
- "conda install keras", "conda install matplotlib", "conda install pandas"
- python

- install Visual Code https://code.visualstudio.com/download
- setup Visual Code
	- create a folder and a test.py file
	- open file with code from the context menu
	- there will be a message on the left pane of code, accept to open the folder
	- code will also suggest to install the python extension
	- when this is done, in the lower left corner there is the python version and Conda environment, select tf_gpu
DONE!

-----------------

## Various topologies of NN

![](https://cdn-images-1.medium.com/max/600/1*UmLdrVH-_EMnL-pUjcYKhA.png)
https://towardsdatascience.com/the-mostly-complete-chart-of-neural-networks-explained-3fb6f2367464
I'm thinking for the reconstruction of noisy analog VTX signal the LSTM would be good as it keeps memory of the flow of video, maybe it can rebuild video when it goes to static. 

Recurrent Neural Nets (RNN)
https://medium.com/cracking-the-data-science-interview/a-gentle-introduction-to-neural-networks-for-machine-learning-d5f3f8987786

## testing Keras things online
https://colab.research.google.com/drive/1LISrn_W2FJDBz5CxJ1VC5CpISnQnuH6X#scrollTo=WHs49rG6LUFm&line=8&uniqifier=1
GANS etc... in Keras.js https://transcranial.github.io/keras-js/#/mnist-acgan

## NOTES:
Normalizing at the end of each dense layer is better than dropout as information doesn't vanish
Leaky Relu better than Relu?

Keras is very easy to use, is it possible to make it self generate and self test various toplogies?

## PROJECTS
Project Auto Pilot:
Phase 1: implement a navigation layer on top of inav or betaflight that dodges trees. Use the Zurich trail navigation method for capturing training data: 3 cameras, one straight, 2 at 60 degrees, each footage is self categorized as forward, left and right.
First attempt yiels poor result, around 50% accuracy and 5 loss, footage was captured inside the house and a lot of images look similar. The cameras were set at 90 degrees from each other. Try 45 degrees and walk or fly slowly inside the forest.

Project VTX healing:
Maybe a simple 
