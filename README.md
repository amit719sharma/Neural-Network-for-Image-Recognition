# neural-network-classifier

Neural Network for Image Recognition of Letters A, B, and C

## Overview
A minimal-from-scratch implementation of a feedforward neural network (one hidden layer) using NumPy to classify binary 5x6 pixel images of letters **A**, **B**, and **C**.

## Files
- `neural_network_classifier.ipynb` — Ready-to-run Jupyter Notebook with code, visualizations and model saving.
- `nn_weights.npz` — (generated after running the notebook) saved weights file.
- `README.md` — this file.

## Approach & Methodology
- **Data**: Manually defined 5×6 binary patterns for A, B, and C, flattened to 30-element vectors.
- **Model**: Feedforward neural network:
  - Input layer: 30 neurons
  - Hidden layer: 8 neurons (sigmoid activation)
  - Output layer: 3 neurons (sigmoid activation)
- **Training**: Batch gradient descent implemented with manual backpropagation using NumPy. Loss used: Mean Squared Error (MSE).
- **Evaluation**: Uses argmax on output neurons to predict class and plots training loss and accuracy.

## Analysis & Notes
- This educational implementation favors clarity over performance. For production models use libraries like PyTorch or TensorFlow.
- Using cross-entropy with softmax is generally better for classification than MSE + sigmoid on outputs; kept MSE+sigmoid here because the assignment specifically emphasized sigmoid and manual backprop demonstration.
