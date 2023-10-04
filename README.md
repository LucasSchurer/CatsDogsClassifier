# Cats and Dogs Classifier

A project for classifying images of cats and dogs using Machine Learning.

## Project Structure

The project is organized as follows:

- **model.ipynb**: This notebook is responsible for creating, training, and saving the convolutional neural network (CNN) model used for classifying images of cats and dogs. The dataset used for training was the [Dog vs Cats](https://www.kaggle.com/c/dogs-vs-cats) dataset provided by Kaggle.

- **app.ipynb**: This notebook contains the code for creating a simple web interface using Flask and ngrok. The interface allows users to upload images from their device or provide URLs and use the trained model to classify them as cats or dogs.

## Model

The architecture of the model used is as follows:

- Layers for data augmentation for image preprocessing.
- Three Conv2D layers with 64, 128, and 256 filters, respectively. After each Conv2D layer, a MaxPool2D layer, BatchNormalization, and Dropout with a rate of 0.3 were added.
- A fully connected layer with 128 units, followed by another Dropout layer with a rate of 0.5.

Hyperparameters were adjusted after several training iterations to optimize the model's performance.