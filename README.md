# 🧠 Deepfake Detection System using Vision Transformers (ViT)

---

## 📌 Overview

This project implements an end-to-end deep learning pipeline to **detect deepfake images using Vision Transformers (ViT)**. It demonstrates the application of transformer-based architectures in computer vision to address real-world challenges in **media authenticity and misinformation detection**.

---

## 🚀 Key Features

* 📷 Image classification using **Vision Transformer (ViT)**
* ⚖️ Handles class imbalance with **Random Oversampling**
* 🔄 Complete ML pipeline: data loading → preprocessing → training → evaluation
* 📊 Performance evaluation using:

  * Accuracy
  * F1 Score (Macro)
  * Confusion Matrix
  * Classification Report
* 🔍 Inference pipeline for real-time predictions
* ☁️ Model deployment on Hugging Face Hub

---

## 🧰 Tech Stack

* **Python**
* **PyTorch**
* **Hugging Face Transformers & Datasets**
* **Scikit-learn**
* **Imbalanced-learn**
* **Matplotlib**

---

## 📂 Project Structure

```
project/
│
├── main.py              
├── Dataset/             
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📊 Dataset

* Contains **real and deepfake images**
* Organized as:

```
Dataset/
  ├── real/
  ├── fake/
```

⚠️ Dataset not included due to size constraints
👉 Use publicly available datasets (e.g., Kaggle Deepfake datasets)

---

## ⚙️ Installation

### 1. Clone the repository

```
git clone https://github.com/DemonKira911/Deepfake-Detection-System-using-Vision-Transformers.git
cd Deepfake-Detection-System-using-Vision-Transformers
```

### 2. Install dependencies

```
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the training pipeline:

```
python main.py
```

### Pipeline Workflow:

* Data loading & preprocessing
* Image augmentation
* Class balancing
* Model fine-tuning (ViT)
* Evaluation & metrics generation
* Model saving & inference

---

## 🧪 Model Details

* **Model:** google/vit-base-patch16-224-in21k
* **Architecture:** Vision Transformer
* **Epochs:** 5
* **Batch Size:** 32 (train), 8 (eval)

---

## 📈 Evaluation Metrics

* Accuracy Score
* F1 Score (Macro)
* Confusion Matrix
* Classification Report

---

## 🔍 Inference

```python
from transformers import pipeline

pipe = pipeline("image-classification", model="your-model-path")
pipe(image)
```

---

## ☁️ Model Deployment

Trained model is deployed on **Hugging Face Hub** for easy access and reuse.

---

## 💼 Resume Description

> Developed a deep learning-based deepfake detection system using Vision Transformers (ViT), implementing data balancing, augmentation, and end-to-end model deployment on Hugging Face.

---

## 🔮 Future Improvements

* Add CNN baselines (ResNet, EfficientNet) for comparison
* Hyperparameter optimization
* Web deployment (Streamlit / Flask)
* Larger and more diverse datasets
* Extend to video-based deepfake detection

---

## 🤝 Contributions

Contributions are welcome. Feel free to fork and submit pull requests.

---

## 📜 License

Licensed under the MIT License.
