# 🧠 Sign Language Binary Classification (NumPy – From Scratch)

## 📌 Overview
This project implements a simple neural network from scratch using only **NumPy**, with no use of high-level frameworks like TensorFlow or PyTorch. The task is a **binary classification** of hand-written digits (`4` vs. `5`) from the Sign Language Digits Dataset.

This work was submitted as **Part 1** of the mid-semester milestone in the *Basics of Deep Learning* course.

---

## 📂 Files
```
sign-language-numpy/
├── notebook.ipynb      # Main notebook with all code
├── report.pdf           # Final project report
├── README.md                                # Project description
├── requirements.txt                         # Python dependencies
```

---

## 📊 Dataset
- **Source:** Sign Language Digits Dataset
- **Classes Used:** Only digits `4` and `5` (binary classification)
- **Images:** 28x28 grayscale, flattened into 784-dim vectors
- **Preprocessing:**
  - Normalized pixel values to [0, 1]
  - Filtered only digits 4 and 5
  - Labeled: `4 → 0`, `5 → 1`
  - Train/Validation/Test split: 80% / 0% / 20%

---

## 🏗️ Model Architecture
- Input Layer: 784 neurons (flattened image)
- Hidden Layer: 32 neurons, **Sigmoid** activation
- Output Layer: 1 neuron, **Sigmoid** activation

### ⚙️ Training Details
- **Loss Function:** Binary Cross-Entropy
- **Optimizer:** Gradient Descent (custom implementation)
- **Learning Rate:** 0.01
- **Epochs:** 50
- **Framework:** Implemented fully using NumPy

---

## 📈 Evaluation & Results
- Accuracy: **97.5%** (on test set)
- Confusion Matrix:
  - TP = 94, TN = 101, FP = 2, FN = 3
- Visualized:
  - Loss curve across epochs
  - Example image + model prediction with confidence (0.9996)

---

## 🚀 How to Run
1. Open the notebook in **Google Colab**
2. Ensure the dataset is accessible via the provided link or manually upload
3. Run all cells in order:
   - Preprocessing
   - Training (forward + backward propagation)
   - Evaluation (metrics + plots)

---

## 📝 Key Concepts Implemented
- Forward propagation
- Backpropagation
- Sigmoid activation
- Cross-entropy loss
- Manual weight updates with gradient descent
- Accuracy & confusion matrix calculation (no external libraries)

---

## 👥 Authors
- **Shir Zohar**
- **Sivan Zagdon**

---

## 📜 License
This project was developed for educational purposes at Colman College, as part of the "Basics of Deep Learning" course.

