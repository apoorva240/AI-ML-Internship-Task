# AI-ML-Internship-Task
Welcome to the repository for my AI/ML internship task! This repository contains the code and documentation for a task assigned during my internship, showcasing my skills in artificial intelligence and machine learning.

# Thermal Image Processing with OpenCV

This Python script demonstrates a basic thermal image processing pipeline using the OpenCV library. The script fetches an image from a specified URL, converts it to grayscale, simulates a thermal image using a color map, applies additional image processing techniques, and displays various intermediate and final results.

## Dependencies
- `cv2` (OpenCV): Open-source computer vision library.
- `requests`: HTTP library for sending requests.
- `numpy`: Library for numerical operations.
- `BytesIO`: Input/output stream for handling binary data.
- `cv2_imshow`: Function for displaying images in Google Colab.

## Functions

### `process_thermal_image(image_url)`
Processes a simulated thermal image from the specified URL.

#### Parameters:
- `image_url` (str): The URL of the image to be processed.

#### Steps:
1. **Download Image:** Fetches the image from the provided URL.
2. **Convert to Grayscale:** Converts the original image to grayscale.
3. **Simulate Thermal Image:** Applies a color map (Jet colormap) to simulate a thermal image.
4. **Gaussian Blur:** Applies Gaussian blur to the grayscale image.
5. **Thresholding:** Creates a binary image by thresholding the blurred image.
6. **Contour Detection:** Finds contours in the binary image.
7. **Contour Visualization:** Draws contours on the original image.

#### Displayed Images:
- Original Image
- Grayscale Image
- Simulated Thermal Image
- Blurred Image
- Binary Image (Thresholded)
- Image with Contours

## Example Usage

Replace 'image_url' with the actual URL of an image you want to use:

<img src="https://media.istockphoto.com/id/517188688/photo/mountain-landscape.jpg?s=612x612&w=0&k=20&c=A63koPKaCyIwQWOTFBRWXj_PwCrR4cEoOw2S9Q7yVl8=" alt="Example Image" width="600"/>

```python
image_url = 'https://media.istockphoto.com/id/517188688/photo/mountain-landscape.jpg?s=612x612&w=0&k=20&c=A63koPKaCyIwQWOTFBRWXj_PwCrR4cEoOw2S9Q7yVl8='
process_thermal_image(image_url)

