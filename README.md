# 🧘‍♀️ Yoga Pose Classifier

> 📍 *Course Project – Image Processing (May 2024 – July 2024)*  
> 📊 Built for pose recognition using deep learning and joint-based geometry

---

## 📌 Project Overview

This project implements a **Yoga Pose Classifier** that can recognize human yoga poses using joint landmarks extracted from images. It combines **vector geometry**, **MediaPipe pose estimation**, and **CNN-based classification** trained on the **Yoga-82 dataset**.

---

## 🔍 Key Features

- ✅ **Joint Angle & Distance-Based Features** using MediaPipe for accurate geometric representation of poses.
- 🧠 **CNN-Based Classifier** trained from scratch for visual recognition of poses.
- 🗂️ **Yoga-82 Dataset** with 17,000+ images covering 82 yoga pose classes.
- 📈 Achieved:
  - **92% accuracy** on a subset of **18 commonly practiced poses**.
  - **73% accuracy** across all **82 pose categories**.
- 🧹 Robust **data preprocessing**:
  - Resizing & normalization
  - Data augmentation
  - Denoising filters

---

## 🏗️ Technical Stack

- **Language:** Python  
- **Libraries:** OpenCV, MediaPipe, NumPy, TensorFlow/Keras, Matplotlib  
- **Model:** CNN (Convolutional Neural Network)  
- **Pose Estimation:** Google’s [MediaPipe](https://mediapipe.dev/)

---

## 🚀 Project Pipeline

1. **Pose Detection:**  
   MediaPipe detects 33 keypoints (joints) per image.

2. **Feature Extraction:**  
   - Vector geometry calculates **angles** and **distances**.
   - These features can be optionally fused with image-based CNN predictions.

3. **Preprocessing:**  
   - Resize, normalize, augment images
   - Apply Gaussian blur and denoising filters

4. **Model Training:**  
   - Train CNN model with categorical cross-entropy
   - Evaluate on validation and test sets

5. **Evaluation:**  
   - Classification accuracy
   - Confusion matrix for pose-specific analysis

---

