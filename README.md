# Real-Time Alphabet Recognition System
Project Overview
This project implements a machine learning-based computer vision system capable of recognizing handwritten alphabets in real-time. It utilizes a Logistic Regression model trained on a large-scale image dataset and uses a live camera feed to capture, process, and predict handwritten characters within a defined region of interest.

Key Features
Real-time Prediction: Uses OpenCV to capture video frames and perform instantaneous classification of handwritten letters.

Automated Image Processing: Implements a grayscale conversion, resizing (28x28 pixels), and pixel scaling pipeline to prepare raw camera data for the model.

Machine Learning Pipeline: Features a full workflow including data loading from .npz and .csv formats, feature scaling, and model training using Logistic Regression.

Region of Interest (ROI) Focus: Draws a centralized bounding box on the camera feed to guide the user and ensure consistent data input.

Technologies Used
Python: Core programming language.

OpenCV (cv2): For video capture and image frame manipulation.

Scikit-learn: For the Logistic Regression classifier and performance metrics.

NumPy & Pandas: For handling numerical arrays and structured label data.

PIL (Pillow): For advanced image processing and array-to-image conversion.

What I Learned
Data Normalization: Learned the importance of scaling pixel values (0-255) to a 0-1 range to improve model convergence and accuracy.

Hardware-Software Interface: Gained experience in managing system camera resources and handling the live data stream loop.

Supervised Learning: Applied fundamental classification concepts to a multi-class problem involving 26 distinct alphabet classes.

How to Run
Ensure image.npz and labels.csv are in the project directory.

Install dependencies:

pip install opencv-python numpy pandas scikit-learn pillow

Run the script:

python alphabet_detection.py

Place a handwritten capital letter inside the green box shown on the camera feed to see the prediction displayed in the console.
