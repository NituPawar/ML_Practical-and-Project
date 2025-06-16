
# 🐾 Animal Image Classification using Logistic Regression

## 📌 Project Overview

This project aims to build a machine learning model to classify images of animals using **Logistic Regression**. The classification is based on extracted image features, and the model is trained and tested on a sample dataset of animal images.

The model helps understand how Logistic Regression can be used for multi-class image classification tasks with feature-engineered data.

---

## 🧠 Algorithms Used

- **Logistic Regression** (Multinomial)
- (Optionally) **Artificial Neural Networks** if included
- **Scikit-learn** library for model building
- **StandardScaler** for feature normalization

---

## 📁 Dataset

- A collection of animal images (e.g., cat, dog, lion, elephant, etc.)
- Images are resized and preprocessed to extract numerical features.
- Total: 50+ images (balanced across classes)
- Labels: Categorical (e.g., `'cat'`, `'dog'`, `'lion'`, etc.)

---

## 🛠️ Tools & Libraries

- Python 3.x
- NumPy
- Pandas
- Matplotlib / Seaborn
- scikit-learn
- Jupyter Notebook / Google Colab

---

## 🔍 Steps Performed

1. **Image Loading & Preprocessing**
   - Resizing
   - Flattening to feature vectors
   - Label encoding

2. **Data Splitting**
   - Training set and testing set using `train_test_split`

3. **Feature Scaling**
   - Standardizing features using `StandardScaler`

4. **Model Training**
   - Logistic Regression (`LogisticRegression()`)

5. **Model Evaluation**
   - Accuracy score
   - Confusion Matrix
   - Classification Report

6. **Prediction**
   - Predict class of test images
   - Compare predictions with actual labels

---

## 📊 Evaluation Metrics

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **Confusion Matrix**

---

## ✅ Conclusion

The Logistic Regression model successfully classified the animal images with good accuracy. This demonstrates that even simple linear models can perform well on image data when features are properly preprocessed. It serves as a foundational approach for image classification tasks and can be further enhanced using deep learning methods.

---

## 📌 Future Work

- Use Convolutional Neural Networks (CNNs) for end-to-end learning.
- Implement data augmentation to improve model generalization.
- Deploy the model using a web interface (Flask or Streamlit).

---

## 🧑‍💻 Author

**Pruthviraj Tarode**  
B.Tech CSE – 3rd Year  
MGM's College of Engineering, Nanded  
