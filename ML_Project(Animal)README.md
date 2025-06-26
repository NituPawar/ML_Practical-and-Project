# 🐾 Animal Image Recognition Using CNN

This project utilizes a Convolutional Neural Network (CNN) built with TensorFlow and Keras to classify images of various animals. The goal is to demonstrate the effectiveness of CNNs in image-based recognition tasks using a custom dataset.

---

## 📌 Project Overview

- **Title:** Animal Image Recognition Using CNN  
- **Submitted by:** Rajsingh Ganeshsingh Thakur (TY CSE-A, Roll No. 103)  
- **Subject Incharge:** Ms. Nitu L. Pariyal  
- **Institution:** M.G.M’s College of Engineering, Nanded  
- **Academic Year:** 2024–2025

---

## 🎯 Objective

To design and train a CNN model that can accurately classify images of animals like cats, dogs, lions, and elephants using supervised learning techniques.

---

## 📂 Dataset

- Labeled image folders by animal class (e.g., cats, dogs).
- Loaded using `image_dataset_from_directory()` in TensorFlow.
- Images resized to `128x128` and normalized.
- Dataset split:
  - 80% Training
  - 20% Validation

---

## 🧪 Preprocessing Steps

- Resize to 128×128 pixels.
- Normalize pixel values with `Rescaling(1./255)`.
- Shuffle and batch images during training.

---

## 🧠 CNN Model Architecture

1. **Rescaling Layer:** Normalize pixel values.
2. **Conv2D + MaxPooling (×3):** 16, 32, 64 filters respectively.
3. **Flatten Layer**
4. **Dense Layer:** 64 units with ReLU.
5. **Output Layer:** Softmax for multi-class classification.

**Input Shape:** `(128, 128, 3)`  
**Output:** Animal class probabilities

---

## ⚙️ Training Details

- **Optimizer:** Adam
- **Loss Function:** Sparse Categorical Crossentropy
- **Epochs:** 5
- **Batch Size:** 32
- **Accuracy:** ~90% training, ~85% validation

---

## 📊 Visualization

Training and validation accuracy/loss plotted per epoch to confirm model learning and generalization.

---

## 🔍 Prediction

The trained model `animal_cnn_model.h5` is used for:
- Predicting new animal images.
- Outputting class probabilities using Softmax.

---

## 🛠 Tools and Libraries

- **Python 3.x**
- **TensorFlow + Keras**
- **Matplotlib** for visualization

---

## 📈 Results and Evaluation

- High accuracy in classifying unseen animal images.
- No overfitting detected.
- Performs best on clear and well-lit images.

---

## 🚀 Future Improvements

- Add data augmentation (rotation, flip, etc.)
- Train for more epochs
- Apply transfer learning (e.g., VGG16, MobileNet)
- Deploy as a real-time web application
- Use confusion matrix and classification report for better evaluation

---

## 📚 References

1. Géron, Aurélien – *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow*  
2. Chollet, François – *Deep Learning with Python*  
3. Mitchell, Tom M. – *Machine Learning*  
4. Goodfellow et al. – *Deep Learning*  
5. Zhang, Zhihua – *A Gentle Introduction to Deep Learning Using Keras*

---

## ✅ Conclusion

This project demonstrates that CNNs are highly capable for image classification tasks. The results validate their practical use in real-world applications, especially in recognizing animal species from images. Further enhancements can take this project from a prototype to a production-level classifier.

---

> 📌 _For academic and learning purposes only. All code and models are created by Rajsingh Ganeshsingh Thakur under guidance of Ms. Nitu L. Pariyal._