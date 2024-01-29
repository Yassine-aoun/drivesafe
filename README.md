# Eyes Drowsiness Detection

This project utilizes computer vision techniques to detect eyes drowsiness in real-time using facial landmarks. It can be used as a safety measure to alert individuals who may be at risk of falling asleep.

## Prerequisites

- Python 3.x
- OpenCV
- Dlib
- Imutils
- Scipy

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/eyes-drowsiness-detection.git
    ```

2. Install the required dependencies:

    ```bash
    pip install opencv-python dlib imutils scipy
    ```

3. Download the shape predictor file (`shape_predictor_68_face_landmarks.dat`) from [[dlib's official website](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2)](http://dlib.net/face_landmark_detection.py.html) and place it in the project directory.

## Usage

1. Run the `drowsiness_detection.py` script:

    ```bash
    python drowsiness_detection.py
    ```

2. The application will open the webcam, and real-time drowsiness detection will begin.

3. Press 'q' to quit the application.

## How it Works

The script uses the dlib library to detect facial landmarks and calculate the eye aspect ratio (EAR) to determine if the eyes are showing signs of drowsiness. When the EAR falls below a threshold, an alert is triggered.

## Configuration

- `thresh`: EAR threshold for drowsiness detection.
- `frame_check`: Number of consecutive frames below the threshold to trigger an alert.

