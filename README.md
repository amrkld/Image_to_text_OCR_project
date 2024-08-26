# Image to Text OCR Project

## Overview

This project is a Python application that uses Optical Character Recognition (OCR) to extract text from images. It leverages the following libraries:
- **PIL** (Pillow) for image handling
- **OpenCV** for image preprocessing
- **pytesseract** for OCR
- **tkinter** for creating a graphical user interface (GUI)

## Features

- Load image files (JPG, JPEG, PNG) via a file dialog.
- Preprocess images to improve OCR accuracy, including converting to grayscale, applying thresholding, and optional denoising.
- Extract text from the preprocessed image.
- Display the extracted text in a scrollable text area.

## Installation

To run this project, you need to have Python installed along with the necessary libraries. Install the required libraries using `pip`:

```bash
pip install pillow opencv-python pytesseract
```

**Note:** You also need to have [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) installed on your system. Ensure that `tesseract` is accessible from your system's PATH.

## Usage

1. Clone or download the project repository.
2. Open the project directory in your terminal or command prompt.
3. Run the script using Python:

   ```bash
   python script.py
   ```

   Replace `script.py` with the name of your Python file.

4. The application window will open. Click the "Open Image File" button to select an image file.
5. The application will process the image and display the extracted text in the scrollable text area.

## Code Explanation

- **preprocess_image(image_path)**: Reads and preprocesses the image, converting it to grayscale, applying thresholding, and optionally denoising.
- **extract_text_from_image(preprocessed_image)**: Uses pytesseract to extract text from the preprocessed image.
- **process_image(image_path)**: A helper function that combines image preprocessing and text extraction.
- **open_file()**: Opens a file dialog for image selection, processes the selected image, and updates the text area with the extracted text.

## GUI Details

- **Open Image File**: Button to open the file dialog and select an image.
- **Scrolled Text Area**: Displays the text extracted from the image.

## Troubleshooting

- **Tesseract Not Found**: Ensure that Tesseract is installed and correctly added to your system's PATH.
- **Library Errors**: Make sure all required libraries are installed. Use the provided `pip` command to install them.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. For significant changes or features, please open an issue to discuss it first.
