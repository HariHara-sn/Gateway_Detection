# Gate Surveillance Object Classification using OpenCV and YOLO on Raspberry Pi
## Overview:
### This project utilizes OpenCV and the YOLO (You Only Look Once) object detection architecture to classify and monitor objects passing through a gate using recorded video footage. The implementation is optimized for deployment on a Raspberry Pi, making it suitable for real-time video processing applications such as security monitoring and traffic management

## Installation:
### To run the Python code, make sure Python is installed and import the required libraries:
- Numpy
- Opencv
  
## Execution:
Run the program with the following command:
```bash
object_classification.py
```
## Functionality

1. **Initialize YOLO Network**: Load pre-trained YOLOv4 model weights and configuration for object detection using OpenCV’s DNN module.

2. **Video Capture**: Read frames sequentially from a recorded video file.

3. **Pre-processing**: Convert frames into a format compatible with the neural network by normalizing, resizing, and channel swapping.

4. **Object Detection**: Utilize the YOLO network to detect objects in the video frames, providing bounding box coordinates, confidence scores, and class IDs for detected objects.

5. **Post-processing**: Apply Non-maximum Suppression (NMS) to filter overlapping boxes based on confidence scores, ensuring each object is labeled once.

6. **Display Results**: Draw bounding boxes and labels on the original frame, displaying the processed frame in a GUI window using OpenCV.

7. **Cleanup**: Release video capture and destroy OpenCV windows upon script completion.
