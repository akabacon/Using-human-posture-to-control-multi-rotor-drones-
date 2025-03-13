capture_interval = 7: 
===
### Sets the time interval for image capture, controlling the capture frequency to prevent performance issues caused by capturing too frequently.


new_range = (300, 300): 
===
### Defines the size of the capture area, with width and height, controlling the range of the capture view.


abs_mid = (960, 540):
===
### Represents the center position of the image or display, typically used for positioning or as a reference point.

cap = cv2.VideoCapture(0)
===
### Make a adjustment with physical camera 
### codec = 0x47504A4D  # MJPG
### cap.set(cv2.CAP_PROP_FPS, 30.0)
### cap.set(cv2.CAP_PROP_FOURCC, codec)
### cap.set(cv2.CAP_PROP_FRAME_WIDTH, 1920)
### cap.set(cv2.CAP_PROP_FRAME_HEIGHT, 1080)
### cap.set(cv2.CAP_PROP_EXPOSURE, 0)

model = YOLO("yolov8m-pose.pt")
===
### This is the choosed Pose Model

Dektop Requirements
===

```
#python and setup
#conda create -n drone python=3.9
#conda install -c conda-forge cudatoolkit=11.6
#conda install cudatoolkit==11.6
#conda install pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.7 -c pytorch -c nvidia

#model
pip install chardet
pip install ultralytics
pip install opencv-python

#flycontroll
pip install dronekit
pip install pymavlink

# Initializing libiomp5md.dll
pip install numpy --upgrade
```
