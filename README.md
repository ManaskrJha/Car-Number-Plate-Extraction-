# Number-Plate-Extraction


This script performs number plate recognition on an image using OpenCV and EasyOCR. It detects the number plate in the image, performs optical character recognition (OCR) on the plate, and displays the recognized text on the image.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)

## Introduction
Number plate recognition is a computer vision task that involves detecting and extracting number plates from images or videos and then recognizing the characters on the plates. This script utilizes OpenCV for number plate detection using a Haar cascade classifier and EasyOCR for text recognition.

The script follows these steps:
1. Initialize the cascade classifier using the pre-trained XML file for number plate detection.
2. Initialize the EasyOCR reader object for text recognition.
3. Read the input image.
4. Convert the image to grayscale for better processing.
5. Detect number plates using the cascade classifier.
6. Iterate through each detected number plate.
7. Draw a bounding box around the number plate on the image.
8. Crop the number plate region from the image.
9. Perform OCR on the cropped number plate image using EasyOCR.
10. Retrieve the recognized text from the OCR result.
11. Display the recognized text on the image.
12. Save the final output image with the recognized number plate and text.

## Installation
1. Clone the repository: `git clone https://github.com/example/repo.git`.
2. Install the required dependencies:
   - OpenCV: `pip install opencv-python`.
   - EasyOCR: `pip install easyocr`.

## Usage
1. Navigate to the project directory: `cd repo`.
2. Place the `numberplate_haarcade.xml` file in the same directory as the script.
3. Set the `img_path` variable in the script to the path of the input image file.
4. Run the script: `python number_plate_recognition.py`.
5. The output image with the recognized number plate and text will be saved as `output.jpg`.

## Contributing
Contributions to this project are welcome. You can contribute by adding new features, improving the existing code, or fixing any issues. To contribute, follow these steps:
1. Fork the repository.
2. Create a new branch for your feature: `git checkout -b feature-name`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push the changes to your fork: `git push origin feature-name`.
5. Submit a pull request.

