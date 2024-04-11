# House Prices Prediction

This repository contains code for predicting house prices using machine learning techniques. It includes data preprocessing, model training, evaluation, and making predictions on new data.

## Introduction

In this project, we aim to predict house prices based on various features such as the size of the house, the number of bedrooms and bathrooms, location, etc. We use a dataset containing historical data on house prices, including information on the features mentioned above.

## Data Preprocessing

We start by reading the train and test datasets using Pandas. We then perform data preprocessing steps, including:

- Handling missing values: We impute missing values for numeric features with the mean and for categorical features with the most frequent value.
- Encoding categorical features: We use OneHotEncoder to encode categorical features into numerical values.
- Standardizing numeric features: We standardize numeric features to ensure they have a mean of 0 and a standard deviation of 1.
- Dimensionality reduction: We reduce the dimensionality of the dataset using Principal Component Analysis (PCA) to improve computational efficiency while preserving most of the variance in the data.

## Model Training

We train a neural network model using TensorFlow/Keras to predict house prices. The model architecture consists of multiple dense layers with ReLU activation functions. We compile the model using the Adam optimizer and mean squared error loss function.

## Model Evaluation

We evaluate the trained model on a validation set by making predictions and calculating the root mean squared error (RMSE) between the predicted and actual house prices.

## Making Predictions

We use the trained model to make predictions on the test dataset. We then convert the predictions back to the original scale and create a submission file containing the predicted house prices.

## File Organization

- `train.csv`: Train dataset containing historical data on house prices and features.
- `test.csv`: Test dataset containing features for which we need to predict house prices.
- `submission.csv`: Submission file containing predicted house prices for the test dataset.
- `README.md`: Markdown file containing information about the project.

## Usage

To run the code and reproduce the results:

1. Clone this repository to your local machine.
3. Run the Jupyter Notebook or Python script containing the code.

## Contributing

Contributions to this project are welcome! If you have any suggestions, improvements, or bug fixes, feel free to open an issue or submit a pull request.

