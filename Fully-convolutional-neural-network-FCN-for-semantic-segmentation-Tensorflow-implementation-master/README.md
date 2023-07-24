# Fully convolutional neural network (FCN) for semantic segmentation with tensorflow.

This is a simple implementation of a fully convolutional neural network (FCN). The net is based on fully convolutional neural net described in the paper [Fully Convolutional Networks for Semantic Segmentation](https://arxiv.org/pdf/1605.06211.pdf).  The code is based on [FCN implementation](https://github.com/shekkizh/FCN.tensorflow)  by Sarath Shekkizhar with MIT license but replaces the VGG19 encoder with VGG16 encoder. The net is initialized using the pre-trained VGG16 model by Marvin Teichmann.
An improved version of this net in pytorch [is given here](https://github.com/sagieppel/Fully-convolutional-neural-network-FCN-for-semantic-segmentation-with-pytorch)
## This is an old model for a New more accurate version of the net focused on recognition of materials in transparent vessels see this [link](https://github.com/sagieppel/Detecting-and-segmenting-and-classifying-materials-inside-vessels-in-images-using-convolutional-net)

## Details input/output
The input for the net is RGB image (Figure 1 right).
The net produces pixel-wise annotation as a matrix in the size of the image with the value of each pixel corresponding to its class (Figure 1 left).

![](/Figure1.png)
Figure 1) Semantic segmentation of image of liquid in glass vessel with FCN. Red=Glass, Blue=Liquid, White=Background

## Requirements
This network was run with Python 3.6  Anaconda package and Tensorflow 1.1. The training was done using Nvidia GTX 1080, on Linux Ubuntu 16.04.

