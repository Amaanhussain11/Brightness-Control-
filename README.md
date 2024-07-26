# Hand Gesture Controlled Screen Brightness

This project demonstrates a real-time hand gesture recognition system that controls the screen brightness based on the distance between the thumb and index finger. It uses OpenCV, Mediapipe, and Screen Brightness Control libraries.

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [How It Works](#how-it-works)
4. [Requirements](#requirements)
5. [Acknowledgements](#acknowledgements)

## Installation

1. *Clone the repository:*

    bash
    git clone https://github.com/Amaanhussain11/Brightness-Control-.git
    cd hand-gesture-brightness-control
    

2. *Install the required libraries:*

    bash
    pip install opencv-python mediapipe screen-brightness-control numpy
    

## Usage

1. *Run the script:*

    bash
    python3 index.py
    

2. *Control the brightness:*

    - Show your hand in front of the webcam.
    - Move your thumb and index finger apart to increase the brightness.
    - Move your thumb and index finger closer to decrease the brightness.

3. *Exit:*

    - Press 'q' to exit the application.

## How It Works

1. *Importing Libraries:*
   - cv2 for image processing and video capture.
   - mediapipe for hand landmark detection.
   - math for calculating the distance between points.
   - screen_brightness_control for adjusting screen brightness.
   - numpy for numerical operations.

2. *Initializing the Model:*
   - Initializes the Mediapipe hand detection model with specified parameters.

3. *Capturing Video:*
   - Uses OpenCV to capture video frames from the webcam.

4. *Processing Frames:*
   - Flips the image for a mirror effect.
   - Converts the image from BGR to RGB.
   - Processes the frame to detect hand landmarks.

5. *Detecting Hand Landmarks:*
   - If hands are detected, extract the landmarks' coordinates.
   - Draws landmarks and connections on the frame.

6. *Calculating Distance and Adjusting Brightness:*
   - Calculates the distance between the thumb tip and index finger tip.
   - Maps the distance to a brightness level using interpolation.
   - Sets the screen brightness based on the calculated level.

7. *Displaying Video:*
   - Displays the video with annotated landmarks and brightness control.
   - Exits when 'q' is pressed.

## Requirements

- Python 3.x
- OpenCV
- Mediapipe
- Screen Brightness Control
- NumPy

## Acknowledgements

- [Mediapipe](https://github.com/google/mediapipe) by Google for hand tracking.
- [OpenCV](https://opencv.org/) for computer vision tasks.
- [Screen Brightness Control](https://pypi.org/project/screen-brightness-control/) for managing screen brightness.

Feel free to customize this project and improve upon it. Happy coding!
