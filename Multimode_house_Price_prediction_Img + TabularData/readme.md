#  Multimodal House Price Prediction

## 📌 Overview

This project builds a **multimodal machine learning model** to predict house prices by integrating **tabular data** and **image data**. It was developed during a hands-on internship at Developer Hub Corporation (June–July 2025), mimicking real-world real estate valuation systems.

---

## 📷 Multimodal Architecture

- **Tabular Features**: Square footage, number of bedrooms/bathrooms, location, etc.
- **Image Features**: Exterior images of the property
- **Combined Model**:
  - Tabular model using `Dense` layers (via Keras)
  - Image model using `CNN` layers (TensorFlow/Keras)
  - Merged features to produce final price prediction

---

## 🧠 Model Design

1. **Tabular Submodel**
   - Input: Normalized tabular data
   - Layers: Dense layers + ReLU + Dropout

2. **Image Submodel (CNN)**
   - Input: Resized property images (e.g., 224x224x3)
   - Layers: Conv2D → MaxPooling → Flatten

3. **Fusion Layer**
   - Concatenated both outputs
   - Passed through Dense layers
   - Output layer with a single neuron for price regression

---

## 🧰 Tools & Libraries

- TensorFlow, Keras
- Pandas, OpenCV
- Sklearn for preprocessing
- Matplotlib for visualization
