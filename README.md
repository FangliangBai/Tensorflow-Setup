# Implement of DeepLab ResNet training on Tensorflow

## Content
1. Introduction
2. Dataset
3. Prerequisite
4. Train
5. Evaluate
6. Test

## Introduction
This implement folows the guide by [DrSleep/tensorflow-deeplab-resnet](https://github.com/DrSleep/tensorflow-deeplab-resnet) and use transfer learning for a custome medical dataset.


## Dataset
There are two datasets employed to train the networks.
1. augmented PASCAL VOC 2012 dataset with 10582 images for training and 1449 images for validation. All data you need can be downloaded from [here](). We use this dataset to validate that tensorflow works properly. 
1. Retouch fluid retinal OCT dataset. The `.raw` data can be download from [ReTouch](). The dataset that can be directly used for training can be downloaded from [here](). We use this dataset to fine-tune the ResNet to segment medical content.
