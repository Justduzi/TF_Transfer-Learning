# TF_Transfer-Learning
Tensorfflow transfer learning Feauture etraction
Transfer Learning with TensorFlow
This project demonstrates how to use transfer learning with TensorFlow to create a custom image classifier for a food recognition task. Transfer learning involves leveraging a pre-trained neural network and fine-tuning it for a specific problem, which can save a lot of time and resources compared to training a model from scratch.

Dataset
The dataset used in this project is a subset of the Food-101 dataset, which contains images of 101 different food categories. We downloaded a smaller version of the dataset that includes only 10 food categories, each with 75 training images and 250 test images.

Getting Started
To run this project, you'll need to have TensorFlow and the necessary dependencies installed. You can install them using pip:

Copy code
pip install tensorflow matplotlib
Next, download the dataset by running the following command:

python
Copy code
wget https://storage.googleapis.com/ztm_tf_course/food_vision/10_food_classes_10_percent.zip
Unzip the dataset:

python
Copy code
unzip 10_food_classes_10_percent.zip
Finally, run the transfer_learning.ipynb notebook to train and evaluate the model.

Results
Our transfer learning model achieved an accuracy of 78.8% on the test set, which is a good result considering that we only used a small subset of the original dataset.

License
This project is licensed under the MIT License - see the LICENSE.md file for details.
