# Automatic Number Plate Recognition

This repository contains a Python script for automatic number plate recognition using OpenCV, Tesseract OCR, and EasyOCR. The script processes images of vehicles to detect and extract number plates, and then performs Optical Character Recognition (OCR) to read the text from these plates.

## Features

- **Pre-processing**: Converts images to grayscale, applies bilateral filtering, and edge detection to enhance number plate visibility.
- **Contour Detection**: Identifies potential number plates using contour detection and filters them based on shape and area.
- **Cropping and OCR**: Crops detected number plates and applies OCR using Tesseract and EasyOCR to extract the text.
- **Visualization**: Draws contours and OCR results on the original image and displays the processed images using Matplotlib.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- imutils
- tqdm
- pytesseract
- easyocr
- matplotlib

You can install the required Python packages using pip:

```bash
pip install opencv-python-headless numpy imutils tqdm pytesseract easyocr matplotlib
```
## Usage

### Clone the Repository

```bash
git clone https://github.com/yourusername/automatic-number-plate-recognition.git
cd automatic-number-plate-recognition
```

### Update Directory Path

Modify the directory variable in the script to the path where your images are stored.

### Run the Script

Execute the script using Python:

```bash
python ANPR.py
```

The script will process images in the specified directory, detect number plates, and display the results with OCR text overlay.

## Side Note: imagePreprocessing.py

The repository also includes a generic imagePreprocessing.py script. This script provides basic image preprocessing functionalities that can be used for various image processing tasks. It is designed to be a versatile tool for enhancing image quality before applying specific algorithms such as number plate detection.
