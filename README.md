# ISL-Recoginition-Project

## 📚 Overview
This project builds a deep learning model to **recognize Indian Sign Language (ISL) alphabets** using a Convolutional Neural Network (CNN).

The model achieves **high accuracy** (~100% on training, ~98% on validation) and generalizes well to unseen hand gestures.

---

## 📂 Project Structure
```
/ISL_Project
    ├── train_model.ipynb   # Training and evaluation code
    ├── ISL_DATA/           # Dataset (train/validation images)
    ├── saved_model/        # Final saved model (.h5 or TensorFlow SavedModel)
    ├── sample_predictions/ # Sample outputs (optional)
    └── README.md           # This file
```

---

## 📈 Model Performance

| Metric | Accuracy |
|:------|:---------|
| Training Accuracy | 100% |
| Validation Accuracy | 98% |

- **Loss curves and accuracy graphs** are plotted for better visualization.
- **Classification Report** shows precision, recall, and F1-score for each class.

---

## 🏗️ Model Architecture
- 3 Convolutional layers
- 3 MaxPooling layers
- 1 Dense layer
- Dropout (0.6) to prevent overfitting
- Final Dense Softmax layer (for multi-class classification)

Optimizer: **Adam** with learning rate **0.0001**  
Loss Function: **Categorical Crossentropy**

---

## 🧪 Data Augmentation
To make the model more robust:
- Random rotations
- Zoom shifts
- Horizontal flips
- Width and height shifts
- Shear transformations

---

## 📷 Sample Predictions
The model can predict hand signs from new images.  
Random samples are taken from the validation set to check real performance.

---

## 📄 Future Improvements
- Test with real-time webcam input.
- Expand to full ISL words (not just alphabets).
- Deploy as a simple web app using Streamlit.

