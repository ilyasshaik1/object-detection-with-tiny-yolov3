# object-detection-with-tiny-yolov3

# YOLOv3-Tiny Object Detection

This repository provides a simple implementation of **YOLOv3-Tiny** for real-time object detection using a webcam. The system detects objects in real-time and displays bounding boxes and labels around detected objects in the video stream.

## Features
- **Real-time object detection** using the YOLOv3-Tiny model.
- **Webcam video feed** for detecting objects.
- **Bounding boxes and labels** drawn on the detected objects.
- **Class detection** based on the COCO dataset labels.

## Requirements

- **Python 3.x**
- **OpenCV** (for video capture and processing)
- **NumPy** (for mathematical operations)

You can install the necessary dependencies using `pip`:

```bash
pip install opencv-python numpy
```

Additionally, you will need the following YOLO files:
- `yolov3-tiny.weights`
- `yolov3-tiny.cfg`
- `coco.names`

These files can be downloaded from the official YOLO repository or other sources that provide YOLOv3-Tiny pre-trained models.

## Setup

1. **Clone the repository**:

2. **Download YOLOv3-Tiny Model Files**:
    - Download the `yolov3-tiny.weights`, `yolov3-tiny.cfg`, and `coco.names` files and place them in the same directory as your Python script.

    You can download them from:
    - [YOLOv3-Tiny Weights](https://pjreddie.com/media/files/yolov3-tiny.weights)
    - [YOLOv3-Tiny Config](https://github.com/pjreddie/darknet/blob/master/cfg/yolov3-tiny.cfg)
    - [COCO Names File](https://github.com/pjreddie/darknet/blob/master/data/coco.names)

3. **Run the Object Detection Script**:

    After installing the required dependencies and downloading the necessary files, you can run the object detection script.

    ```bash
    python yolo_object_detection.py
    ```

    This will start the webcam feed, and you should see detected objects displayed with bounding boxes and class labels.

## Usage

- **Press 'q'** to exit the detection loop and stop the video feed.
- The program will display the object labels and bounding boxes for each detected object in real-time.

### Example Output:
When objects are detected, the script will display bounding boxes and their corresponding labels in the video stream. For example, if a person or a cat is detected, the label `person` or `cat` will be shown next to the object.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- YOLOv3-Tiny model and weights are from the [YOLO website](https://pjreddie.com/darknet/yolo/).
- The COCO dataset class names are from the [COCO dataset](http://cocodataset.org/).
- This implementation uses OpenCV and NumPy for real-time object detection and image processing.

---

