# Face Emotion Recognition using Mini-Xception

This project is a real-time face emotion recognition system built using a pre-trained Mini-Xception CNN model. It detects human emotions from facial expressions using OpenCV for face detection and TensorFlow/Keras for prediction.

The application is implemented using Streamlit, allowing users to either upload an image or capture one using their webcam

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#Tech Stack)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Model Information](#Model-Information)
- [Acknowledgment](#Acknowledgment)
- [License](#license)

## Overview

The application detects faces in an image and categorizes them into one of seven emotion classes
- Angry  
- Disgust  
- Fear  
- Happy  
- Sad  
- Surprise  
- Neutral

The model works on **48x48 grayscale images**, making it lightweight and efficient for real-time use.This model can be used for educational purposes

## Features

- Upload image file (jpg, jpeg, png) for emotion detection  
- Capture image using webcam using Streamlit’s built-in camera input. 
- Real-time face detection using OpenCV  
- Emotion prediction results with bounding boxes and confidence score  
- Simple and interactive UI using Streamlit  

## Tech Stack

- Python  
- TensorFlow / Keras  
- OpenCV  
- Streamlit  
- NumPy / Pandas  

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/emotion_recognition_app.git
   cd emotion_recognition_app
   ```

2. **Create and Activate a Virtual Environment (optional but recommended):**

   ```bash
   python -m venv venv
   # On macOS/Linux:
   source venv/bin/activate
   # On Windows:
   venv\Scripts\activate
   ```

3. **Install Dependencies:**

   ```bash
   pip install --upgrade pip
   pip install -r requirements.txt
   ```

4. **Add Your Model:**

   Place your saved Keras model file (e.g., `model.h5`) in the root directory of the project. Ensure the path in `model.py` points to this file.

## Usage

To run the app, execute the following command in your terminal:

```bash
streamlit run app.py
```

This will open a new browser window with the Streamlit interface where you can:
- **Upload an Image:** Choose an image file to process and view the emotion detection results.
- **Webcam Mode:** Capture a picture using your webcam and view the detection results.

## Project Structure

```
face-emotion-recognition/
│
├── app.py
├── model.py
├── requirements.txt
├── README.md
├── _mini_xception.100_0.65.hdf5
└── face-recognition.ipynb
```

## Model Information

Architecture: Mini-Xception (CNN)
Input: 48x48 grayscale face images
Output: Emotion classification (7 classes)

## Acknowledgment

This project is based on and inspired by the original work:

https://github.com/sathiyasubramanaya/face_emotion_recognition_mini_Xception

The implementation has been modified, cleaned, and structured for learning and demonstration purposes.

## License

This project is licensed under the MIT License.
```

