# Traffic-Sign-Detection
## Overview
ZaloAI Challenge 2020 - Vietnam traffic sign 

## Datasets
Download Datasets: ```! kaggle datasets download -d hongduc4/traffic-sign-detection-zalo-challenge-2020 ```

Link Dataset Kaggle: [Link](www.kaggle.com/datasets/hongduc4/traffic-sign-detection-zalo-challenge-2020)

Dataset discovery in [EDA](https://github.com/ducbvh)

### Structure of dataset
Dataset contains:
*  csv annotation files for training set, validation set and test set, 
    *  `label_map.pbtxt` for TF2 object detection API
    
## Models
The models used in this project are trained on the following pretrained models:
* YOLOv5 small ([Ultralytics](https://github.com/ultralytics/yolov5))
* YOLOv5 medium ([Ultralytics](https://github.com/ultralytics/yolov5))
* YOLOv5 large ([Ultralytics](https://github.com/ultralytics/yolov5))
* SSD MobileNet 320x320 ([Tensorflow object detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md))

 You can find notebooks for training in the [Models](https://github.com/ducbvh)

## Results
The following table sums up the results for our models:
|Model|mAP@[.5:.95] validation|mAP@[.5:.95] public test| FPS|
|-|-|-|-|
|YOLO v5 small| 37.8| 35.4|25.2|
|YOLO v5 medium| 38.6| 37.2|23.5|
|YOLO v5 large |42.7 |35.1|20.2|
|SSD MobileNet |11.7|9.5|15.4|




## Structure of Reposity
* `models`: contains Jupyter notebook file on how to train and evaluate the models
    *  `Train_MobilenetV2.ipynb`: Train MobilenetV2
    *  `Train_YoloV5.ipynb`: Train YoloV5
* `EDA`: contains 
    *  exploratory data analysis result
    *  `YoloV5_conversion.ipynb`: format data for train YoloV5
    *  `data_processing.ipynb`: data explore and analysis
    *  `data_reduce.ipynb`: removing boxes with area smaller than 40
* `saved_models`: contains saved models or weights for models.
* `results`: contains some inference results



