# Image_satelite_classification_CNN

This project aims to classify satellite images using a convolutional neural network (CNN). Satellite images are multispectral data, with each pixel containing information from different spectral bands (red, green, blue, and infrared). The goal is to predict the category to which each image belongs, among four classes: Barren Land, Trees, Grassland, and Other. 

Project Steps: 

Data Preprocessing: Satellite images were preprocessed to prepare them for CNN training. This included loading the data from CSV files, resizing images to 28x28 pixels with 4 channels, and normalizing pixel values between 0 and 1. 

CNN Model Construction: A simple CNN model was built using TensorFlow. The model consists of multiple convolutional and pooling layers, followed by fully connected layers. ReLU activation function is used for hidden layers, while the output layer uses softmax activation for multi-class classification. 

Model Training: The CNN model was trained on a training dataset using stochastic gradient descent with categorical cross-entropy loss function. The Adam optimizer was used to minimize the loss. Model Evaluation: The trained model was evaluated on a test dataset to assess its performance. 

Evaluation metrics include accuracy and loss obtained on the test set.

Results:
After training the CNN model, the following performance was achieved on the test dataset:

Accuracy: 97%
Loss: 0.08
The model demonstrated high precision in satellite image classification, showcasing its effectiveness in this domain
