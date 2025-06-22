# 👤 Age & Gender Detection Web App

A clean and interactive web application built with **Streamlit** to detect **age and gender** from uploaded images using a pre-trained deep learning model in Keras. The app allows batch processing of multiple images and displays age/gender predictions with confidence scores.

---

## 🧠 Model Overview

The model used in this project was trained to perform:
- **Binary classification** for gender (Male/Female)
- **Regression** for age (in years)

It expects input images of shape **(48, 48, 3)**, preprocessed by resizing and normalization.

> 🔍 The model is stored in `.h5` format and loaded using `legacy_h5_format` from `keras.src.legacy.saving`.

---

## 📂 Project Structure

age-gender-detector/
├── Age_Sex_Detection.h5          # Pre-trained Keras model
├── app.py                        # Streamlit web app (main file)
├── Age_Gender_Detection.ipynb    # Jupyter notebook for demo & explanation
├── requirements.txt              # List of dependencies
└── README.md                     # You're here!

## 🚀 Getting Started
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/YOUR_USERNAME/age-gender-detector.git
cd age-gender-detector
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
Or manually:

bash
Copy
Edit
pip install streamlit tensorflow keras opencv-python pillow numpy
3. Run the Streamlit App
bash
Copy
Edit
streamlit run app.py
4. Open in Browser
After launching, Streamlit will open your default browser. If not, navigate manually to:

arduino
Copy
Edit
http://localhost:8501
## 📓 Notebook Version
You can also check out the included Jupyter notebook Age_Gender_Detection.ipynb for:

Model loading and structure

Single image prediction

Preprocessing steps

Visualizations and interpretation

To run the notebook:

bash
Copy
Edit
jupyter notebook Age_Gender_Detection.ipynb
## 🛠️ Notes
The model is not 100% accurate and may make mistakes, especially with low-quality or out-of-distribution images.

Works best with clear frontal face images.

You can improve performance by integrating a face detector (e.g., MTCNN, Haar cascades) before passing input to the model.

## 📦 Dependencies
Python 3.7+

Streamlit

TensorFlow / Keras

Pillow

NumPy

OpenCV

See requirements.txt for a complete list.
