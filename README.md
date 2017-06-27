# Implement of DeepLab ResNet training on Tensorflow

## Content
1. Introduction
2. Dataset
3. Prerequisite
4. Train
5. Evaluate
6. Test

## Introduction
This implement folows the guide by [DrSleep/tensorflow-deeplab-resnet](https://github.com/DrSleep/tensorflow-deeplab-resnet) and use transfer learning for a custome medical dataset. You can download the repo from [here](https://github.com/DrSleep/tensorflow-deeplab-resnet.git). All the files and settings are the same as above work other than specified in this document.


## Dataset
There are two datasets employed to train the networks.
1. augmented PASCAL VOC 2012 dataset with 10582 images for training and 1449 images for validation. Images can be downloaded from [here](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/VOCtrainval_11-May-2012.tar). Labels can be download from [here](https://www.dropbox.com/s/oeu149j8qtbs1x0/SegmentationClassAug.zip?dl=0#). Following the structure in [tensorflow-deeplab-resnet/dataset/train.txt](https://github.com/DrSleep/tensorflow-deeplab-resnet/blob/master/dataset/train.txt) to create folder and put in corresponding `.png` files. This dataset is used to validate that tensorflow works properly. 
1. Retouch fluid retinal OCT dataset. The `.raw` files can be download from [ReTouch](). The `.png` files that can be directly used for training can be downloaded from [here](). This dataset is used to fine-tune the ResNet to segment medical content.

## Prerequisite
1. you should have Tensorflow installed in your PC and make. Take a look of its version and make sure the `DrSleep/tensorflow-deeplab-resnet` supports your version. You can check the latest version it supports from [`Update` section of tensorflow-deeplab-resnet/README.md](https://github.com/DrSleep/tensorflow-deeplab-resnet/blob/master/README.md#updates).
