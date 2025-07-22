# Hindi Spoken Digit Classification

This project focuses on classifying Hindi spoken digits (शून्य, एक, दो, तीन...) using a Recurrent Neural Network (LSTM) trained on a custom, real-world dataset of voice recordings. The goal is to build a personalized and practical speech recognition system, tailored for regional language applications and accessibility-focused tools.


---

## 📁 Dataset
- A custom dataset was recorded by multiple students in varied acoustic environments, making the model robust to real-world noise and voice diversity.

- Each .wav file corresponds to a digit spoken in Hindi (0 to 9).

- Data augmentation was applied to increase sample diversity and improve generalization.


---

## 🧠 Project Overview
Audio data was preprocessed using MFCC (Mel-frequency cepstral coefficients) for feature extraction.

An RNN model based on stacked LSTM layers was trained to classify the spoken digits.

The model achieved:

✅ Training Accuracy: 91.65%

✅ Test Accuracy: 89.97%

The trained model was saved as best_model.h5.


---

## 🔁 Project Flow

1️⃣ Audio Preprocessing:

Each .wav file is converted into MFCC features.

Padding is applied to ensure consistent input length for the model.

2️⃣ Label Encoding:

Spoken digits (ek, do, etc.) are mapped to integer labels (0–9).

One-hot encoding prepares the targets for classification.

3️⃣ Model Design:

A sequential LSTM-based RNN model was used:

- Layers:

Two stacked LSTM layers with dropout

Final Dense layer with softmax activation

- Loss: categorical_crossentropy

- Optimizer: adam

4️⃣ Training:

Trained on augmented MFCC features



Achieved ~90% accuracy on unseen Hindi recordings



Saved model: best_model.h5


## 📊 Model Performance

### 📈 Accuracy & Loss
<img width="576" height="455" alt="accuracy_plot" src="https://github.com/user-attachments/assets/772a6063-0ad6-4b50-a46f-10c4dbd7d14d" />


### 🔀 Confusion Matrix
<img width="653" height="551" alt="confusion_matrix" src="https://github.com/user-attachments/assets/a7dca196-0bf0-44ca-a690-455105317d64" />


---

## 🧠 Tech Stack Used
Python

NumPy, Matplotlib

Librosa (for audio processing and MFCC feature extraction)

TensorFlow / Keras (for RNN model)

Scikit-learn (for evaluation metrics)


---

## 🚀 Potential Applications

- Accessibility Tools for differently-abled or visually impaired users who prefer or require Hindi speech interfaces.

- Educational Aids for teaching Hindi counting to children or language learners.

- Voice-activated Systems or smart devices in regional/rural Indian contexts.

- Data Entry Alternatives for Hindi-speaking users in government or local agencies.


---

## 📌 Project Highlights

✔️ Real-world, custom Hindi audio dataset

✔️ End-to-end audio classification pipeline

✔️ High accuracy with robust LSTM architecture

✔️ Promotes regional language inclusion in AI

