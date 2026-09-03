# Augmented Grapevine Disease Classification with Custom CNN & MobileNetV2

An end-to-end Computer Vision project to detect and classify grapevine leaf diseases using Custom CNN and **MobileNetV2 Transfer Learning**, deployed via an interactive Streamlit web application.

---

## Project Overview

This repository evaluates custom convolutional layers against pre-trained **MobileNetV2 Transfer Learning** feature representations to identify plant pathology conditions, maintaining high diagnostic accuracy and memory efficiency.

* **Dataset:** Augmented Grapevine Disease Dataset
* **Architectures:** Custom CNN & MobileNetV2 Transfer Learning
* **Task Type:** Multi-Class Classification (4 Classes)
* **Deployment:** Streamlit Web Application

---

## Performance & Results

| Architecture | Training Accuracy | Validation Accuracy | Validation Loss |
| :--- | :--- | :--- | :--- |
| **Custom CNN** | ~97.10% | 97.70% | ~0.0820 |
| **MobileNetV2 (Transfer Learning)** | **99.05%** | **99.25%** | **0.0255** |

* **Classes (4):** Black Rot, Esca (Black Measles), Leaf Blight (Isariopsis Leaf Spot), Healthy
* **Loss Function:** `sparse_categorical_crossentropy`

---

## Key Features

* **Dual Architecture Comparison:** Benchmarks a custom CNN against pre-trained **MobileNetV2** representations.
* **Memory-Efficient Data Streaming:** Uses `tf.data.Dataset` pipelines with `.cache()` and `.prefetch()` to manage system RAM effectively.
* **Regularization:** Incorporates Dropout (0.3) layers to prevent overfitting.
* **Interactive UI:** Streamlit interface for uploading grapevine leaf scans and obtaining immediate diagnostic predictions with confidence scores.

---

## Tech Stack

* **Python 3.x**
* **TensorFlow / Keras**
* **Streamlit**
* **Pillow (PIL) & NumPy**
* **Matplotlib, Seaborn, Scikit-Learn**

---

## Dataset Structure

* **Split Ratio:** 80% Training, 20% Validation
* **Target Resolution:** 128 x 128 x 3 (RGB)

---

## Running the Web App Locally

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/grapevine-disease-classification.git](https://github.com/your-username/grapevine-disease-classification.git)
   cd grapevine-disease-classification
