# Neural Networks and Deep Learning
<!-- 
use this to shrink the image size 
<img src="" width="500"> 
-->
<img src="https://user-images.githubusercontent.com/72336341/166098474-f0dc7da9-102a-40ee-9e25-6fdff655fd9c.png" width="500"> 

Strategy for building a machine learning system has changed in the era of deep learning. For example, the way you split your data into train, development/dev(also called holdout cross-validation sets), and test sets, has changed in the era of deep learning

RNN: recurrent neural networks; LSTM models: long short term memory models

## What is Neural Network?
<img src="https://user-images.githubusercontent.com/72336341/166098485-79f23ff2-bc7f-4460-9516-40e2d32454fa.png" width="500"> 

since house price cannot be negative, we make it 0 (rectified) when blue line starts to touch x-axis.

neuron implements the function curve in blue

<img src="https://user-images.githubusercontent.com/72336341/166098491-e1664434-b66d-4f3f-a5d1-78c1d7a568c0.png" width="500"> 

family size, walkability, school quality are our interpretation of the outputs of first layer of neurons, it is not input!! 

In the implementation:

<img src="https://user-images.githubusercontent.com/72336341/166098523-49700bdb-22a9-48b0-b852-4375ee9c14d1.png" width="500"> 

in neural network, give node① all the features and neural network will decide its representation.

## Supervised Learning with Neural Network
<img src="https://user-images.githubusercontent.com/72336341/166098531-90202cdc-a80d-4e25-85b1-6ff6c662fb44.png" width="500"> 

What model to use? Sequence data (like audio, language text):RNN; Image application: CNN; autonomous driving: custom hybrid NN 

<img src="https://user-images.githubusercontent.com/72336341/166098533-875fa2e9-c0c3-4c41-9cb3-4f111bb5b941.png" width="500"> 

RNN is suitable for 1-dimensional sequence data.

### Structured Data and Unstructured Data

Structured Data: each of the feature has well-defined meaning

<img src="https://user-images.githubusercontent.com/72336341/166098538-cbfa30d9-39b6-45d8-9659-2f2298f73644.png" width="500"> 

Unstructured Data: each of the feature do not has well-defined meaning

<img src="https://user-images.githubusercontent.com/72336341/166098544-0354beed-7330-42dd-9579-891c36005a17.png" width="500"> 

features of image: pixels values; features of text: individual words.

