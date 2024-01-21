# Capturing the Happiness: Real-time Facial Expression Recognition with OpenCV

## Overview

The "Capturing the Happiness" project utilizes OpenCV to perform real-time facial expression recognition, focusing on detecting smiles. The system captures video from the default camera, identifies faces using Haar cascades, and further detects smiles within the detected faces.

## Dependencies

Make sure you have the following dependencies installed:

- Python 3.x
- OpenCV (`pip install opencv-python`)
- Haar Cascade XML files for face and smile detection (included in the `dataset` folder)

## Usage

 Clone the repository:

   ```bash
   git clone https://github.com/j4ck4l-24/capturing_the_happiness/tree/main

   cd capturing_the_happiness

   pip install opencv-python numpy

   python capturing_happiness.py
```

## Haar Cascades

The project uses Haar cascades for face and smile detection. The pre-trained Haar cascade XML files are included in the `dataset` directory. You can replace them with more accurate or specialized cascades if needed.

- Face Cascade: `haarcascade_frontalface_default.xml`
- Smile Cascade: `haarcascade_smile.xml`

## Image Capture

Captured images are saved in the project directory. The filenames are in the format `n.jpg`, where `n` is an incrementing number starting from 500.

## Customization

Feel free to experiment and customize the parameters in the script (`capturing_happiness.py`) to improve face and smile detection based on your environment. You may consider adjusting the following parameters:

- `detectMultiScale` parameters for both face and smile detection
- Colors and thickness of rectangles used for visualizing face and smile detection in the live video stream
- Image capture conditions, such as the number of images to capture (`cnt >= 503` in the provided script)


