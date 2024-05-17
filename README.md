# Face Recognition Attendance System

This is a Flask-based web application for managing attendance using face recognition. It uses OpenCV for face detection, a KNN model for face recognition, and SSIM for signature verification. The application captures images using a webcam and compares faces and signatures to maintain attendance records.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)

## Features
- **Face Detection and Recognition:** Uses OpenCV and a KNN model for recognizing faces.
- **Signature Verification:** Compares signatures using SSIM to verify identities.
- **Attendance Management:** Records attendance data in CSV files.
- **Web Interface:** User-friendly interface for adding users, listing users, and viewing attendance.

## Installation
To get started with the Face Recognition Attendance System, follow these steps:

1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/face-recognition-attendance.git
    ```

2. **Navigate to the project directory:**
    ```sh
    cd face-recognition-attendance
    ```

3. **Create a virtual environment:**
    ```sh
    python3 -m venv venv
    ```

4. **Activate the virtual environment:**
    - On Windows:
        ```sh
        venv\Scripts\activate
        ```
    - On macOS and Linux:
        ```sh
        source venv/bin/activate
        ```

5. **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

6. **Download the Haar Cascade file:**
    Download the `haarcascade_frontalface_default.xml` file from the OpenCV GitHub repository and place it in the project directory.

7. **Run the Flask app:**
    ```sh
    python app.py
    ```

The application should now be running on `http://localhost:5000`.

## Usage
### Adding a New User
1. Open the web application.
2. Go to the "Add User" page.
3. Enter the new user's name and roll number.
4. Capture images using the webcam.
5. Upload the user's signature.
6. Submit the form to save the user data and train the model.

### Taking Attendance
1. Go to the home page.
2. Click on the "Take Attendance" button.
3. The system will use the webcam to recognize faces and mark attendance.

### Verifying Signatures
1. Go to the "Verify Signature" page.
2. Enter the user's name.
3. Upload a signature to verify.
4. The system will compare the uploaded signature with the reference signature and display the result.

## Technologies Used
- **Python:** Programming language.
- **Flask:** Web framework for Python.
- **OpenCV:** Library for computer vision tasks.
- **scikit-learn:** Machine learning library for Python.
- **scikit-image:** Image processing library for Python.
- **Pandas:** Data manipulation and analysis library.
