Poisonous and Non-Poisonous Plant Classification:

This project focuses on classifying images of plants as either poisonous or non-poisonous using machine learning techniques. The goal is to develop an image classifier that can help identify potentially harmful plants based on visual characteristics.

DATASET: https://www.kaggle.com/datasets/nitron/poisonous-plants-images

Overview: 
The project utilizes the OpenCV library in Python to train a Support Vector Machine (SVM) model on a dataset of images representing poisonous and non-poisonous plants. The dataset is obtained from Kaggle and consists of labeled images of various plant species. The SVM model is trained to learn the distinguishing features between poisonous and non-poisonous plants.

Steps Involved:
Dataset Preparation: The dataset is organized into separate folders for training and testing. Each folder contains subfolders representing the classes (poisonous and non-poisonous), with image files inside them.

Image Preprocessing: The images are preprocessed to ensure consistency in size, format, and quality. Common preprocessing techniques such as resizing, normalization, and any necessary additional steps are applied.

Feature Extraction: The preprocessed images are flattened into feature vectors to create the training data. Each image is transformed into a 1D array representing its pixel values.

Training the SVM Model: The feature vectors and corresponding labels are used to train the SVM model. The model learns the patterns and characteristics that distinguish poisonous plants from non-poisonous ones.

Prediction: The trained model is used to predict the class labels (poisonous or non-poisonous) for new, unseen images. The images are preprocessed in the same manner as the training data, and their feature vectors are fed into the SVM model for prediction.

Confidence or Probability Scores: The decision values from the SVM model are converted into confidence or probability scores using the sigmoid function. These scores indicate the model's confidence in its predictions.

Usage
To use this project, follow these steps:

Prepare the dataset: Download the dataset from Kaggle or any other reliable source. Organize the images into separate folders for training and testing, with subfolders representing the classes.

Train the model: Run the training code provided in this repository, specifying the path to the training images folder. This will train the SVM model on the dataset.

Save the model: Save the trained SVM model to a file, which can be later loaded for predictions.

Test the model: Run the prediction code provided in this repository, specifying the path to the test images folder. The model will predict the class labels for the test images and print the results, including the confidence or probability scores.

Dependencies
Python
OpenCV
NumPy
