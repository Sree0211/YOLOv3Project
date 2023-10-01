# Object detection using YOLO

## Overview
This project utilizes YOLOv3 (You Only Look Once), a state-of-the-art object detection algorithm, with Darknet, an open-source neural network framework, for detecting objects in both images and videos. The project consists of two separate scripts, one for object detection in images and another for object detection in videos.

## Table of Contents
* Overview
* Table of Contents
* Installation
* Usage
* Object Detection in Image
* Object Detection in Video
* Configuration
* * License

## Installation
Clone Darknet Repository: Clone the Darknet repository, which includes the YOLOv3 implementation.

`git clone https://github.com/AlexeyAB/darknet.git`

Install Dependencies: Ensure you have all the necessary dependencies installed. You can use the requirements file provided in the repository.

`pip install -r requirements.txt`

## Usage
### Object Detection in Image
Place the image(s) you want to analyze in the input_images directory.

Run the image detection script:

`python yolo.py --image path/to/image --yolo path/to/yolo_weights_and_cfg --confidence --threshold`

The script will process the input images and save the output images with bounding boxes around detected objects in the output_images directory.
![Horses](https://github.com/Sree0211/YOLOv3Project/assets/43269126/2aa0eb58-a13a-4239-adc7-abd2e5920f4d)


### Object Detection in Video
Place the video(s) you want to analyze in the input_videos directory.

Run the video detection script:

`python yolo_video.py --input path/to/input_video --output /path/to/output --yolo path/to/yolo_weights_and_cfg --confidence --threshold`

The script will process the input videos and save the output videos with bounding boxes around detected objects in the output_videos directory.

## Configuration
Adjust configurations such as YOLOv3 model weights, thresholds, and file paths in the scripts as needed.

## License
This project is licensed under the MIT License.



