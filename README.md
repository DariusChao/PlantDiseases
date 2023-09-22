# Plant Disease Classification Model

## Overview

This repository contains a machine-learning model for the classification of 38 different plant diseases commonly found in crops. The model uses convolutional neural networks (CNNs) to analyze images of crop leaves and predict the specific diseases affecting them.

## Table of Contents

- [Dataset](#dataset)
- [Usage](#usage)
- [Results](#results)

## Dataset

The model was trained on the [New Plant Diseases Dataset](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset) from Kaggle. This dataset contains a vast collection of augmented images of diseased and healthy crop leaves, categorized into 38 classes. These images are sorted into ~70000 training images and ~17000 validation images. I used a part of the validation images to create a testing dataset as there was no testing dataset.

## Usage

Requirements:
1. Tensorflow
2. Keras
3. Numpy
4. scikit-learn
5. matplotlib

Steps:
Simply run each cell in order, ensuring that the dataset has been fully downloaded from Kaggle before moving on to process the data. A Kaggle account is required in order to download the dataset so create an account and get the account key prior to beginning.

## Results
The model ended up performing pretty well with approximately 98% accuracy on the testing data. The recall, f1-score, and precision are all high as well for most of the 38 classes. There were some signs of minor overfitting during training, so I would like to continue tweaking and experimenting with the model architecture and hyperparameters. I also plan to test out transfer learning by fine-tuning a pre-trained model with the dataset and see how the performance may differ.
