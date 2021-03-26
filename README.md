# CMPUT366
Assignment project 3 of CMPUT366

(Neural Networks) The MNIST dataset is a set of images of handwritten digits labelled by
their actual digit. We will operate on two versions of this dataset: one with the images shifted
2 pixels to the upper-left, and one with the images shifted 2 pixels to the bottom-right.
This question requires the use of TensorFlow. You may need to install Tensorflow using the
following command:
pip3 install tensorflow
(a) [10 points] Implement a fully-connected feed-forward neural network for classifying
MNIST images according to the digit that they represent by editing the mlp2 function in
the provided cnn.py file.
The network should have two hidden layers: one with 128 rectified linear (‘relu’) units,
and one with 64 rectified linear units. The output should be a fully-connected layer of 10
units with the softmax activation. The cnn.py file contains an example implementation
of a network with a single hidden layer in the mlp1 function that you may template from.
The main function will test your program for you; you may add any tests that you like.
It will also create a file called examples.png that contains examples images from the two
test sets.
The function should train the network using the training features train_x and labels
train_y, and then evaluate the accuracy of the trained network on two different test
sets: test1_x, test1_y, and test2_x, test2_y. This is demonstrated in mlp1.
We will run your code by importing the cnn module and calling mlp2, so it is important
that your code follow these naming conventions.
Submit all of your code for this question and question 1 (including provided boilerplate
files) in a single zip file.
(b) [30 points] Implement a convolutional neural network for classifying MNIST images by
editing the cnn function in the provided cnn.py file.
The network should have the following architecture:
• A layer of 32 convolutional units with a kernel size of 5 × 5 and a stride of 1, 1.
• A max-pooling layer with a pool size of 2 × 2 and a stride of 2, 2.
• A layer of 64 convolutional units with a kernel size of 5 × 5 and the default stride.
• A max-pooling layer with a pool size of 2 × 2 and the default stride.
• A Flatten layer (to reshape the image from a 2D matrix into a single long vector)
• A layer of 512 fully-connected relu units
• A layer of 10 fully-connected softmax units (the output layer)
Submit all of your code for this question and question 1 (including provided boilerplate
files) in a single zip file.
