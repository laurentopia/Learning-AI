# Learning-AI

Topology of NN
![](https://cdn-images-1.medium.com/max/600/1*UmLdrVH-_EMnL-pUjcYKhA.png)
https://towardsdatascience.com/the-mostly-complete-chart-of-neural-networks-explained-3fb6f2367464
I'm thinking for the reconstruction of noisy analog VTX signal the LSTM would be good as it keeps memory of the flow of video, maybe it can rebuild video when it goes to static. 

testing Keras things online
https://colab.research.google.com/drive/1LISrn_W2FJDBz5CxJ1VC5CpISnQnuH6X#scrollTo=WHs49rG6LUFm&line=8&uniqifier=1

Recurrent Neural Nets (RNN)
https://medium.com/cracking-the-data-science-interview/a-gentle-introduction-to-neural-networks-for-machine-learning-d5f3f8987786

NOTES:
Normalizing at the end of each dense layer is better than dropout as information doesn't vanish
Leaky Relu better than Relu?

Keras is very easy to use, is it possible to make it self generate and self test various toplogies?

Project Auto Pilot:
Phase 1: implement a navigation layer on top of inav or betaflight that dodges trees. Use the Zurich trail navigation method for capturing training data: 3 cameras, one straight, 2 at 60 degrees, each footage is self categorized as forward, left and right.
First attempt yiels poor result, around 50% accuracy and 5 loss, footage was captured inside the house and a lot of images look similar. The cameras were set at 90 degrees from each other. Try 45 degrees and walk or fly slowly inside the forest.

Project VTX healing:
Maybe a simple 

GANS etc... in Keras.js https://transcranial.github.io/keras-js/#/mnist-acgan
