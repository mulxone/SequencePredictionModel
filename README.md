# SequencePredictionModel
This repository contains a sequence prediction model built using PyTorch. The model predicts the next number in a sequence based on previous numbers using a simple feedforward neural network. It is trained using a custom dataset and aims to learn the temporal dependencies in the sequences.

This code features the use of Poetry, a dependency and virtual environment manager. If you don't have Poetry, please install it via the Python package manager pip. Then change directories to this code, and run poetry install --no-root, which will install all of the required dependencies for you. You then select the poetry virtual environment as your Python kernel in your IDE.

To train the model, run the `train.py` file. The output/loss values will print to the console.
