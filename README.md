# Real-Time Object Detection with MobileNet SSD

This repository contains code for real-time object detection using the MobileNet SSD (Single Shot Detector) model. The script uses OpenCV's deep learning module to detect objects in real-time from a webcam video stream.


## Installation

1. Clone the repository:

```bash
git clone https://github.com/eyagammoudi2002/object_detection.git
cd object_detection
```

2. Install the required packages:

```bash
pip install -r requirements.txt
```

## Usage

Run the script with the following command:

```bash
python object_detection.py --prototxt path/to/MobileNetSSD_deploy.prototxt.txt --model path/to/mobilenet_iter_73000.caffemodel --confidence 0.2
```

### Arguments

- `--prototxt`: Path to the Caffe 'deploy' prototxt file.
- `--model`: Path to the Caffe pre-trained model.
- `--confidence`: Minimum probability to filter weak detections (default is 0.2).

Example:

```bash
python object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model mobilenet_iter_73000.caffemodel --confidence 0.2
```

## Dependencies

- `imutils`
- `numpy`
- `opencv-python`
- `argparse`

Install the dependencies using:

```bash
pip install imutils numpy opencv-python argparse
```



