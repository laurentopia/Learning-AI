# Learning-AI

## Setup on windows 10
https://towardsdatascience.com/installing-tensorflow-with-cuda-cudnn-and-gpu-support-on-windows-10-60693e46e781
The summary:
- download and install python 3.7 full https://www.python.org/downloads/
- download and install CUDA 10 https://developer.nvidia.com/cuda-downloads?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exenetwork
- download CUDNN https://developer.nvidia.com/rdp/cudnn-download
	- unzip and replace the content of zip\cuda inside C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v10.0
- install tensorflow:
	- open a command prompt with admin rights (right click on CMD, admin)
	- "pip3 install --upgrade tensorflow-gpu"
- restart
- test the environment:
	- open "idle"
	- type "import tensorflow as tf"
	- no error?
	- type "tf.test.is_gpu_available()", it it's TRUE all is working, YAY
- install Visual Code https://code.visualstudio.com/download
- setup Visual Code
	- create a folder
	- open CMD and go to that folder
	- type "code ." enter
	= this launches VC in the folder as project
	- go in extensions and type python, install the python module with the higuest * count
	- in VC create a file and save it as test.py
	- in that file type "import tensorflow as tf"
	- Code will initiate install of the python interpreter, ok all that
	- right click on the background of the editor window and select run in terminal
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
