# Real-Time Facial Recognition with OpenCV

- This project implements real-time facial recognition using OpenCV.
- Captures video from the laptop's camera.
- Detects faces using a pre-trained Haar Cascade classifier.
- Highlights detected faces with green rectangles in the live video feed.

## Features
- Real-time facial detection from webcam video feed.
- Uses Haar Cascade (`haarcascade_frontalface_default.xml`) for facial recognition.
- Displays detected faces with a green rectangle overlay.

## Requirements
- Python 3.x.
- OpenCV library (`cv2`).

## Installation
- Clone this repository:
  - `git clone <repository_url>`
  - `cd <repository_name>`
- Install dependencies:
  - `pip install opencv-python`

## How to Use
- Run the script: `python facial_recognition.py`.
- The webcam will start capturing video.
- Detected faces will be highlighted with green rectangles.
- To exit, press the **'q'** key.

## Project Structure
- `facial_recognition.py`: Main script for facial detection.
- `.gitignore`: Ensures unnecessary files (e.g., cache files, virtual environments) are not tracked in the repository.

## Dependencies
- OpenCV: A library for real-time computer vision.
- Installation: `pip install opencv-python`.
- Webcam access is required for video input.

## Customization
- Adjust the window size by modifying:
  - `width, height = 640, 480`
  - `video_capture.set(cv2.CAP_PROP_FRAME_WIDTH, width)`
  - `video_capture.set(cv2.CAP_PROP_FRAME_HEIGHT, height)`
- Modify detection sensitivity by tweaking:
  - `scaleFactor` and `minNeighbors` in the `detectMultiScale` method:
    - `faces = faceCascade.detectMultiScale(gray, scaleFactor=1.1, minNeighbors=5, minSize=(30, 30))`

## Acknowledgments
- This project uses the Haar Cascade classifier provided by OpenCV for facial detection.
- Learn more about it [here](https://github.com/opencv/opencv/tree/master/data/haarcascades).
