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

How to Use
1. **Prepare the image:**
    - Place your image of the chessboard in the "data" folder within the project directory.
    - Ensure the image file is named correctly or update the file path in the code accordingly.
2. **Run the notebook:**
    - Open the .ipynb file (Jupyter Notebook) in your preferred environment (e.g., Jupyter Lab, Google Colab).
    - Execute each code cell sequentially to run the image processing and square detection.
3. **View the results:** The program will display multiple windows with the following:
    - The original image
    - Grayscale version of the image
    - Histogram equalized image
    - Thresholded image
    - Image with contours drawn
    - Approximated corners on the chessboard
    - Color-coded chessboard (black and white squares highlighted)
    - Cropped chessboard and final detection results
4. **Check the accuracy:** After processing the image, the program will print the accuracy of the black and white square detection to the console.

## Example Output

```mathematica
Black squares: 32
White squares: 32
Black Square Accuracy: 100.00%
White Square Accuracy: 100.00%
Overall Accuracy: 100.00%
```

## Notes
The program expects a standard chessboard layout, where the number of black and white squares is 32 each.
The accuracy calculation assumes the chessboard has exactly 32 black squares and 32 white squares. If the detection result differs, the accuracy is adjusted accordingly.

## Troubleshooting
No image found: Ensure the image is stored in the "data" folder and that the file path is correct in the code.
Contour detection fails: This might happen if the image quality is poor or the chessboard is not fully visible. Try using a clearer image or adjusting the preprocessing parameters.