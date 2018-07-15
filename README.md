# Face-Detection-Python

Simple implementaion of **tinyYolo** trained on **FDDB dataset** for face detection in **Keras**

## Step 1
Download tinyYOLO cfg and weights from darkent and convert them using [YAD2K](https://github.com/allanzelener/YAD2K)

## Step 2
Download FDDB data set and extract annotations in XML using [converter](https://github.com/penolove/FDDB_DataSet_4_faster_rcnn)

I have already included `.xml` annotation in the `FDDB_2010/Annotations` folder
Also included `.txt` files folowing darket in the `FDDB_2010/JPEGImages` folder


## Step 3

1. Enter the path to the `tiny-yolo.h5` converted from **Step 1** in the `.ipynb`
2. Similarly enter the path to `ImageFolder` and `Annotations` after extraction and conversion.
3. `train` and `test`

# Note
The `tinyYOLO` implementation is not accurate enough. I trained it for `200` iterations and found minimal but promising result. 

# Needed
1. Better implementation of `NMS` for `boundingBoxes`


Based on reference from [experiencor](https://github.com/experiencor/keras-yolo2)


