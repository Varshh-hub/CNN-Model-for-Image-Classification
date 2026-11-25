# Flower Classification using CNN

## Project Overview

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify flower images into five categories: **Daisy, Dandelion, Roses, Sunflowers, and Tulips**.

The model is trained on the Flower Photos dataset to recognize visual patterns and features from images and predict the corresponding flower category. The project covers image preprocessing, dataset splitting, CNN model development, training, and performance evaluation.

## Dataset

The project uses the TensorFlow Flower Photos dataset containing **3,670 images** across five categories:

- Daisy
- Dandelion
- Roses
- Sunflowers
- Tulips

**Dataset Split:**
- Training: 2,936 images (80%)
- Validation: 734 images (20%)

Images are resized to **180 × 180 pixels** and normalized before being passed to the model.

## Model Architecture

A custom CNN was developed using TensorFlow and Keras with the following layers:

- Image normalization using Rescaling
- Three convolutional layers with ReLU activation
- Max Pooling layers for spatial feature extraction
- Flatten layer
- Dense layer with 128 neurons
- Dropout for regularization
- Softmax output layer for five-class classification

**Total Parameters:** 6,647,621

## Technologies Used

- Python
- TensorFlow and Keras
- NumPy
- Matplotlib
- Scikit-learn
- Convolutional Neural Networks (CNN)
- Deep Learning
- Image Classification

## Project Workflow

1. Download and load the flower image dataset.
2. Explore the dataset and identify flower categories.
3. Resize and normalize images.
4. Split the dataset into training and validation sets.
5. Build and compile the CNN architecture.
6. Train the model using the Adam optimizer.
7. Apply Early Stopping to monitor validation loss.
8. Evaluate model performance using classification metrics.
9. Visualize predictions, confusion matrix, accuracy, and loss curves.
10. Save the trained model in `.keras` format.

## Results and Evaluation

The model achieved the following validation performance:

| Metric | Result |
|---|---:|
| Validation Accuracy | 68.66% |
| Validation Loss | 0.8279 |
| Training Accuracy (Epoch 5) | 89.34% |

The model was evaluated using:

- Classification Report (Precision, Recall, F1-score)
- Confusion Matrix
- Training vs. Validation Accuracy
- Training vs. Validation Loss
- Actual vs. Predicted Image Comparisons

The results indicate that the model learned meaningful image features. However, the difference between training and validation accuracy suggests overfitting.

## Model Saving

The trained CNN model is saved in TensorFlow's Keras format:

`flower_classification_cnn.keras`

This model can be loaded later for flower image classification and prediction.

## Key Learnings

- Understanding CNN architecture and image classification.
- Working with image datasets using TensorFlow.
- Implementing image preprocessing and normalization.
- Training and evaluating deep learning models.
- Interpreting classification metrics and confusion matrices.
- Identifying overfitting through training and validation performance.
