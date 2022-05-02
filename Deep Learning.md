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

## Why is Deep Learning taking off?

<img src="https://user-images.githubusercontent.com/72336341/166120751-264e3b50-e1aa-4e24-bd71-88aa36c0e38b.png" width="500"> 

If you have a large amount of data, make use of them to train a large model to make use of your data well.

<img src="https://user-images.githubusercontent.com/72336341/166120805-d6fbe075-be85-4827-a546-ab1c731172f9.png" width="200"> 


In sigmoid function, in region①②，gradient is close to 0, in gradient descend, the parameters will be updated very slow (See [NNDL book page 81](https://nndl.github.io/nndl-book.pdf)).
In ReLU function, the gradient for all >0 input is 1, the gradient is less likely to shrink to 0 in gradient descent. So gradient descend will work faster using ReLU.  

Cycle of developing a NN🔤

<img src="https://user-images.githubusercontent.com/72336341/166120916-b037c437-96e8-4c73-9c6e-7ff206caaabb.png" width="200"> 

# Logistic Regression as a Neural Network
## Binary Classification
<img src="https://user-images.githubusercontent.com/72336341/166217490-c696055b-5265-4061-952d-bbfb0ab4458c.png" width="500">
<img src="https://user-images.githubusercontent.com/72336341/166218227-a8d9461d-6a6b-4c39-8f58-03e52fbcabe0.png" width="500">

## Logistic Regression

<img src="https://user-images.githubusercontent.com/72336341/166219530-60bbc601-0a46-4555-805d-1e950c96138a.png" width="500">

when training the model, we need to leran w and b, for which prediction y has accurate prediction

## cost function

<img src="https://user-images.githubusercontent.com/72336341/166220552-2acef28f-04f5-4fb5-8178-02b7f8cea6d7.png" width="500">

when define the loss as (half) square of error, the optimization may be nonconvex, so the gradient descent cannot find global optimum.

The loss function computes the error for a single training example; the cost function is the average of the loss functions of the entire training set. In training the logistic regression model, we try to find parameters W and B that minimize the overall cost function J, written at the bottom.

## gradient desce nt

<img src="https://user-images.githubusercontent.com/72336341/166222674-3aee1d0f-fe13-4cc9-b8f1-f923ca34b0f2.png" width="500">

We can use any initial point for initization, since the J is convex, it doesn't matter which initial value
Gradient descent starts at that initial point and then takes a step in the steepest downhill direction. After steps of gradient descent, it might end up in J being global optimum.

<img src="https://user-images.githubusercontent.com/72336341/166223296-19bfe256-8d92-4234-bacb-2cb1301de872.png" width="500">

## Derivative with a Computation Graph 

<img src="https://user-images.githubusercontent.com/72336341/166224802-668995d5-bf48-416a-8223-5990153bdbd6.png" width="500"> 

Derivatives of final output is computed in right-to-left way.

<img src="https://user-images.githubusercontent.com/72336341/166225533-cd0bcda5-2b1a-4bc0-bfd3-5ec33f001000.png" width="500"> 
we will use da to mean dJ/da in python. 

In this class, in Python, we use **dvar** to represent **dFinalOutputVar/dvar** the derivative of a FinalOutputVariale w.r.t. intermediate quantities var.

<img src="https://user-images.githubusercontent.com/72336341/166225850-00d72f1c-cd90-4541-a6ff-aa7d645dc2d3.png" width="500"> 


## Logistic Regression Gradient Descent

<img src="https://user-images.githubusercontent.com/72336341/166226531-d2172774-a8a5-453c-8460-6db758a6a383.png" width="300"> 

<img src="https://user-images.githubusercontent.com/72336341/166227245-7bb25bd2-3d44-4e80-bb0b-599a0c0cb220.png" width="500"> 
