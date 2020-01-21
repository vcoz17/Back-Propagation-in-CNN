# Back Propagation in Convolution Neural Networks

Convolution Neural Network is widely used for various tasks in analyzing visual imagery. Such tasks include image/video recognition, recommender systems, image classification, and natural language processing.

In our final project, we want to explore specifically how CNN classifies number digits (0-9) based on the hand written images. In this case, we would want to utilize the MNIST dataset (handwritten digits images for training image processing systems) and to see how our model predicts the result of test images after training after a short period of time.

Layers for our network
In our model for simplicity, we includes 4 most importants layers to achieve the desire prediction:

Convolution Layers:

Extract the features from the images.
Filter the image with smaller pixel filter to decrease the size of the image without hurting the relationship between the pixel and its adjacents/close pixels.
Rectified Linear Unit (ReLU):

Increase the non-linearity in our images, i.e, ReLU layers remove all the black elements from the input images, and keep pixels carrying a positive value (grey and white colors).
Max Pooling layers:

Reduce parameters counts, and thus, computational complexity. Specifcally, we select the maximum, average, or sum of values insides the pixels.
Prevent overfitting problems for our model.
Set of fully connected layers

Furthermore, in each layer, we include a forward pass and a backpropagation to simplify the computation. Specifcally, after performing a forward pass, we want to use backpropagation to compute loss function gradient w.r.t its weight, and then we update the weight using gradient descent. The method of backpropagation allows us to achieve faster derivatives computation and narrow the difference between desired output and achieved model's outpur as much as possible.

Google Colab: https://colab.research.google.com/drive/1Adu093zFsgXCmbwgQWXeKlkD-ILiCKgb?authuser=1


