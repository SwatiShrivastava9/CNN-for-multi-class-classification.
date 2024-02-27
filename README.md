# CNN-for-multi-class-classification.
CNN is implemented for multi-class classification. The dataset consists of handwritten digits; 60k images for training and 10k images for testing.
The convolutional neural network (CNN) architecture is designed with three fully convolutional layers, each serving a specific purpose. The first convolutional layer employs a 7x7 kernel, includes max-pooling with a stride of 1, and produces 16 output channels. The second convolutional layer, utilizing a 5x5 kernel, incorporates max-pooling with a stride of 1 and generates 8 output channels. The third convolutional layer features a 3x3 kernel, average pooling with a stride of 2, and yields 4 output channels. The output layer is tailored to match the number of classes in the classification task which is 10.

To maintain the input image dimension, zero padding is applied. The dataset is split into standard train-test partitions. The batch size is 16.

The activation function ReLU is employed for convolutional layers, while the softmax activation is applied to the output layer. The Adam optimizer is utilized, and the loss function is set as cross-entropy. Training is conducted for 10 epochs. Accuracy and loss per epoch are plotted to visualize the learning progress.

Additionally, a confusion matrix is generated for the test set, providing insights into the model's performance across various classes. Finally, the total trainable and non-trainable parameters are reported, encapsulating the network's complexity and resource requirements

Additionally batch normalization is used to improve performance and avoid overfitting,
