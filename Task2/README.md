# MNIST Classification Project

## Project Description

This project implements image classification for the MNIST dataset using three different algorithms:

- **Random Forest**
- **Feed-Forward Neural Network** (FFNN)
- **Convolutional Neural Network** (CNN)

Each classifier is implemented as a separate class following the `MnistClassifierInterface` interface.

## File Structure

- `Task1.ipynb` – Main project file containing code for data loading, preprocessing, model training, and evaluation.
- `RandomForest.ipynb` – File containing the implementation of the Random Forest model with hyperparameter tuning.
- `Feed-Forward.ipynb` – File with the implementation of a fully connected neural network (FFNN) using Keras.
- `cnn.ipynb` – File with the implementation of a Convolutional Neural Network (CNN) for MNIST classification.

## Installation and Execution

### Required Libraries

Before running the project, make sure you have all the necessary libraries installed. You can install them using:

```bash
pip install numpy pandas scikit-learn tensorflow keras matplotlib
```

### Running the Project

1. Open `Task1.ipynb` in Jupyter Notebook.
2. Run all cells to load the dataset, train the models, and evaluate their performance.
3. Classification results will be displayed as accuracy and loss values.

## Methods Used

### 1. Random Forest

- Uses the Random Forest algorithm from `sklearn.ensemble.RandomForestClassifier`.
- Hyperparameters are tuned using `RandomizedSearchCV` or `GridSearchCV`.

### 2. Feed-Forward Neural Network

- A neural network with 3 hidden layers: 300, 100, and 100 neurons.
- Uses ReLU activation and `categorical_crossentropy` as the loss function.
- Optimizers can be configured, with SGD used by default.

### 3. Convolutional Neural Network (CNN)

- Implements a CNN model using `tensorflow.keras`.
- Includes convolutional layers, max pooling, and fully connected layers.
- Uses softmax activation for multi-class classification.

## Model Evaluation

- **Accuracy** is used as the primary metric for model comparison.
- **Loss** (model error on test data) is also analyzed.


