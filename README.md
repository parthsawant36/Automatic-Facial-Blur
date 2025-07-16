# 😷 Real-Time Face Blur using OpenCV and DNN

This project uses Python and OpenCV's DNN module to blur detected faces in real-time from a webcam feed. It ensures privacy by applying Gaussian blur only on the detected face regions while keeping the rest of the frame untouched. FPS (Frames Per Second) is also displayed to monitor performance in real-time.

## 🎯 Features
- Real-time face detection using a pre-trained DNN model
- Gaussian blur applied only to faces
- Live FPS counter on the original frame
- Seamless video stream from webcam
- Lightweight and efficient

## 🧠 How It Works
1. Capture frames from webcam using `cv.VideoCapture`.
2. Convert the frame to a blob and use the DNN model to detect faces.
3. Create a mask around detected faces.
4. Apply Gaussian blur only to the face regions using bitwise operations.
5. Combine blurred face regions with the rest of the frame.
6. Display both original and blurred frames, along with real-time FPS.

## 🧰 Requirements
- Python 3.x
- OpenCV (`opencv-python`)
- NumPy
- Pre-trained DNN face detector:
  - `deploy.prototxt.txt`
  - `res10_300x300_ssd_iter_140000_fp16.caffemodel`

Install dependencies:
```bash
pip install opencv-python numpy
