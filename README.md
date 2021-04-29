# Neural-Nework
This is the third project of Machine learning, where we try to implement a Neural Network. Neural network is bassicaly a network structure where we feed the inputs into hidden layers with certain number of nodes and after an activation of these nodes, we get a certain output. There are certain weights and biases associated with the nodes, so we train the network and tweak the weights and biases untill we get the desired outputs. The training of the model is done by a method call backpropagation ( also known as Gradient desent.)

## Implementation
I implemented the nerual network where we can input the number of hidden layers and the number of nodes required per hidden layer. For activation, I tired using the relu, sigmoid and softmax function. Some of them were effective for other I ran into regularity issues (moslty overflow of values!). 

The forward propagation stage was implemented with the relu function and the output activation was done with the softmax activation (softmax worked best with classification.) Training the model was done by backpropagation. They are in the jupyter notebooks. 

Initialzing with the correct weights were also important, else the model quickly ran into issues with overflow. 

## Data sets.
I chose two data sets, very different from each other. One is a mushroom data set which had around 8000 observation. We had to classify the mushroom into poisonous or edible. The inputs were all catogorical, so I converted them into all binary input. A 90-10% Training-Testing split was used for this data set

The other data set was a mesothelioma data set, there was 324 observations, and with the given input we had to identify if the patients had mesothelioma or not. Before implementing the model on this I normalized the data set, else the model ran into overflow issues. A 75-25% Training- Testing split was use for this data set. 

## Observations

One thing that I observed is that there is no one specific model that works with all data sets. The nature of the inputs, the number of observations, dimension of the input, number of layers in the network, number of nodes per layer, the learning rate during backpropagation, the kind of activation functions used, all play a part in a successful model. 

The model was highly successful in classifying the mushrooms, the model gave an accuracy of about 97%, with just as much as 30 iterations through the entire data set. I believe this was due to the very nice nature of the input (thery were binary inputs) and the fact that there were many training instances. It took a lot of tweaking to the original model to make the network run smoothly. 

The model also ran very efficiently with the mesothelioma data set with a very high accuracy of 98% ( I set the accuracy standard even higher than for the mushroom data set). Since the number of data instances were small compared to the mushroom data set, I iterated through the data set 200 times. 

All the results are documented in the ipynb file. 




