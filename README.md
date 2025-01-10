# Satellite Image Inpainting

This project aims to perform inpainting on satellite images using a convolutional neural network (CNN). The inpainting process involves filling in missing or corrupted parts of an image by utilizing the surrounding context.

## Overview

The notebook covers the following steps:

1. **Imports of Required Libraries**: Import necessary libraries such as NumPy, Matplotlib, OpenCV, TensorFlow, and TensorFlow Datasets.
2. **Dataset Preparation**: Load the EuroSAT dataset and split it into training, validation, and test sets. The dataset consists of RGB satellite images.
3. **Image Masking**: Implement a generator to create masks on the images for training, validation, and testing.
4. **Model Definition**: Define a CNN model with an encoder-decoder architecture for image inpainting. The model uses convolutional layers, batch normalization, and upsampling layers.
5. **Model Compilation**: Compile the model using the Adam optimizer and mean squared error (MSE) as the loss function.
6. **Model Training**: Train the model with the training data and use validation data to monitor performance. Implement callbacks for saving the best model and early stopping.
7. **Model Evaluation**: Evaluate the model on the test set by computing the MSE over multiple iterations to ensure robustness.
8. **Results Visualization**: Compare original, masked, and inpainted images to visualize the inpainting performance of the model.

## Results

The model's performance is evaluated by computing the mean and standard deviation of the MSE over multiple test iterations. The results show the effectiveness of the model in reconstructing the missing parts of the satellite images.

Feel free to explore the notebook for detailed code and visualizations.
