# grape_disease
Classify different types of grape diseases using a dataset of grape images.

# TensorFlow Image Classification

This notebook demonstrates how to build an image classification model using TensorFlow. The model is trained to classify different types of grape diseases using a dataset of grape images.

## Prerequisites
- TensorFlow
- matplotlib

## Dataset
The dataset used in this notebook contains images of grape leaves affected by various diseases, as well as healthy grape leaves. The dataset is organized into separate folders for each class:
- Grape___Black_rot
- Grape___Esca_(Black_Measles)
- Grape___healthy
- Grape___Leaf_blight_(Isariopsis_Leaf_Spot)

## Preprocessing
The notebook starts by removing any corrupted images from the dataset. It then prepares the dataset for training and validation by splitting it into training and validation sets. The images are resized to a uniform size of 180x180 pixels and are batched for efficient processing.

## Data Augmentation
Data augmentation is applied to the training dataset to improve model generalization and prevent overfitting. The augmentation includes random horizontal flipping and random rotation of the images.

## Model Training
A convolutional neural network (CNN) model is used for image classification. The model is trained using the augmented training dataset. The training is performed using mini-batches, with the model weights updated based on the gradients computed during each batch. The validation dataset is used to monitor the model's performance during training and prevent overfitting.

## Results
After training, the notebook displays a grid of sample images from the training dataset, along with their corresponding labels. The grid provides a visual check to verify that the dataset and data augmentation are correctly applied.

## Next Steps
You can further improve the model's performance by adjusting hyperparameters, exploring different CNN architectures, or applying additional preprocessing techniques. Additionally, you can evaluate the model's performance on a separate test dataset to assess its generalization ability.
