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

* **Language:** ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

* **Data Manipulation:** ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)

* **Visualization:** ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat) ![Seaborn](https://img.shields.io/badge/Seaborn-5B8DB8?style=flat)

* **Deep Learning:** ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-D00000?style=flat&logo=keras&logoColor=white)

* **Evaluation:** ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white) (`accuracy_score`, `classification_report`, `confusion_matrix`)

* **Environment:** ![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-F37626?style=flat&logo=jupyter&logoColor=white) ![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white)

---

*To explore the detailed code, feel free to download the notebook file on this repo, or check out my [Kaggle](https://www.kaggle.com/code/maximendacleu/digit-recognizer).*
