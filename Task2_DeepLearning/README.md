# Task 2: Deep Learning – CIFAR-10 Image Classification

## Objective
Build and evaluate a deep learning model for image classification using the CIFAR-10 dataset.

## Dataset
CIFAR-10 contains 60,000 RGB images of size 32×32 belonging to 10 classes:
airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck.

## Model
A lightweight Convolutional Neural Network (CNN) was implemented using PyTorch.

## Training
The model was trained for 3 epochs.

| Epoch | Training Accuracy |
|------|-------------------|
| 1 | 48.50% |
| 2 | 63.45% |
| 3 | 69.33% |

## Test Performance
Test Accuracy: 71.03%

## Data Augmentation
The training data uses image transformations and normalization to improve model generalization.

## Evaluation
The model was evaluated using:
- Test accuracy
- Confusion matrix
- Classification report
- Sample image predictions

## Generated Files
- cifar10_cnn_model.pth
- Task2_Training_Accuracy.png
- Task2_Confusion_Matrix.png
- Task2_Classification_Report.txt
- Task2_Inference_Result.png
- Task2_Results.txt
- Task2_DeepLearning.ipynb

## Environment
Python 3.12
PyTorch
Torchvision
NumPy
Matplotlib
Scikit-learn

## Conclusion
The trained CNN achieved a test accuracy of 71.03% on the CIFAR-10 test dataset.
