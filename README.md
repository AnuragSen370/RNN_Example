# RNN_Example
# Program Description:
This program builds a simple Recurrent Neural Network (RNN) model to learn a numeric sequence pattern and predict the next number in the sequence.

First, it creates a dataset where:

Each input (x) is a sequence of 3 consecutive numbers, e.g., [1, 2, 3], [2, 3, 4], etc.

Each output (y) is the next number in the sequence, e.g., 4, 5, etc.

The inputs are reshaped into a 3D array format (samples, time_steps, features) using NumPy, which is the required input shape for RNN models.

Then, a Sequential model is built with the following layers:

A SimpleRNN layer with 10 units and ReLU activation that learns from the sequential input.

A Dense layer with 1 unit to predict the next number in the sequence.

The model is compiled using the Adam optimizer and Mean Squared Error (MSE) as the loss function, and it's trained for 300 epochs on the created dataset.

Finally, the model is tested with a new input sequence [10, 11, 12], and it predicts the next number in the pattern. The result is printed after rounding it to 2 decimal places.

# ✅ Use Case:
This is a basic example of sequence prediction using RNN. It helps in understanding how RNNs work and can be expanded for real-world tasks like time series forecasting, stock prediction, or natural language processing.
