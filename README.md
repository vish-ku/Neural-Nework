# Neural-Nework
This is the third project of Machine learning, where we try to implement a Neural Network. Neural network is bassicaly a network structure where we feed the inputs into hidden layers with certain number of nodes and after an activation of these nodes, we get a certain output. There are certain weights and biases associated with the nodes, so we train the network and tweak the weights and biases untill we get the desired outputs. The training of the model is done by a method call backpropagation ( also known as Gradient desent.)

## Implementation
I implemented the nerual network where we can input the number of hidden layers and the number of nodes required per hidden layer. For activation, I tired using the relu, sigmoid and softmax function. Some of them were effective for other I ran into regularity issues (moslty overflow of values!). 

The forward propagation stage was implemented with the relu function and the output activation was done with the softmax activation (softmax worked best with classification.) Training the model was done by backpropagation. They are in the jupyter notebooks. 

Initialzing with the correct weights were also important, else the model quickly ran into issues with overflow. 

## Data sets.
I chose two data sets, very different from each other. One is a mushroom data set which had around 8000 observation. We had to classify the mushroom into poisonous or edible. The inputs were all catogorical, so I converted them into all binary input. 

The other data set was a liver disoder data set, there was only 345 observations, and with the given input we had to identify if the patients had liver disorder or not. Before implementing the model on this I normalized the data set, else the model ran into overflow issues. 

## Observations

One thing that I observed is that there is no one specific model that works with all data sets. The nature of the inputs, the number of observations, dimension of the input, number of layers in the network, number of nodes per layer, the learning rate during backpropagation, the kind of activation functions used, all play a part in a successful model. 

The model was highly successful in classifying the mushrooms, the model gave an accuracy of about 97%. I believe this was due to the very nice nature of the input (thery were binary inputs) and the fact that there were many training instances. 

With the liver disorder data set, I was not able to get as good results as the mushroom data set. Probably this was because of the low number of training instances and the nature of inputs. I was not able to find the appropriate parameters to train the model. This gave me an accuracy of 20%

All the results are documented in the ipynb file. 




