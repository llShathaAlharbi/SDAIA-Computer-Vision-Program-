# Computer Vision Program - Portfolio & Assignments 🚀
[![SDAIA Academy Supported](https://img.shields.io/badge/Supported_By-SDAIA_Academy-007A3D?style=for-the-badge&logo=github)](https://github.com/SDAIAAcademy)

---

Welcome to my portfolio for the Computer Vision Program provided by SDAIA Academy ([SDAIA Academy GitHub](https://github.com/SDAIAAcademy)). This repository showcases my practical assignments and projects, ranging from foundational image processing to deep learning classification and object detection models.

---

## 🛠️ Environment & Tools
* Development Environment: Google Colab / Python 3.x
* Core Libraries: OpenCV (`cv2`), NumPy, Matplotlib, Ultralytics YOLO, PyTorch
* Version Control: Git & GitHub

---

## 📂 Repository Structure

* 📁 images/ : Contains test input images for Assignment 1 and Assignment 2.
* 📜 Assignment_1.ipynb : Pixel Manipulation & Image Filtering.
* 📜 Assignment_2.ipynb : YOLO26 Object Detection & Natural Language Summary.
* 📜 Assignment_3.ipynb : CIFAR-10 Classification, YOLO Training & Confusion Matrix Evaluation.
* 📄 README.md : Documentation and repository overview.

---

##  Smart Restaurant Video Analytics System

### 📌 Project Overview
A comprehensive Computer Vision and Video Analytics pipeline designed for automated indoor restaurant monitoring (specifically tested on fast-food environments like Burger King). The system processes fixed-camera CCTV footage to perform multi-task operational tracking while actively preserving customer privacy.

### 🎯 Key Features & Requirements Met
1. Queue Counter: Monitors the customer waiting line on the left side using region-based tracking (`ROI`) to count active customers in real-time.
2. Customer & Staff Tracking: Assigns a unique tracking ID (`track_id`) to individuals within the scene to monitor movement.
3. Table Occupancy Detection: Automatically analyzes the dining area on the right to distinguish between available and occupied tables.
4. Crowd Congestion Alert: Triggers a real-time visual warning on the video stream whenever the queue length exceeds a predefined threshold.
5. Privacy-Preserving Face Anonymization: Automatically detects human faces and applies a Gaussian Blur (`cv2.GaussianBlur`) to protect customer privacy.

### 🛠️ Tech Stack & Libraries
* Python
* OpenCV (`cv2`) for frame processing, region drawing, blurring, and text overlays.
* Ultralytics YOLO (`yolov8n.pt`) for object detection and multi-object tracking.
* NumPy for spatial coordinate management and polygon testing (`cv2.pointPolygonTest`).

### 🚀 How to Run
1. Ensure your input video file (e.g., `-2470060199592079249.mov`) is located in the same directory.
2. Run the processing script in your Google Colab environment:
   ```bash
   pip install ultralytics opencv-python numpy
   python your_script_name.py
---

## 📝 Assignments Details

### 🔹 Assignment 1: Advanced Pixel-Level Manipulation
> Independent Task: Matrix operations, array slicing, and spatial filtering.
* Notebook: Assignment_1.ipynb
* Objective: Manipulate image matrices directly at the array level using NumPy and OpenCV.
* Steps & Requirements:
  1. Load, inspect, and display two input images (`Image 1` and `Image 2`) and print their shape/dimensions.
  2. Crop a $30 \times 30$ patch from a random location in Image 1 using array slicing and paste it into the center of Image 2 (saved as `Image3`).
  3. Convert all three images (`Image 1`, Image 2, and `Image 3`) to grayscale.
  4. Apply a custom $3 \times 3$ sharpening kernel exclusively to Image 3 to enhance its edges.

---

### 🔹 Assignment 2: Object Detection & Scene Summary
> Independent Task: Custom inference pipeline with manual bounding box rendering.
* Notebook: Assignment_2.ipynb
* Objective: Perform object detection using Ultralytics YOLO26 on a custom image and programmatically generate a descriptive text summary.
* Steps & Requirements:
  1. Upload a custom input image (e.g., basketball player with a ball).
  2. Run inference using the YOLO26 model (`yolo26n.pt`).
  3. Apply custom confidence thresholding (CONFIDENCE_THRESHOLD >=0.50).
  4. Manually draw bounding boxes and class labels on detected objects using OpenCV (without using built-in plot functions).
  5. Programmatically generate a natural language summary of all detected items below the image.

---

### 🔹 Assignment 3: CIFAR-10 Classification & Evaluation
> Independent Task: Pre-trained inference, model fine-tuning, and multi-class confusion matrix analysis.
* Notebook: Assignment_3.ipynb
* Objective: Work with the CIFAR-10 dataset using a YOLO classification model to test initial accuracy, fine-tune the model, and evaluate performance across all 10 categories.
* Steps & Requirements:
  * Part 1: Initial Testing and Accuracy Calculation
    1. Load the CIFAR-10 dataset.
    2. Randomly sample 10 images from the dataset.
    3. Run classification inference on these 10 images using a baseline/pre-trained YOLO classification model.
    4. Compare predicted labels against ground truth labels and report the baseline accuracy for the subset.
  * Part 2: Model Training and Confusion Matrix Evaluation
    1. Train (or fine-tune) a YOLO classification model on the CIFAR-10 dataset.
    2. Perform a comprehensive evaluation on the test/validation split.
    3. Generate, visualize, and analyze a multi-class Confusion Matrix to evaluate model performance across all 10 CIFAR-10 categories.

---

## 📸 Test Images
Sample images used for testing Assignment 1 and Assignment 2 can be found in the [`images/`](./images) directory:
* [Download Image 1](./images/image1.jpg)
* [Download Image 2](./images/image2.jpg)
* [Download Basketball Image](./images/basketball.jpg)

---

## 💻 How to Run
1. Open any notebook (`Assignment_1.ipynb`, Assignment_2.ipynb, or `Assignment_3.ipynb`) directly in Google Colab.
2. Run the code cells sequentially.
3. For Assignment 1 & 2, upload the required test images when prompted during execution.
