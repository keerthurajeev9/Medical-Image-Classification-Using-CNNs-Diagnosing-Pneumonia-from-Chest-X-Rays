

# Medical Image Classification Using CNNs: Diagnosing Pneumonia from Chest X-Rays
## Description
This project focuses on classifying chest X-ray images into two categories: Normal and Pneumonia. Using deep learning and the Torch library in R, our goal is to automate pneumonia detection to assist healthcare professionals and enhance diagnostic accuracy and efficiency.

## Project Goals
Automate the detection of pneumonia from chest X-ray images.
Improve diagnostic speed and reduce human error.
Make diagnostic services more accessible in areas with limited healthcare resources.
Dataset
Source: Pediatric chest X-rays from Guangzhou Women and Children’s Medical Center.
Classes: Normal and Pneumonia (bacterial and viral).
Quality Assurance: Images were quality-checked and labeled by expert physicians.

## Installation
To set up the project environment, install R and the following packages:
install.packages(c("torch", "torchvision", "luz", "gridExtra", "jpeg", "imager", "magick", "dplyr", "EBImage"))

## For Bioconductor dependencies:
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install("EBImage")
## Project Setup
Clone the repository:
git clone <your-repo-link>
Navigate to the directory and set up your environment.
Install the dependencies as listed above.
## Usage
### Data Preprocessing
Normalizes pixel values and resizes images to a uniform size of 224x224.
### Data Augmentation
Applies transformations like random horizontal and vertical flips and color jittering to increase data diversity.
### Model Training
Uses a Convolutional Neural Network (CNN) implemented with Torch in R.
### Evaluation
Performance metrics include accuracy, loss plots, and additional classification metrics.
Model Architectures
Custom CNN: Features convolutional, pooling, and fully connected layers.
MobileNet: Lightweight, efficient architecture ideal for mobile applications.
ResNet: Deep residual network used for performance comparison.
### Results
Evaluation metrics and comparisons between different architectures.
Learning curves showcasing training and validation losses and accuracies.
## Challenges and Improvements
### Challenges
Handling class imbalance and optimizing model complexity.
Ensuring sufficient diversity in the training data.
### Future Improvements
Experimenting with additional architectures and transfer learning.
Implementing strategies to address class imbalance effectively.
Contribution
Contributions are welcome! If you'd like to improve this project, please fork the repository and submit a pull request.

## References
Image Preprocessing in R
Magick Package Documentation
