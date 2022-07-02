# Classification-with-Neural-Network-using-Numpy-only

Author: jvachier <br>
Creation date: June 2022 <br>
Publication date: July 2022 <br>

My goal is to classify $10$ digits from $0$ to $9$ with Neural Networks using Numpy only. The training set (train.csv) contains $42 000$ labelled pictures and the testing set (test.csv) contains $28 000$ non-labelled pictures. Each picture has $789$ pixels ($28 \times 28$) and is the input size of the network. (data from https://www.kaggle.com/c/digit-recognizer) <br>

Three Networks are built: <br> 
* 1 - Two Layers Neural Network with Sigmoid (2 Layers with Sigmoid 1), using a sigmoid activation function for the output layer. After the input, the first layer is composed of $20$ neurons. The second layer (the output layer) contains $10$ neurons as $10$ digits are classified. <br><br>
* 2 - Two Layers Neural Network with Softmax (2 Layers with Softmax), however here we use a softmax as activation function for the output layer. <br><br>
* 3 - Three layers Neural Network with Softmax (3 Layers with Softmax). The first layer contains $128$ neurons, the second layer $20$ neurons and the output layer $10$ neurons.

In the three Networks, the activation function for the intermediate layers is ReLu and the accuracy is computed. Moreover, the cost function used is the mean squared error (MSE). In the case of the first Neural Network, two backward propagations are used to show that it is not necessary to include the activation function of the output layer in the computations (appendix - 2 Layers with Sigmoid 2). In addition, to see the effect of the learning rate in the third Neural Network, two values are used and the accuracy is compared (appendix). <br>

The three Networks are first trained independently on the training set and then tested using the test set. The accuracy reaches almost $99\%$.

(Additionally, this code is also available on my Kaggle profile at )
