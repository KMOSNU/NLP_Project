# NLP_Project

## Topic 

Heart rate estimation with PPG data by using biLSTM.

## data source 

https://archive.ics.uci.edu/ml/datasets/PPG-DaLiA

## baseline paper 

Reiss, A., Indlekofer, I., Schmidt, P., & Van Laerhoven, K. (2019). Deep PPG: Large-scale heart rate estimation with convolutional neural networks. Sensors, 19(14), 3079.

## brief description of this project 

We estimated heart rate with PPG data with different way of previous works. We estimated without using FFT preprocessing, but used only biLSTM architecture(we get inspired by ELMO). Although we couldn't beat the previous performance, with appropriate data augmentation or some modification of model architecture might help the model to find important features, as FFT helped to previous models, so the performance can be better with future works.

## model architecture 

biLSTM layer - embedding layer - fc layer

## data


input data size: 128(batch size)X512(8second-64Hz)
embedded data size : 128X3(representation of PPG data sequence)
output data size : 128X1(heart rate)
