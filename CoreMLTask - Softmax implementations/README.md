## Overview of the task

The task 

## Analysis of implementation of different variations of Softmax on CNN for image classification

The softmax function is a widely used activation function in neural networks, particularly in classification tasks. However, its computational complexity is a concern when dealing with a large number of classes. 

In this study, I explore  and try to implement different softmax variations and their impact on model performance and training time in the context of image classification tasks using the CIFAR-100 dataset. The task is to develop a convolutional neural network (CNN) model with the standard softmax and compare it with two alternative softmax implementations, namely logsoftmax and Gumbel-Softmax. These models were then evaluated using various performance metrics, including accuracy, precision, recall, F1 score, and confusion matrix, and compare their performance and epoch time.

### Introduction

Neural networks have revolutionized image classification tasks, and the softmax function has become a popular choice for generating probabilistic outputs. However, its time complexity grows linearly with the number of classes, making it computationally expensive for large-scale classification problems. 

![](assets/softmaxworkingsimple.jpg)

To address this issue, alternative softmax implementations have been proposed, such as logsoftmax and Gumbel-Softmax, which aim to reduce the computational complexity while maintaining performance.

logsoftmax reduces this this complexity to O(logN)

### Methodology:

In this study, we employ the CIFAR-100 dataset, consisting of 100 classes of images, to compare the performance of different softmax variations in CNN models. We first develop a baseline CNN model with the standard softmax implementation. Then, we create two additional models using the same architecture but replacing the softmax layer with logsoftmax and Gumbel-Softmax, etc.


