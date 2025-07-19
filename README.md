# 📩 SMS Spam Detection with Neural Networks

A machine learning project to detect spam SMS messages using text preprocessing, tokenization, and a neural network built with TensorFlow and Keras.

---

## 🧠 Project Overview

This project uses a neural network to classify SMS messages as **Spam** or **Ham** (not spam) based on their content. It is trained on the [UCI SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection).

---

## 🔧 Tech Stack

- Python 3.12
- TensorFlow / Keras
- Pandas / NumPy
- Scikit-learn

---

## 🗃️ Dataset

- 📄 5,572 labeled SMS messages
- Format: `v1 = label` (ham/spam), `v2 = message text`

---

## 🧹 Preprocessing Steps

- Lowercasing
- Removing punctuation and stopwords
- Tokenization
- Padding sequences
- Label encoding (ham = 0, spam = 1)
- **Balancing the dataset** via downsampling

---

## 🧪 Model Architecture

```text
Embedding Layer → GlobalAveragePooling1D →
Dense Layer (ReLU) → Output Layer (Sigmoid)
