# Traffic Sign Recognition using Convolutional Neural Networks (CNN)

## Overview

This repository contains the implementation of a Convolutional Neural Network (CNN) for the recognition of traffic signs. The project aims to accurately classify traffic signs from images using deep learning techniques. The trained CNN model can be utilized to enhance road safety, improve autonomous vehicle capabilities, and contribute to traffic management systems.

## Table of Contents

- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Results](#results)

## Dataset

The project utilizes the [German Traffic Sign Recognition Benchmark](http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset) dataset, which consists of more than 50,000 images of 43 different traffic sign categories. The dataset is split into training, validation, and test sets to ensure robust model evaluation.


## Model Architecture

The CNN model architecture consists of multiple convolutional and fully connected layers, designed to learn hierarchical features from traffic sign images. The architecture is as follows:

1. Convolutional Layer #1: Input = 32x32x1, Output = 28x28x6, Activation = ReLU, Pooling = 2x2
2. Convolutional Layer #2: Input = 14x14x6, Output = 10x10x16, Activation = ReLU, Pooling = 2x2
3. Flattening Layer: Input = 5x5x16, Output = 400
4. Fully Connected Layer #1: Input = 400, Output = 120, Activation = ReLU
5. Fully Connected Layer #2: Input = 120, Output = 84, Activation = ReLU
6. Fully Connected Layer #3: Input = 84, Output = 43 (Number of traffic sign categories), Activation = Softmax

## Results

The trained CNN model achieves an impressive accuracy on the test dataset, demonstrating its effectiveness in accurately classifying traffic signs in real-world scenarios. The model's performance is visualized using training and validation accuracy/loss curves.

