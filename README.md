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

# Patient Data Encryption and Database

## Overview

This Python script demonstrates a simple implementation of patient data encryption and storage in a database. It utilizes the `cryptography` library to perform encryption and decryption using the Fernet symmetric key encryption scheme.

## How It Works

The code consists of two main classes:

1. **PatientDataEncryption:**
   - Initializes with a key (or generates a new one if not provided).
   - Uses Fernet cipher for encryption and decryption.
   - Provides methods to encrypt and decrypt patient data.

2. **PatientDatabase:**
   - Initializes an empty list to store patient data.
   - Offers methods to add patients to the database and display the current patient records.

## Example Usage

1. **Encryption Module Initialization:**
   - Creates an instance of the `PatientDataEncryption` class.

2. **Patient Database Initialization:**
   - Creates an instance of the `PatientDatabase` class.

3. **Sample Patient Data:**
   - Defines sample patient data in a dictionary format.

4. **Data Encryption:**
   - Encrypts patient data using the `PatientDataEncryption` instance.

5. **Adding Encrypted Data to the Database:**
   - Adds encrypted patient data to the database.

6. **Displaying Encrypted Patient Data:**
   - Displays the encrypted patient data stored in the database.

7. **Data Decryption:**
   - Decrypts the patient data using the `PatientDataEncryption` instance.

8. **Displaying Decrypted Patient Data:**
   - Prints the decrypted patient data.

## How to Use

1. Clone the repository.

    ```bash
    git clone https://github.com/your-username/patient-data-encryption.git
    cd patient-data-encryption
    ```

2. Install dependencies.

    ```bash
    pip install -r requirements.txt
    ```

3. Run the script.

    ```bash
    python patient_data_encryption.py
    ```

4. View the encrypted and decrypted patient data in the console.

## Dependencies

- Python 3.x
- cryptography library (`pip install cryptography`)

## License

This project is licensed under the [MIT License](LICENSE).

## Contributions

Feel free to modify and enhance the code to suit your specific requirements. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request. Thank you for using this patient data encryption and database example!




