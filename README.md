# SequencePredictionModel
This repository contains a sequence prediction model built using PyTorch. The model predicts the next number in a sequence based on previous numbers using a simple feedforward neural network. It is trained using a custom dataset and aims to learn the temporal dependencies in the sequences.

This code features the use of Poetry, a dependency and virtual environment manager. If you don't have Poetry, please install it via the Python package manager pip. Then change directories to this code, and run poetry install --no-root, which will install all of the required dependencies for you. You then select the poetry virtual environment as your Python kernel in your IDE.

To train the model, run the `train.py` file. The output/loss values will print to the console.


# Setup Instructions for Model
# paste the following in your terminal seperately:

pip install poetry
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" 
brew install python@3.11    
brew link python@3.11
poetry env use python3.11
poetry install --no-root
poetry run pip install torch==2.1.2 -f https://download.pytorch.org/whl/cpu.html
poetry lock
poetry install --no-root
poetry shell
poetry show
python train.py



### Explanation of the Steps:
1. **Install Poetry**: Poetry is the primary tool for managing dependencies and virtual environments in Python.
2. **Install Homebrew**: Homebrew is required to install Python and other dependencies that are not Python-based.
3. **Install Python 3.11 via Homebrew**: Homebrew is used to install Python 3.11, which is required for compatibility with the project.
4. **Poetry Configuration**: Ensures Poetry uses the correct Python version for the project.
5. **Install Dependencies**: Using Poetry, we install the project dependencies.
6. **Install PyTorch**: PyTorch is installed manually using `poetry run pip` as it might not be included directly in the `pyproject.toml` file.
7. **Lock Dependencies**: Locking dependencies ensures reproducibility across different systems.
8. **Activate Poetry Shell**: This creates an isolated environment where you can work on your project without interfering with other projects or system Python packages.
9. **Train the Model**: The final step is running the training script once everything is set up.
