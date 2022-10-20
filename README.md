# CIFAR10-Photo-Classification

Using Keras, a convolutional neural network (CNN) was used to complete the photo classification task for the CIFAR-10 dataset (https://www.tensorflow.org/datasets/catalog/cifar10).

## Model & Training
The following choices were made:

  • Convolutional Layers:
    o Number of Layers: 3
    o Number of Kernels:
      ▪ 1st Convolutional Layer: 32
      ▪ 2nd Convolutional Layer: 64
      ▪ 3rd Convolutional Layer: 128
    o Dimension of Kernels: 3 x 3
    o Activation Function: ReLU
    o Padding: Same

  • Max-Pooling Layers:
    o Number of Layers: 3
    o Dimension of Kernels: 2 x 2

  • Dense Layers:
    o Number of Layers: 1 hidden layer & 1 output layer
    o Number of Nodes:
      ▪ Hidden Layer: 128
      ▪ Output Layer: 10
    o Activation Function:
      ▪ Hidden Layer: ReLU
      ▪ Output Layer: Softmax

  • Dropout: increasing ratios (0.2, 0.3, 0.4, 0.5)

  • Batch Normalization

  • Gradient Descent:
    o Method: Adam 
    o Learning Rate: 0.001 (default)

  • Loss Function: Sparse Categorical Cross Entropy

  • Metric: Accuracy

  • Number of Epochs: 400

  • Batch Size: 128

The final model summary is as shown below:

![image](https://user-images.githubusercontent.com/25527107/196992099-2f4e9d8c-9f97-4c77-af88-7ecd0969a2fc.png)

## Results
Training and Testing Accuracies:

![image](https://user-images.githubusercontent.com/25527107/196992263-f29bb364-a76a-4dae-9ab4-04464b79126e.png)

Training and Testing Losses:

![image](https://user-images.githubusercontent.com/25527107/196992325-63b62f72-1622-4819-80ce-64028f08e9da.png)
