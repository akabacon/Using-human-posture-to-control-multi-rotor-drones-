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
# Make a adjust with physical camera 
codec = 0x47504A4D  # MJPG
cap.set(cv2.CAP_PROP_FPS, 30.0)
cap.set(cv2.CAP_PROP_FOURCC, codec)
cap.set(cv2.CAP_PROP_FRAME_WIDTH, 1920)
cap.set(cv2.CAP_PROP_FRAME_HEIGHT, 1080)
cap.set(cv2.CAP_PROP_EXPOSURE, 0)

model = YOLO("yolov8m-pose.pt")
===
# Pose Model
