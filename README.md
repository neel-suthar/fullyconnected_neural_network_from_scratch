# Fully Connected Neural Network

## Part - 1
- In part 1 we created and trained fully connected neural network from scratch using NumPy.

## Part - 2 
- In part 2 we developed fully connected neural network using PyTorch.
For Kernel size 5 with 10 epochs we get:

Accuracy of the network on the 10000 test images: 59 %

Accuracy of plane : 63 %

Accuracy of car : 74 %

Accuracy of bird : 45 %

Accuracy of cat : 26 %

Accuracy of deer : 58 %

Accuracy of dog : 46 %

Accuracy of frog : 72 %

Accuracy of horse : 61 %

Accuracy of ship : 76 %

Accuracy of truck : 67 %

For Kernel size 3 with 10 epochs we get:

Accuracy of the network on the 10000 test images: 59 %

Accuracy of plane : 65 %

Accuracy of car : 72 %

Accuracy of bird : 38 %

Accuracy of cat : 46 %

Accuracy of deer : 41 %

Accuracy of dog : 51 %

Accuracy of frog : 68 %

Accuracy of horse : 63 %

Accuracy of ship : 72 %

Accuracy of truck : 73 %

From above observation we can say that for some labels the training accuracy increase and for other training accuracy decreases. Kernel decides whether the neural network analyses smaller details or larger details.

With 2 Convolutional Layers(3->30, 30->60) and 3 Linear Layers(input->120->84->10): In this attempt I took Kernel size as 3x3, but I increase the number of output channels in convolutional layers. The output of 1st layer is 30 and second is 60.

For kernel size 3x3 and 10 epochs, I got following results:

Accuracy of the network on the 10000 test images: 65 %

Accuracy of plane : 73 %

Accuracy of car : 85 %

Accuracy of bird : 26 %

Accuracy of cat : 43 %

Accuracy of deer : 57 %

Accuracy of dog : 63 %

Accuracy of frog : 78 %

Accuracy of horse : 74 %

Accuracy of ship : 73 %

Accuracy of truck : 76 %

I tried changing the final activation function from softmax to logsoftmax with the same architecture as above.

The following results were obtained on changing the activation function of final linear layer to logsoftmax with 10 epochs:

Accuracy of the network on the 10000 test images: 69 %

Accuracy of plane : 72 %

Accuracy of car : 79 %

Accuracy of bird : 60 %

Accuracy of cat : 39 %

Accuracy of deer : 67 %

Accuracy of dog : 63 %

Accuracy of frog : 78 %

Accuracy of horse : 75 %

Accuracy of ship : 82 %

Accuracy of truck : 75 %

We can see from other observation that the activation function plays a huge role in increasing the accuracy of the neural network just like the architecture.

I changed the structure of neural network again. This time I used 3 convolutional layers and 6 linear layers.

On running the input through this neural network with 10 epochs the following result is obtained:

Accuracy of the network on the 10000 test images: 71 %

Accuracy of plane : 75 %

Accuracy of car : 86 %

Accuracy of bird : 45 %

Accuracy of cat : 57 %

Accuracy of deer : 69 %

Accuracy of dog : 59 %

Accuracy of frog : 81 %

Accuracy of horse : 78 %

Accuracy of ship : 81 %

Accuracy of truck : 75 %

Thus we can see that there is a 2% increase in the accuracy, it is due to increase in linear as well as convolutional layers.

## Run Code
- Download the nn.ipynb and run it on google colab.
