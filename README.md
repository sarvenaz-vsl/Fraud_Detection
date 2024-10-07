# Fraud Detection with Autoencoders

## Project Overview
This project applies an unsupervised learning approach using autoencoders to detect fraudulent transactions. By training on normal transaction data, the model learns to reconstruct the input. Transactions that the model struggles to reconstruct, indicated by a high reconstruction error, are flagged as potential fraud.

## Technologies Used
- **TensorFlow**: Utilized for building and training the neural network models.
- **Keras**: Used as the interface for TensorFlow to streamline model creation and training.
- **Python**: Programming language used for the entire project.

## Dataset
The dataset used in this project is sourced from the IEEE-CIS Fraud Detection competition on Kaggle. It comprises a wide range of features from transaction data that are essential for identifying fraudulent activity.

- **Dataset Link**: [IEEE-CIS Fraud Detection on Kaggle](https://www.kaggle.com/c/ieee-fraud-detection/data)

## Model Description
The autoencoder is a type of neural network used for anomaly detection in this project:
- **Training**: The autoencoder is trained solely on 'normal' transactions to learn the pattern of typical data.
- **Detection**: It predicts the output for new data, and if the reconstruction error surpasses a predetermined threshold, the transaction is considered fraudulent.
