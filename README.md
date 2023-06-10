# Deep Learning-Based System for Alzheimer's Prediction

This project focuses on Alzheimer's prediction using a deep learning-based 
system after resolving the class imbalance in the Alzheimer dataset. The 
goal is to develop an accurate model that can effectively identify Alzheimer's 
cases.

## Dataset Balancing
The initial challenge in the project was the class imbalance in the Alzheimer
dataset. To address this issue, the dataset was balanced by employing suitable 
techniques such as oversampling, undersampling, or synthetic data generation. 
By achieving a balanced representation of positive and negative cases, the 
model's performance and reliability were enhanced.

## Deep Learning Autoencoder Model
An autoencoder-based deep learning model was used in this project.  The model 
was trained on the balanced dataset, allowing it to capture important features
related to Alzheimer's disease.

## Training Process
In addition to the general autoencoder model, a specialized autoencoder 
model was created specifically for positive labeled examples. This model
was trained exclusively on positive samples and then the trainable property
was turned off. By feeding negative examples to this frozen model, 
inferences were made based on the resulting loss values to determine 
whether the samples were positive or negative.

## Alzheimer's Prediction
The trained deep learning-based system, with its balanced dataset and autoencoder
models, can be utilized to predict Alzheimer's test cases. By analyzing 
the learned representations and leveraging the inferences from the specialized 
autoencoder, the model provides insights into whether an example belongs
to the positive or negative class, aiding in accurate Alzheimer's diagnosis.