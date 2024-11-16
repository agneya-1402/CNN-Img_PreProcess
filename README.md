# Computer Vision Data Preprocessing and Basic CNN Model

This repository demonstrates a complete workflow for preprocessing image data and training a basic convolutional neural network (CNN) model using TensorFlow. The guide includes steps like loading data, normalizing, resizing, augmenting, splitting, and feeding it into a simple CNN model.

---

## Table of Contents
- [Features](#features)
- [Setup and Installation](#setup-and-installation)
- [Workflow Overview](#workflow-overview)
- [Code Structure](#code-structure)
- [Usage Instructions](#usage-instructions)
- [Model Summary](#model-summary)
- [Results](#results)
- [License](#license)

---

## Features
- Dataset Handling**: Uses CIFAR-10 dataset for demonstration.
- Preprocessing**: Includes normalization, resizing, and one-hot encoding.
- Augmentation**: Applies techniques like rotation, zoom, and flipping.
- Modeling**: Implements a basic CNN for image classification.
- Visualization**: Plots training and validation accuracy and loss.
- Evaluation**: Tests the model on unseen data.

---

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/agneya-1402/CNN-Img_PreProcess.git
   cd CNN-Img_PreProcess
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Verify installation by running the script:
   ```bash
   python CNN-Img_PreProcessing.ipynb
   ```

---

## Workflow Overview

1. Data Loading**: CIFAR-10 dataset is used for demonstration purposes.
2. Normalization**: Image pixel values are scaled to the range [0, 1].
3. Resizing**: Images are resized to a uniform shape of 64x64 pixels.
4. Augmentation**: Random transformations like rotation and flipping are applied.
5. Splitting**: Data is split into training, validation, and test sets.
6. CNN Model**: A sequential model with convolutional, pooling, and dense layers.
7. Training**: The model is trained with augmented data.
8. Evaluation**: The model's performance is tested on unseen data.

---

## Usage Instructions

1. Modify the dataset or preprocessing parameters in `CNN-Img_PreProcessing.ipynb` as needed.
2. Run the script:
   ```bash
   CNN-Img_PreProcessing.ipynb
   ```
3. Check the training progress and visualizations generated by the script.

---

## Model Summary

- Architecture: 
  - Convolutional layers with ReLU activation.
  - MaxPooling layers for dimensionality reduction.
  - Dense layers for classification.
- Output: Softmax activation for 10 classes in CIFAR-10.

---

## Results

- Training Accuracy**: Achieved ~75% accuracy on the training set.
- Validation Accuracy**: Achieved ~80% accuracy on the validation set.
- Test Accuracy**: Achieved ~78% accuracy on unseen data.

The model can be fine-tuned further for better performance by:
- Using advanced architectures (e.g., ResNet, VGG).
- Fine-tuning hyperparameters.
- Experimenting with more augmentations.

---

## License

This project is licensed under the MIT License. Feel free to use and modify the code.
