# Digit Recognizer - MNIST CNN
<img width="560" height="279" alt="header" src="https://github.com/user-attachments/assets/71f3f8ca-fe44-4f63-9717-d8005dbf106d" />

## Context
From [Kaggle](https://www.kaggle.com/competitions/digit-recognizer)

## Objective
This notebook implements a **Convolutional Neural Network (CNN)** for the **MNIST Digit Recognition** Kaggle competition. The goal is to classify handwritten digits (between 0 and 9) from grayscale images with high accuracy.

## Notebook Structure & Workflow
1. **Data Loading & Exploration:** Loading the MNIST dataset, visualizing sample images, and checking class distribution.
2. **Data Preprocessing:** Reshaping images to (28, 28, 1), normalization, and one-hot encoding of labels.
3. **Data Augmentation:** Applying random rotation, zoom, and translation to improve generalization.
4. **Model Architecture:** A CNN with 3 convolutional blocks (32→64→128 filters), batch normalization, max pooling, dropout, and dense layers.
5. **Training:** Using Adam optimizer, categorical cross-entropy loss, early stopping, and learning rate reduction.
6. **Evaluation:** Validation accuracy, classification report, and confusion matrix to analyze digit-level performance.

## Key Insights & Results
- The model achieves **approximately 99.08% validation accuracy**.
- Strong performance across all digits (**precision/recall/F1 > 0.99** for most classes).
- Data augmentation and batch normalization significantly help reduce overfitting.
- The confusion matrix shows very few misclassifications, mostly between visually similar digits.

## Tech Stack & Libraries
- **Language:** Python
- **Data Manipulation:**: `pandas`, `numpy`
- **Visualization:** `Matplotlib`, `Seaborn`
- **Deep Learning:** `TensorFlow` / `Keras`
- **Evaluation:** `scikit-learn` (`accuracy_score`, `classification_report`, `confusion_matrix`)
- **Environment:** Kaggle Notebook

---

*To explore the detailed code, feel free to download the notebook file on this repo, or check out my [Kaggle](https://www.kaggle.com/code/maximendacleu/digit-recognizer).*
