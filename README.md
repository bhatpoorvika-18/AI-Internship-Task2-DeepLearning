# AI Internship - Task 2: Deep Learning

This project implements a deep learning image classification model using the CIFAR-10 dataset and PyTorch.

## Objective

To develop, train, evaluate, and save a CNN-based deep learning model for classifying CIFAR-10 images.

## Dataset

- Dataset: CIFAR-10
- Training Images: 50,000
- Testing Images: 10,000
- Number of Classes: 10
- Image Size: 32 × 32
- Classes: Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck

## Model

A Convolutional Neural Network (CNN) was developed using PyTorch.

The model contains:
- Convolutional layers
- ReLU activation
- Max pooling
- Fully connected layers
- Softmax-based prediction

## Data Augmentation

The training dataset uses:
- Random Horizontal Flip
- Random Rotation
- Normalization

## Training

The model was trained for 3 epochs using:
- Loss Function: Cross Entropy Loss
- Optimizer: Adam
- Learning Rate: 0.001
- Batch Size: 128

## Results

| Epoch | Training Accuracy |
|------:|------------------:|
| 1 | 48.50% |
| 2 | 63.45% |
| 3 | 69.33% |

**Test Accuracy: 71.03%**

## Model Evaluation

The project includes:
- Training accuracy graph
- Training loss graph
- Confusion matrix
- Classification report
- Sample inference result

## Files

- `Task2_DeepLearning.ipynb` – Complete implementation
- `cifar10_cnn_model.pth` – Trained CNN model
- `Task2_Training_Accuracy.png` – Training accuracy graph
- `Task2_Training_Loss.png` – Training loss graph
- `Task2_Confusion_Matrix.png` – Confusion matrix
- `Task2_Classification_Report.txt` – Classification report
- `Task2_Inference_Result.png` – Sample prediction
- `Task2_Results.txt` – Results summary
- `Task2_Report.md` – Detailed project report

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Conclusion

A CNN-based deep learning model was successfully developed for CIFAR-10 image classification. The model achieved **71.03% test accuracy** after three training epochs and demonstrates the complete workflow from data preparation to model evaluation and saving.
