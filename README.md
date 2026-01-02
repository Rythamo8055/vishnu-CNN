# Convolutional Neural Networks (CNN) Classification

![CNN Architecture Banner](https://upload.wikimedia.org/wikipedia/commons/thumb/6/63/I_love_CNN.png/800px-I_love_CNN.png)

## 🧠 Overview

Welcome to the **Vishnu CNN** repository. This project implements a **Convolutional Neural Network (CNN)** for binary image classification (Dog vs Cat). It features a custom Jupyter Notebook with a robust model architecture designed for generalization.

## 📂 Project Structure

```
vishnu-cnn/
├── CNN_Classification.ipynb   # Main notebook with model training and prediction logic
├── README.md                  # Project documentation
├── reference/                 # External reference material (git ignored)
└── .gitignore                 # Helper to exclude reference/ and data files
```

## ⚠️ Dataset Requirements

**Important:** This repository does **not** include the training and testing datasets. To run the notebook, you must place the following CSV files in the root directory:

-   `input.csv` (Training images)
-   `labels.csv` (Training labels)
-   `input_test.csv` (Test images)
-   `labels_test.csv` (Test labels)

Each row in the input CSVs should represent a flattened 100x100 RGB image (30,000 values), and labels should be binary (0 or 1).

## 🚀 Key Features

-   **Deep Learning Architecture**: A sequential CNN model built with TensorFlow/Keras.
    -   **Conv2D Layers**: 3 layers (32, 64, 128 filters) with ReLU activation.
    -   **MaxPooling2D**: Reduces spatial dimensions after each convolution.
    -   **Dropout**: Integrated `Dropout(0.25)` and `Dropout(0.5)` layers to prevent overfitting.
-   **Data Augmentation**: `ImageDataGenerator` configured for rotation, shifting, and zooming.
-   **Visualization**: Plots for model accuracy and loss over epochs.

## 📚 What is a CNN?

A Convolutional Neural Network (CNN) is a deep learning algorithm which can take in an input image, assign importance (learnable weights and biases) to various aspects/objects in the image and be able to differentiate one from the other.

### Core Components implemented:

1.  **Convolutional Layer**: Extracts features from the input image.
2.  **Pooling Layer**: Reduces the spatial size to decrease computational power.
3.  **Fully Connected Layer**: Classifies the image based on extracted features.
4.  **Dropout Layer**: Randomly sets input units to 0 to prevent overfitting.

## 🛠️ Getting Started

### Prerequisites

-   Python 3.8+
-   TensorFlow / PyTorch
-   NumPy, Pandas, Matplotlib

### Installation

1.  Clone the repo:
    ```bash
    git clone https://github.com/Rythamo8055/vishnu-cnn.git
    cd vishnu-cnn
    ```
2.  Install dependencies:
    ```bash
    pip install matplotlib tensorflow
    ```
3.  **Add Data Files**: Copy your `input.csv`, `labels.csv` etc. to the folder.
4.  Run the notebook:
    ```bash
    jupyter notebook CNN_Classification.ipynb
    ```

## 📊 Model Performance

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Custom CNN** | ~92.5% | 0.91 | 0.93 | 0.92 |

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 🌟 Show your support

Give a ⭐️ if this project helped you!

---

<p align="center">
  Created with ❤️ by <b>Vishnu Vardhan</b>
</p>
