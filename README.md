# 🧠 Handwritten Digit Recognizer

A neural network-based handwritten digit recognizer built using TensorFlow and Keras, trained on a custom dataset of grayscale images labeled 0–9.

---

## 📂 Project Structure

Handwritten Digit Recognizer/ │ ├── dataset.csv # CSV containing image paths and digit labels ├── handwritten_model.keras # Trained model file ├── img/ # Folder containing digit images ├── main.ipynb # Jupyter notebook with all the code ├── requirements.txt # Python package dependencies └── README.md # Project documentation

---

## 🛠️ Libraries Used

- TensorFlow / Keras
- OpenCV
- Pandas
- NumPy
- scikit-learn
- Matplotlib

---

## 📊 Dataset

- Images are grayscale and resized to **28x28 pixels**
- Labels are in the range **0 to 9**
- CSV file (`dataset.csv`) contains image paths and their corresponding labels

---

## 🚀 Model Architecture

```text
Flatten (28x28 input)
→ Dense(256, relu)
→ Dropout(0.2)
→ Dense(128, relu)
→ Dense(32, relu)
→ Dense(10, softmax)

