# Computer Vision Program - Portfolio & Assignments 🚀

Welcome to my portfolio for the Computer Vision Program provided by SDAIA Academy ([SDAIA Academy GitHub](https://github.com/SDAIAAcademy)). This repository showcases my practical implementations, hands-on assignments, and future projects—spanning image processing, deep learning object detection, video analysis, and computer vision applications.

---

## 🛠️ Environment & Tools
* Development Environment: Google Colab / Python 3.x
* Core Libraries: OpenCV (`cv2`), NumPy, Matplotlib, Ultralytics YOLO26
* Version Control: Git & GitHub

---

## 📂 Repository Structure

* 📁 images/ : Contains sample input images used for testing (`image1.jpg`, image2.jpg, `basketball.jpg`).
* 📜 Assignment_1.ipynb : Pixel Manipulation & Image Filtering.
* 📜 Assignment_2.ipynb : YOLO26 Object Detection & Summary Generation.
* 📄 README.md : Documentation and program overview.
  
📝 Course Work & Assignments
🔹 Assignment 1: Advanced Pixel-Level Manipulation
 Notebook: ⁠Assignment_1.ipynb⁠
 Objective: Perform direct array manipulation, slicing, grayscale transformations, and edge sharpening using NumPy and OpenCV.
 Key Steps:
1. Load, inspect, and display two input images (⁠image1.jpg⁠ and ⁠image2.jpg⁠).
2. Crop a 30x30 patch from a random location in Image 1 using array slicing and paste it into the center of Image 2 (saved as ⁠Image3⁠).
3. Convert all three images to grayscale.
4. Apply a custom 3x3 sharpening kernel specifically to ⁠Image3⁠.
🔹 Assignment 2: Object Detection & Natural Language Summary
 Notebook: ⁠Assignment_2.ipynb⁠
 Objective: Implement an object detection pipeline using Ultralytics YOLO26, apply custom confidence thresholding, plot bounding boxes manually, and generate a natural language scene description.
 Key Steps:
1. Upload a custom input image (⁠basketball.jpg⁠).
2. Perform inference using the ⁠yolo26n.pt⁠ model.
3. Apply custom confidence thresholding (CONFIDENCE_THRESHOLD >= 0.50).
4. Manually draw bounding boxes and render class labels using OpenCV (without built-in result plots).
5. Programmatically generate a descriptive text summary of detected objects below the image.
📸 Test Images
You can access and download the exact test images used in these assignments from the ⁠images/⁠ directory:
 Download Image 1
 Download Image 2
 Download Basketball Image
💻 How to Run
1. Open any ⁠.ipynb⁠ notebook directly in Google Colab.
2. Run the cells sequentially.
3. When prompted, upload the corresponding test images from the ⁠images/⁠ directory
