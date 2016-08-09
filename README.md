# SummerTraining_hw2

*TA: Pang-Chi Huang*

*Email: zyi870701@gmail.com*

*August 9, 2016*

## Problem Description

Train a simple deep CNN on the CIFAR10 small images dataset.

## Basic

Finish watching **lecture 3 – Convolutional Neural Network** first.

According to the lecture, you need to modify the sample code we provide so that it can generate the accuracy higher than **81.0%**. For example, you can try different depths, batch size, activation functions, filters and pool size, etc.

Tip: You can also adjust the number of epoch to save your time.

* Sample code: cifar10_cnn.py
* Reference: https://github.com/fchollet/keras/blob/master/examples/cifar10_cnn.py

## Option

You can use the sample code to visualize filters or use other ways to analyze the functionality of **"filter"**.

The sample code will use the model training from cifar10_cnn.py, so you need to modify the model architecure in the sample code if you adjust the model in cifar10_cnn.py.

You can also adjust the configuration in the sample code to get different visualization result. Like Below:

    # === Configuration ===

    # dimensions of the generated pictures for each filter.
    img_width = 128
    img_height = 128
    
    # path to the model weights file.
    weights_path = 'cnn_weights.h5'
    model_path = 'cnn_model.json'
    
    # the name of the layer we want to visualize (see model definition below)
    layer_name = 'conv2_1'
    
    # we will stich the best filters on a 1 x 1 grid.
    n = 1
    
    # we only scan through the first 30 filters,
    # but there are actually 32 of them
    scan_filter_num = 30
    
    # === End of Configuration ===


Here are some visualization examples in the folder **visualization_examples**, the 1x1 and 4x4 images are produced by the CNN network from the sample code, and the 8x8 image is produced by the VGG network from the reference below.

* Sample code: conv_filter_visualization.py
* Reference: https://github.com/fchollet/keras/blob/master/examples/conv_filter_visualization.py

## Reminder

* About how to install Keras and how to run the sample code, please refer to homework 1.
* If you have any question, please feel free to contact us or post it on Facebook group.

## More References

1. http://cs231n.github.io/convolutional-networks/
2. Neural Networks and Deep Learning (Chapter 6)
  - http://neuralnetworksanddeeplearning.com/
3. How convolutional neural networks see the world
  - https://blog.keras.io/how-convolutional-neural-networks-see-the-world.html
