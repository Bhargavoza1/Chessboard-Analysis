# Chessboard Square Detection
 
This program processes an image of a chessboard to identify and classify its squares as black or white. It uses image processing techniques like contour detection, perspective transformation, and intensity analysis to achieve accurate results. The program then calculates the accuracy of the detected squares based on expected values.

## Features

- Converts the image to grayscale for easier analysis.
- Applies Contrast Limited Adaptive Histogram Equalization (CLAHE) for improved contrast.
- Uses thresholding and contour detection to identify the chessboard.
- Performs a perspective transformation to obtain a top-down view of the chessboard.
- Divides the cropped chessboard into an 8x8 grid and classifies each square as black or white based on its intensity.
- Calculates and displays the accuracy of the black and white square detection against expected values.

## Requirements

- Python 3.8+
- OpenCV for python
- NumPy
- matplotlib

You can install the required dependencies using:
```bash
pip install -r requirements.txt
```