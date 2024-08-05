# Dense Layer Classification using Olivetti Faces Dataset - CAP 6619

## Author: Amparo Godoy Pastore
## Date: June 2nd, 2024
## Course: CAP 6619 - Deep Learning - Florida Atlantic University

## Overview
This repository contains the code and data for Homework 2, Question 6 of the CAP 6619 - Deep Learning course at Florida Atlantic University. The task involves building and evaluating dense layer neural networks to classify images from the Olivetti Faces Dataset.

## Dataset
The Olivetti Faces Dataset consists of 400 grayscale images of faces. Each image is 64x64 pixels and there are 40 distinct individuals with 10 images per individual.

## Repository Contents
- `olivetti_faces.npy`: Numpy array containing the images.
- `olivetti_faces_target.npy`: Numpy array containing the target labels.
- `Dense Layer Classification Notebook.ipynb`: Jupyter Notebook containing the code for loading data, visualizing it, training, and evaluating different neural network architectures.

## Notable Functions
- `show_a_random_face_per_class(images, unique_ids)`: Displays one random face for each of the 40 classes in the dataset.
- `create_model(layers)`: Creates a neural network model with the specified number of layers.
- `evaluate_model(layers, data, target, kf)`: Evaluates a model using k-fold cross-validation.

## Results
The notebook compares the performance of four different neural network architectures:
1. Model 1: One hidden layer with 10 nodes.
2. Model 2: One hidden layer with 50 nodes.
3. Model 3: One hidden layer with 500 nodes.
4. Model 4: Two hidden layers with 50 nodes in the first layer and 10 nodes in the second layer.

### Accuracy Results
- **Model 1:** Mean Accuracy: 0.0150, Std Dev: 0.0122
- **Model 2:** Mean Accuracy: 0.0450, Std Dev: 0.0150
- **Model 3:** Mean Accuracy: 0.2725, Std Dev: 0.0647
- **Model 4:** Mean Accuracy: 0.0225, Std Dev: 0.0208

### Conclusion
Model 3, with one hidden layer and 500 hidden nodes, exhibits the best performance in terms of mean accuracy. Therefore, Model 3 is the preferred choice among these neural network architectures for the given task.
