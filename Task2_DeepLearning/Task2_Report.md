# Task 2 – Deep Learning Image Classification

## 1. Objective

To develop a deep learning model for image classification using the CIFAR-10 dataset and evaluate its performance using training and testing metrics.

## 2. Dataset

The CIFAR-10 dataset was used for this project.

- Training images: 50,000
- Testing images: 10,000
- Number of classes: 10
- Image size: 32 × 32 pixels
- Image channels: RGB

### Classes

1. Airplane
2. Automobile
3. Bird
4. Cat
5. Deer
6. Dog
7. Frog
8. Horse
9. Ship
10. Truck

## 3. Data Preprocessing and Augmentation

The training images were processed using:

- Random horizontal flipping
- Random rotation
- Conversion to tensors
- Normalization using CIFAR-10 mean and standard deviation

The test images were normalized without augmentation.

## 4. Model Architecture

A lightweight Convolutional Neural Network (CNN) was developed using PyTorch.

The model consists of:

- Convolutional Layer 1: 3 → 32 channels
- ReLU activation
- Max Pooling
- Convolutional Layer 2: 32 → 64 channels
- ReLU activation
- Max Pooling
- Convolutional Layer 3: 64 → 128 channels
- ReLU activation
- Max Pooling
- Fully Connected Layer: 128 × 4 × 4 → 256
- ReLU activation
- Output Layer: 256 → 10 classes

Total trainable parameters: 620,362

## 5. Training Configuration

The model was trained using:

- Loss function: Cross Entropy Loss
- Optimizer: Adam
- Learning rate: 0.001
- Batch size: 128
- Number of epochs: 3
- Device: CPU

## 6. Training Results

| Epoch | Training Loss | Training Accuracy |
|------:|--------------:|-------------------:|
| 1 | 1.4209 | 48.50% |
| 2 | 1.0344 | 63.45% |
| 3 | 0.8759 | 69.33% |

## 7. Model Evaluation

The trained model achieved:

**Test Accuracy: 71.03%**

The model was also evaluated using:

- Confusion Matrix
- Classification Report
- Sample Image Inference

## 8. Sample Inference

A sample image was passed through the trained model.

Example prediction:

- Predicted class: Truck
- Confidence: 74.48%

## 9. Output Files

The following files were generated:

- `cifar10_cnn_model.pth`
- `Task2_Training_Accuracy.png`
- `Task2_Training_Loss.png`
- `Task2_Confusion_Matrix.png`
- `Task2_Classification_Report.txt`
- `Task2_Inference_Result.png`
- `Task2_Results.txt`

## 10. Conclusion

A CNN-based deep learning model was successfully developed for CIFAR-10 image classification using PyTorch. The model achieved 71.03% test accuracy after three training epochs. The project demonstrates the complete workflow of dataset preparation, augmentation, CNN model development, training, evaluation, and model saving.