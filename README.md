# Week 1 Assignment: Numerical Data Prediction

## Overview

This assignment demonstrates how to generate numerical data, train a
neural network to learn the relationship between inputs and outputs, and
evaluate predictions on unseen test data.

## Objective

-   Generate numerical data using a known mathematical relationship.
-   Train a neural network to learn the relationship.
-   Predict outputs for unseen inputs.
-   Visualize training/validation loss and compare actual versus
    predicted values.

## Dataset

The data is generated in Python using NumPy and the equation:

**y = 3x + 2**

Random noise is not added.

-   Total samples: 200
-   Training samples: 160 (80%)
-   Testing samples: 40 (20%)
-   Input range: 0 to 10

## Technologies Used

-   Python
-   NumPy
-   Matplotlib
-   TensorFlow / Keras
-   Scikit-learn
-   Jupyter Notebook

## Model Architecture

The notebook uses a feedforward neural network with: - Input: one
numerical feature - Hidden layer 1: 16 neurons with ReLU activation -
Hidden layer 2: 16 neurons with ReLU activation - Output layer: 1 neuron
for numerical prediction

The model is compiled with the Adam optimizer, Mean Squared Error (MSE)
loss, and Mean Absolute Error (MAE) as a metric. It is trained for 100
epochs with a batch size of 16 and uses 20% of the training split for
validation.

## Evaluation Results

The notebook reports these results on the test dataset:

  Metric               Result
  ----------------- ---------
  Test Loss (MSE)     0.01176
  Test MAE            0.09197
  R² Score            0.99985

The high R² score and low test errors indicate that the model's
predictions are very close to the actual values for this generated
dataset.

## Visualizations

1.  **Generated Numerical Data:** Shows the relationship between input
    values and output values.
2.  **Training and Validation Loss Curve:** Shows how loss changes over
    the training epochs.
3.  **Actual vs Predicted Graph:** Compares the actual test outputs with
    the model's predictions. Points close to the diagonal reference line
    indicate accurate predictions.

## Conclusion

The neural network learned the linear relationship in the generated data
and predicted unseen test outputs with high accuracy. This assignment
demonstrates the basic workflow of data generation, train-test
splitting, neural network training, prediction, evaluation, and
visualization.

## How to Run

1.  Open `num.ipynb` in Jupyter Notebook or Google Colab.
2.  Ensure the required libraries are installed.
3.  Run the notebook cells in order.
4.  Review the graphs, printed predictions, and evaluation metrics.
