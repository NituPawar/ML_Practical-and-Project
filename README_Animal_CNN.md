
# 🐾 Animal Image Classification using CNN

## 📌 Project Overview

This project focuses on building a **Convolutional Neural Network (CNN)** model to classify images of various animals. The model is trained using **TensorFlow and Keras** on a custom dataset consisting of multiple animal categories. With a well-structured architecture and training process, the model achieves high accuracy and demonstrates the effectiveness of CNNs for visual recognition tasks.

---

## 🎯 Objective

To design, train, and evaluate a CNN-based model that classifies animal images into their respective categories with high accuracy. The project also aims to explore essential concepts in deep learning and apply them to a real-world image classification problem.

---

## 📁 Dataset

- **Classes:** Dogs, Cats, Elephants, Lions, etc.
- **Structure:** Labeled folders per animal class
- **Size Split:**
  - 80% for training
  - 20% for validation
- **Loaded Using:** `image_dataset_from_directory()` (TensorFlow)

---

## 🧹 Preprocessing

- Resize images to `128 × 128` pixels
- Normalize pixel values using `Rescaling(1./255)`
- Shuffle and batch data for efficient training

---

## 🧠 CNN Model Architecture

| Layer                 | Configuration                          |
|----------------------|-----------------------------------------|
| Input Layer          | Rescaling layer                        |
| Conv2D (Layer 1)     | 16 filters, 3×3 kernel, ReLU activation |
| MaxPooling2D         | Pool size: 2×2                          |
| Conv2D (Layer 2)     | 32 filters, 3×3 kernel, ReLU activation |
| MaxPooling2D         | Pool size: 2×2                          |
| Conv2D (Layer 3)     | 64 filters, 3×3 kernel, ReLU activation |
| MaxPooling2D         | Pool size: 2×2                          |
| Flatten              | -                                       |
| Dense Layer          | 64 neurons, ReLU activation             |
| Output Layer         | Softmax activation                      |

- **Input Shape:** (128, 128, 3)
- **Output:** Number of animal classes

---

## ⚙️ Training Details

- **Optimizer:** Adam
- **Loss Function:** Sparse Categorical Crossentropy
- **Epochs:** 5
- **Batch Size:** 32
- **Accuracy:**
  - Training: ~90%
  - Validation: ~85%
- **Observation:** No overfitting observed

---

## 📊 Visualization

- Plotted **Accuracy vs. Epoch** and **Loss vs. Epoch** graphs
- Training and validation performance improved steadily

---

## 🔍 Prediction

- The trained model (`animal_cnn_model.h5`) is used to predict new images
- Input images are resized and normalized before prediction
- Model returns the predicted class

---

## 🧰 Tools & Libraries

- TensorFlow & Keras
- Python 3.x
- Matplotlib

---

## ✅ Results and Evaluation

- High classification accuracy within few epochs
- Model performs well on clear, centered animal images
- Evaluation metrics can be expanded (confusion matrix, F1-score)

---

## 📌 Conclusion

The CNN model effectively classifies animal images with high accuracy and low training time. This demonstrates the strength of deep learning for visual tasks. The model is lightweight and ideal for basic applications involving animal classification.

---

## 🚀 Future Improvements

- Apply data augmentation for better generalization
- Train for more epochs
- Use transfer learning (VGG16, MobileNet, etc.)
- Add F1-score, precision-recall, and confusion matrix
- Deploy as a web app for live image testing

---

## 📚 References

- *Machine Learning* by Tom M. Mitchell  
- TensorFlow: https://www.tensorflow.org  
- Keras: https://keras.io  
- François Chollet – *Deep Learning with Python*  
- Dataset Source: Custom / Self-Collected / Public Datasets

---

## 👨‍💻 Submitted by

**Pruthviraj Shyamrao Tarode**  
Roll No: 102  
TY CSE - A  
MGM’s College of Engineering, Nanded  
Academic Year: 2024–25
