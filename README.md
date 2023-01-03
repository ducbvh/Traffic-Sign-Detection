# Traffic-Sign-Detection
ZaloAI Challenge 2020 - Vietnam traffic sign


## Datasets
Download Datasets: ```! kaggle datasets download -d hongduc4/traffic-sign-detection-zalo-challenge-2020 ```

Link Dataset Kaggle: [Link](www.kaggle.com/datasets/hongduc4/traffic-sign-detection-zalo-challenge-2020)

Dataset discovery in [EDA](https://github.com/ducbvh)

## Models
The models used in this project are trained on the following pretrained models:
* YOLOv5 small ([Ultralytics](https://github.com/ultralytics/yolov5))
* YOLOv5 medium ([Ultralytics](https://github.com/ultralytics/yolov5))
* YOLOv5 large ([Ultralytics](https://github.com/ultralytics/yolov5))
* SSD MobileNet 320x320 ([Tensorflow object detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md))

 You can find notebooks for training in the [Models](https://github.com/ducbvh)

## Results

The following table sums up the results for our models:
|Model|mAP@[.5:.95] validation|mAP@[.5:.95] public test|
|-|-|-|
|YOLO v5 small| 39.3| 35.8|
|YOLO v5 medium| 40.6| 38|
|YOLO v5 large |40.5 |37.5|
|SSD MobileNet |10.7 |7.77|
|SSD ResNet50 FPN |46.7| 20.8|
|EfficientDet D1 |13.2| 8.2|
|Faster R-CNN Resnet50 |26.9 |14.5|

The following table sums up the results for our models:
|Model|mAP@[.5:.95] validation|mAP@[.5:.95] public test|FPS|
|-|-|-|
|YOLO v5 small| 37.3| 32.4| 23.0|
|YOLO v5 medium| 38.5| 36.7| 22.1|
|YOLO v5 large |42.7 |37.5| 20.2|
|SSD MobileNet |12.1 |9.8| 18.5|
