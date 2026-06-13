# 🖐️ Hand Gesture Recognition System

A Machine Learning project that classifies hand gestures from images using a **Random Forest Classifier** trained on the **LeapGestRecog Dataset**.

Built with **Python**, **Scikit-Learn**, **Streamlit**, **Matplotlib**, and **Seaborn**.

---

## 📋 Table of Contents

* Project Overview
* Dataset
* Gesture Classes
* Image Preprocessing
* Model Architecture
* Evaluation Metrics
* Project Structure
* Installation & Usage
* Tech Stack
* Future Improvements
* Author

---

# 🎯 Project Overview

Hand Gesture Recognition (HGR) is a Computer Vision task that identifies hand poses from images and maps them to meaningful gesture labels such as:

* 👋 Palm
* ✊ Fist
* 👍 Thumbs Up
* 👌 OK Sign
* ☝️ Index Finger

This project implements a complete Machine Learning workflow:

```text
Image
 ↓
Grayscale Conversion
 ↓
Resize (64×64)
 ↓
Flatten Features
 ↓
Feature Scaling
 ↓
Random Forest Classifier
 ↓
Gesture Prediction
```

### Applications

* Sign Language Recognition
* Touchless User Interfaces
* Human Computer Interaction
* Smart Systems
* Robotics & Automation

---

# 📂 Dataset

### LeapGestRecog Dataset

| Property     | Value                |
| ------------ | -------------------- |
| Dataset      | LeapGestRecog        |
| Source       | Kaggle               |
| Participants | 10                   |
| Classes      | 10 Hand Gestures     |
| Format       | Grayscale PNG Images |
| License      | CC0 Public Domain    |

---

# ✋ Gesture Classes

| ID | Label        |
| -- | ------------ |
| 01 | Palm         |
| 02 | L Shape      |
| 03 | Fist         |
| 04 | Fist Moved   |
| 05 | Thumb Up     |
| 06 | Index Finger |
| 07 | OK Sign      |
| 08 | Palm Moved   |
| 09 | C Shape      |
| 10 | Down         |

---

# 🖼️ Image Preprocessing

Every image undergoes the following preprocessing steps:

### 1. Image Loading

Images are loaded using Pillow.

### 2. Grayscale Conversion

RGB images are converted into grayscale format to reduce complexity.

### 3. Resizing

All images are resized to:

```text
64 × 64
```

### 4. Flattening

Each image is converted into a one-dimensional feature vector.

```text
64 × 64 = 4096 Features
```

### 5. Standardization

Features are normalized using StandardScaler to improve model performance.

---

# 🤖 Model Architecture

### Algorithm

**Random Forest Classifier**

### Hyperparameters

| Parameter         | Value    |
| ----------------- | -------- |
| n_estimators      | 200      |
| max_depth         | None     |
| min_samples_split | 2        |
| class_weight      | balanced |
| random_state      | 42       |

### Why Random Forest?

* Ensemble learning approach
* Reduces overfitting
* Handles high-dimensional data efficiently
* Provides robust predictions
* Performs well on image-derived feature vectors

---

# 📊 Evaluation Metrics

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

These metrics help measure both overall performance and class-wise prediction quality.

---

# 📁 Project Structure

```text
Hand-Gesture-Recognition-System/
│
├── app.py
├── train_model.py
├── requirements.txt
├── README.md
├── .gitignore
│
└── utils/
    ├── __init__.py
    └── predict.py
```

---

# ⚙️ Installation & Usage

### 1. Clone the Repository

```bash
git clone https://github.com/AkshitaDhiman18/Hand-Gesture-Recognition-System.git

cd Hand-Gesture-Recognition-System
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Train the Model

```bash
python train_model.py
```

### 4. Run the Streamlit Application

```bash
streamlit run app.py
```

Open:

```text
http://localhost:8501
```

---

# 🛠️ Tech Stack

| Technology   | Purpose              |
| ------------ | -------------------- |
| Python       | Core Programming     |
| Scikit-Learn | Machine Learning     |
| Streamlit    | Interactive Web App  |
| NumPy        | Numerical Operations |
| Pandas       | Data Processing      |
| Pillow       | Image Processing     |
| Matplotlib   | Visualization        |
| Seaborn      | Data Visualization   |

---

# 🚀 Future Improvements

* CNN-based Deep Learning Model
* Real-Time Webcam Prediction
* Mobile Application Integration
* Sign Language Translation
* Gesture Sequence Recognition
* Cloud Deployment

---

# 👩‍💻 Author

## Akshita Dhiman

Aspiring Machine Learning Engineer with a strong interest in Machine Learning, Data Science, Artificial Intelligence, and Software Development.

This project showcases practical experience in:

✔ Data Preprocessing
✔ Feature Engineering
✔ Machine Learning Model Development
✔ Model Evaluation
✔ Streamlit Application Development
✔ End-to-End Project Building

### GitHub

https://github.com/AkshitaDhiman18

---

⭐ If you found this project useful, consider giving it a star.

### “Building intelligent solutions through Machine Learning, one project at a time.”

Made with ❤️ by **Akshita Dhiman**

