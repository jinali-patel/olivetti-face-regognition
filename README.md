# Face Recognition Using LDA, SVM, and CNN

Introduction to Artificial Intelligence — Academic Project  
Author: Jinali Patel

## Overview
Comparison of Linear Discriminant Analysis (LDA), a Support Vector
Machine (SVM), and a LeNet-style Convolutional Neural Network (CNN)
on the Olivetti faces dataset.

## Technologies
Python, NumPy, pandas, Matplotlib, scikit-learn, and PyTorch.

## Dataset
400 grayscale images of 40 individuals, each measuring 64 × 64 pixels.
The notebook downloads the dataset through scikit-learn.

## Experimental Setup

| Model | Training Images | Validation Images | Test Images |
|-------|----------------:|------------------:|------------:|
| LDA | 320 | 0 | 80 |
| SVM | 320 | 0 | 80 |
| CNN | 240 | 80 | 80 |

All models use the same test images. The CNN trains for 30 epochs
and preserves the weights with the highest validation accuracy.

## Evaluation
- Test accuracy and macro F1-score.
- Confusion matrices for each model.
- CNN training loss and training/validation accuracy curves.

## Run the Project
1. Open `intro_to_ai_face_recognition.ipynb` in Google Colab.
2. Select Runtime → Run all.
3. Review the evaluation outputs and plots.

An internet connection is required to download the dataset.

## Results

| Model | Test Accuracy | Macro F1-score |
|-------|--------------:|---------------:|
| LDA | 97.50% | 0.9742 |
| SVM | 92.50% | 0.9075 |
| CNN | 80.00% | 0.7893 |

Results use the same 80 test images. LDA and SVM use 320
training images; the CNN uses 240 training images and
80 validation images.

## Limitations
This comparison uses a small, controlled dataset and different
training-set sizes across models. Results do not establish
real-world face recognition performance.
