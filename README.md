# Pothole vs Normal Road CNN

## Project Overview

This project is a binary image classification system that detects whether a road image contains a pothole or represents a normal road.

The project uses Convolutional Neural Network (CNN) based image classification with image preprocessing and data augmentation.

## Objective

The main objective is to automatically classify road images into two classes:

- Normal Road
- Pothole

## Dataset

A publicly available Pothole and Normal Road dataset was used.

Dataset Source:
https://zenodo.org/records/13334878

The dataset contains:

- 2500 Normal Road images
- 2500 Pothole images

A balanced dataset was prepared for training, validation, and testing.

## Dataset Split

The dataset was divided into:

- Training: 3500 images
- Validation: 750 images
- Testing: 750 images

## Preprocessing and Augmentation

The following preprocessing and augmentation techniques were used:

- Image resizing to 224 × 224 pixels
- Pixel value rescaling
- Rotation
- Width and height shifting
- Zooming
- Horizontal flipping

These techniques help improve model generalization.

## Model

A CNN model was developed for binary classification.

The model contains:

- Convolutional layers
- Max Pooling layers
- Flatten layer
- Dense layer
- Dropout layer
- Sigmoid output layer

The final output classifies an image as either Normal Road or Pothole.

## Training

The model was trained using:

- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Batch Size: 32
- Epochs: 5

Early stopping and learning-rate reduction techniques were also used.

## Results

The final model achieved:

**Test Accuracy: 92.4%**

The classification report showed approximately:

- Normal Road F1-score: 0.92
- Pothole F1-score: 0.92

## Evaluation

The project includes:

- Training and validation accuracy graph
- Training and validation loss graph
- Confusion matrix
- Classification report
- Sample predictions

These evaluation methods help measure the performance of the trained model.

## Technologies Used

- Python
- Google Colab
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## How to Run

1. Open the provided Google Colab notebook.
2. Run the cells in order.
3. The dataset will be downloaded automatically.
4. The images will be preprocessed and divided into training, validation, and testing sets.
5. The CNN model will be trained.
6. The final accuracy, graphs, confusion matrix, and sample predictions will be generated.

## Project Files

- `pothole_vs_normal_road_classification.ipynb` - Complete project notebook
- `README.md` - Project documentation

## Conclusion

This project demonstrates how deep learning and CNN-based image classification can be used to detect potholes in road images. The achieved test accuracy of 92.4% shows that the model can effectively distinguish between pothole and normal road images.
