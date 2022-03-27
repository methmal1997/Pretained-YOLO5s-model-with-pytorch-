# Pretained-YOLO5s-model-with-pytorch-

Object detection has two main state
1.One-stage methods - these are mainly focused on the inference speed. Examples include: YOLO, RetinaNet, and SSD.
2.Two-stage methods - these are mainly focused on detection accuracy. Examples include: Mask R-CNN, Faster R-CNN, and Cascade R-CNN.


YOLO is a fast and accurate approach to object detection. The algorithm only looks at an image once and detects all the objects that are present along with their location.

YOLO works by splitting images into a grid where each grid cell identifies an object by itself. The grid cells predict all the bounding boxes and give each of them a confidence score to determine the accuracy of each prediction.
YOLOv5, the latest release of the YOLO family is a group of compound-scaled object detection models trained on the COCO dataset

![2022-02-21-17-32-29-xd1it3cnuuc](https://user-images.githubusercontent.com/71443389/160272609-28513c6b-c966-42b7-9452-c486228dfefd.png)



you have to install required packages

first you have python 3.7.0 or later version
installed relevant cuda version
In here i used cuda 11.0

After that install tha pytorh using

'pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu113' command

Then you can run the jupyter file in the 1 directory. You have to specify the image that tou want to detect.
(This pretrained model of pytorch)


But when you want to run Git clone file change directory to like '..YOLO5 with pytorch\Github clone\yolov5>' .
Then in terminal, pip install -r requirements.txt

After installation,

python detect.py --source 0 ,  for using web cam detection in terminal.

python detect.py --weights yolov5s.pt --img 640 --conf 0.25 --source data/images/download.jpg,  for detecting own image.
