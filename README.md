# Custom-Object-Detection-from-Drone

A real-time object detection system using a Tello drone and OpenCV. This project enables autonomous object detection and tracking using a pre-trained SSD MobileNet V3 model.

## Features

- Real-time object detection using a Tello drone
- Pre-trained SSD MobileNet V3 model for accurate detection
- Support for 91 different object classes (COCO dataset)
- Real-time video streaming and display
- Confidence threshold adjustment for detection accuracy
- Non-Maximum Suppression (NMS) for better detection results
- Battery status monitoring
- Automatic drone takeoff and altitude adjustment

## Prerequisites

- Python 3.x
- Tello drone
- OpenCV (cv2)
- djitellopy library
- cvzone library

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Custom-Object-Detection-from-Drone.git
cd Custom-Object-Detection-from-Drone
```

2. Install the required dependencies:
```bash
pip install opencv-python djitellopy cvzone
```

## Project Structure

- `main.py` - Main script for object detection and drone control
- `coco.names` - List of object classes (91 classes from COCO dataset)
- `frozen_inference_graph.pb` - Pre-trained model weights
- `ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt` - Model configuration file
- `LICENSE` - MIT License file

## Usage

1. Ensure your Tello drone is powered on and connected to your computer's WiFi network
2. Run the main script:
```bash
python main.py
```

3. The drone will:
   - Connect to the Tello drone
   - Display battery status
   - Take off and move to a safe altitude
   - Start real-time object detection
   - Display detected objects with confidence scores

## Configuration

You can adjust the following parameters in `main.py`:
- `thres` - Confidence threshold (default: 0.55)
- `nmsThres` - Non-Maximum Suppression threshold (default: 0.2)

## Notes

- Make sure you have enough space for the drone to take off safely
- Keep the drone within WiFi range
- Monitor battery levels during operation
- The system uses the COCO dataset for object detection, supporting 91 different object classes

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to submit issues and enhancement requests!