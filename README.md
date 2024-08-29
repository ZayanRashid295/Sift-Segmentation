# SIFT and Image Segmentation

This project demonstrates how to perform feature detection using SIFT (Scale-Invariant Feature Transform) and segment images based on color using the HSV color space. It also includes methods for evaluating segmentation accuracy against ground truth masks.

## Description

### SIFT Keypoints Detection

SIFT is a powerful algorithm used to detect and describe local features in images. It is invariant to scale and rotation, making it suitable for various image processing tasks such as object recognition and image stitching. In this project, SIFT is used to:
- Detect keypoints in an image.
- Compute descriptors for these keypoints to capture the local image features.

### Image Segmentation

The project performs image segmentation by converting the image to the HSV color space and applying color-based thresholding. This allows for distinguishing different regions in the image based on their color. Specifically, the segmentation focuses on:
- Identifying and isolating regions representing the sky.
- Identifying and isolating regions representing the sea.

### Accuracy Calculation

To evaluate the effectiveness of the segmentation, the project calculates the accuracy of the segmented regions by comparing them to ground truth masks. The accuracy is computed as the ratio of correctly classified pixels to the total number of pixels in the ground truth mask.

## Implementation

1. **Feature Detection with SIFT**:
   - Detected keypoints and computed descriptors using the OpenCV library.
   - Visualized keypoints on the image.

2. **Segmentation**:
   - Converted the input image to HSV color space.
   - Applied color-based thresholding to segment the sky and sea regions.

3. **Accuracy Calculation**:
   - Resized segmented masks to match the dimensions of the ground truth masks.
   - Computed accuracy by comparing the segmented regions to the ground truth.

## Usage

1. **Prepare the Environment**:
   - Clone the repository and install dependencies using `requirements.txt`.

2. **Place Images**:
   - Add your input image and ground truth masks to the `images` folder.

3. **Run the Script**:
   - Execute the `sift_segmentation.py` script to perform feature detection, segmentation, and accuracy calculation.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- Matplotlib


