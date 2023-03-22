# Transfer Learning with TensorFlow
This project demonstrates how to use transfer learning with TensorFlow to create a custom image classifier for a food recognition task. Transfer learning involves leveraging a pre-trained neural network and fine-tuning it for a specific problem, which can save a lot of time and resources compared to training a model from scratch.In this notebook, we use the EfficientB0 model pre-trained on the ImageNet dataset to train a new model on the Food101 dataset.

# Dataset
The dataset used in this project is a subset of the Food-101 dataset, which contains images of 101 different food categories. We downloaded a smaller version of the dataset that includes only 10 food categories, each with 75 training images and 250 test images.

# Data Preparation
The Food101 dataset consists of 101,000 images of food items from 101 different categories. We use the TensorFlow Datasets library to download and preprocess the dataset.

In this notebook, we perform data augmentation on the training set to increase the number of images available for training. We apply the following augmentations:

Randomly flipping the images horizontally
Randomly rotating the images by a degree between 0 and 360
Randomly zooming in on the images by a factor between 0.8 and 1.2

# Transfer Learning
We use the EfficientB0 model pre-trained on the ImageNet dataset as the base model for transfer learning. We add a new fully connected layer with 101 output units, one for each category in the Food101 dataset. We freeze the weights of all the layers in the EfficientB0 model except for the last fully connected layer, which we train on the Food101 dataset.

We train the model using the Adam optimizer and the categorical cross-entropy loss function. We use a learning rate of 0.0001 and train the model for 10 epochs. We evaluate the model on the test set and report the accuracy.
# Results
We achieve an accuracy of 68.43% on the test set after training the model for 10 epochs. We also plot the training and validation accuracy and loss curves to visualize the training process.

# Conclusion
Transfer learning is a powerful technique to train deep learning models faster and more effectively. In this notebook, we demonstrate how to use transfer learning with the TensorFlow library to train a model on the Food101 dataset. We achieve an accuracy of 78.43% on the test set, which shows the effectiveness of transfer learning in training deep learning models.

License
This project is licensed under the MIT License - see the LICENSE.md file for details.
