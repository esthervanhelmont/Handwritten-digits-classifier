# Handwritten-digits-classifier
## Handwritten Digits Classifier using a Neural Network

This project trains a neural network to recognize handwritten digits (0–9).  
Using a dataset of small grayscale images, the model learns to identify patterns such as curves, edges, and shapes that characterize each digit.

This type of system is commonly used in document processing, postal mail automation, and educational machine learning examples.

---

## Summary

The goal of this project is to build, train and evaluate a handwritten digit classifier using PyTorch.  
The notebook includes:

- Loading and preparing the digit dataset  
- Normalizing and batching the data  
- Building a neural network model  
- Training the model over several epochs  
- Evaluating accuracy on unseen test data  
- Making predictions on new digit samples  

---

## Problem Statement

We want to classify small 28×28 pixel images of handwritten digits into one of 10 classes (0–9).  
A neural network can learn these visual patterns through supervised learning.

---

## Model Overview

The model is implemented using PyTorch and follows a simple feed-forward architecture:

- Flatten input layer (28×28 → 784 features)  
- Fully connected (Linear) layers  
- ReLU activation functions  
- Output layer with 10 units (for digits 0–9)  
- LogSoftmax activation for classification  

Loss function: **Negative Log Likelihood Loss (NLLLoss)**  
Optimizer: **Stochastic Gradient Descent (SGD)** or **Adam** depending on your configuration.

---

## Notebook Workflow

### **1. Import Libraries**
- `torch`, `torchvision`, `torch.nn`, `torch.utils.data`
- Helper functions for transforms and visualization  

---

### **2. Load Dataset**
- Load training and test datasets  
- Apply normalization  
- Create DataLoaders for batching  
- Shuffle training data for better learning  

---

### **3. Build Neural Network**
Example structure:

