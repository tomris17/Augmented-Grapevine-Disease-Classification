# Augmented Grapevine Disease Classification with CNN & Streamlit Web App

This project builds a Convolutional Neural Network (CNN) using TensorFlow/Keras to detect and classify grapevine leaf diseases (such as Black Rot, Esca, Leaf Blight, and Healthy leaves) and deploys the trained model via an interactive Streamlit web application.

The primary goal of this repository is to demonstrate how to train a high-accuracy computer vision model on plant disease images while maintaining memory efficiency and providing an intuitive UI for real-time predictions.

---

## Key Features

* **Memory-Efficient Data Loading:** Uses tf.data.Dataset pipelines to stream and preprocess images without overloading system RAM.
* **Fast Training:** Optimized image resizing and batching for smooth execution.
* **High Performance:** Reaches high classification accuracy across all disease classes on the validation set.
* **Visual Evaluation:** Includes training curve plots and a clear confusion matrix to analyze model performance.
* **Interactive Web Interface:** User-friendly Streamlit interface to upload grapevine leaf images and retrieve immediate disease predictions with confidence scores.

---

## Performance & Results

* **Classes:** Black Rot, Esca (Black Measles), Leaf Blight (Isariopsis Leaf Spot), Healthy
* **Evaluation:** High precision and recall across all plant pathology classes.

---

## Tech Stack & Libraries

* **Python 3.x**
* **TensorFlow / Keras**
* **Streamlit**
* **NumPy**
* **Pillow (PIL)**
* **Matplotlib & Seaborn**
* **Scikit-learn**

---

## Dataset

The project utilizes the Augmented Grapevine Disease Dataset featuring images of healthy and diseased grapevine leaves across multiple categories.

* Data splits: 80% Training, 20% Validation
* Input image resolution: 128 x 128 x 3

---

## Web Application Setup

To run the Streamlit application locally:

1. Save your trained model as `grapevine_model.keras` in the project root directory.
2. Run the Streamlit app:

```bash
streamlit run app.py
