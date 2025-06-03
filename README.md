# Autonomous Vehicle Collision Detection using YOLOv3 🚗🛑

This project simulates a basic autonomous vehicle control system that detects pedestrians and stops to avoid collisions. It uses a camera feed to detect objects and makes real-time driving decisions using YOLOv3.

## 🔍 Overview

A camera mounted on a simulated vehicle captures images. These frames are processed using the YOLOv3 object detection model to detect pedestrians. If a pedestrian is detected with high confidence, a signal is sent to stop the vehicle via a longitudinal controller module.

## 📁 File Descriptions

| File | Description |
|------|-------------|
| `yolo_detector.py` | Captures video frames and detects objects using YOLOv3 |
| `longitudinal controller.py` | Listens for detection signals and stops the vehicle |
| `coco.names` | Labels for object classes used in YOLO (e.g., person, car) |
| `yolov3.cfg` & `yolov3.weights` | YOLOv3 model configuration and weights |
| `collision_detection.mp4` / `.webm` | Demo videos showing system response |
| `PEAS Analysis.pdf` | PEAS analysis of the system’s performance and environment |

## 🚀 How to Run

> **Requirements**:
> - Python 3.x  
> - OpenCV (`cv2`)  
> - NumPy  
> - YOLOv3 model files (`.cfg`, `.weights`, `coco.names`)

```bash
# Run the detector
python3 yolo_detector.py

# Run the controller
python3 "longitudinal controller.py"
```

## 📌 Author

Hemangi Patel  
GitHub: [@hpatel1997](https://github.com/hpatel1997)
