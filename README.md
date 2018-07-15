# Face-Detection-Python

Simple implementaion of **tinyYolo** trained on **FDDB dataset** for face detection in **Keras**

## Step 1
Download tinyYOLO `cfg` and `weights`(yolo-darknet folder) from darkent and convert them using [YAD2K](https://github.com/allanzelener/YAD2K)

## Step 2
Download FDDB dataset and extract annotations in XML using [converter](https://github.com/penolove/FDDB_DataSet_4_faster_rcnn)

I have already included `.xml` annotation in the `FDDB_2010/Annotations` folder
Also included `.txt` files following darket in the `FDDB_2010/JPEGImages` folder


## Step 3

1. Enter the path to the `tiny-yolo.h5` converted from **Step 1** in the `.ipynb`
2. Similarly enter the path to `ImageFolder` and `Annotations` after extraction and conversion.
3. `train` and `test`

# Note
The `tinyYOLO` implementation is not accurate enough. I trained it for `200` iterations and found minimal but promising results. 

# Needed
1. Better implementation of `NMS` for `bounding-Boxes`. 
2. You can use a full-blown implemention of `YoloV2` or `YoloV3`, but will be needing atleast `5.5GB` of VRAM. Step-by-Step implementation for the same can be found at `experiencor-repo` mentioned below. I have implemented the same for `F1-RaceCar` detection [here](https://github.com/dAmnation69/Deep-Learning-Python/tree/master/05.Keras-Object%20Detection)


Based on reference from [experiencor](https://github.com/experiencor/keras-yolo2). Similar implementation can be found [here](https://github.com/joycex99/tiny-yolo-keras) but i haved made a few changes to `utils` and the code iteself.


