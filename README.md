# Logo and Number Plate Detection and Prediction
Jan 2023 - Feb 2023

This project focuses on detecting logos and reading number plates from images or videos. It uses advanced deep learning techniques such as ResNet for object detection and Xception CNN for car logo brand prediction. Additionally, EasyOCR is used for number plate recognition. The model is deployed via a Gradio interface for easy access.

---
## 📌 Features
-Logo Detection: Detects logos from a predefined set of 8 brands (Hyundai, Lexus, Mercedes, Opel, Skoda, Toyota, Volkswagen, Mazda).
-Brand Prediction: Identifies the brand of the detected logo using a trained CNN model with an accuracy of 86%.
-Number Plate Recognition: Uses the EasyOCR library to detect and read number plates.
-Object Detection: Utilizes the ResNet 640x640 architecture for training the object detection model.
-Gradio Interface: A user-friendly interface for easy image and video processing.

---
---


### 🛠️ Technologies Used
Deep Learning Frameworks: TensorFlow, Keras
Languages: Python
Libraries: EasyOCR, Gradio, OpenCV, NumPy, Matplotlib, PIL
Models: Convolutional Neural Networks (CNNs), ResNet, Xception
Tools: LabelImg (for dataset annotation)

### 📦 Installation
-Prerequisites
-Ensure you have the following installed:

Python 3.8+
pip (Python package manager)

### Clone the Repository
```bash
Copy code
git clone https://github.com/<your-username>/Logo-and-Number-Plate-Detection.git
cd Logo-and-Number-Plate-Detection
```

### Install Dependencies
```bash
Copy code
pip install -r requirements.txt
```
### 📸 How to Run
Image Detection
To perform logo and number plate detection on an image, run the following script:

```bash
Copy code
python detection-image.py
Video/ Webcam Detection
```

To perform detection using a webcam or video file, run the following script:

```bash
Copy code
python detection-vid.py
```
In this mode, the program will store images with the highest detection scores. To view predictions and recognition on these images, press 'q'. To perform predictions on a specific frame, press 'w'. To stop the process, press 'a'.

### Video Output
To generate a video with detection annotations, run the following script:

```bash
Copy code
python detection-to-video.py
```

This will generate an AVI video file named detected.avi in the working directory, with a frame rate of 20 FPS. Press 'a' to stop saving the video.

### 📂 Dataset
The dataset was self-collected and annotated using the LabelImg tool. It contains images of cars with logos from 8 different brands, as well as number plate images for OCR.

### 📈 Model Performance
Logo Brand Prediction: Achieved a validation accuracy of 86% using the Xception CNN architecture for brand classification.
Object Detection: Trained on the ResNet 640x640 architecture to detect logos and number plates with high accuracy.
