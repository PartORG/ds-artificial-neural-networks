# Artificial Neural Networks

In this repo, we will explore artificial neural networks through a series of Jupyter notebooks designed to cover regression, classification, regularization, model persistence, convolutional neural networks (CNN), and transfer learning.

## Requirements

To run this project, you need the following dependencies with their specified versions:

- jupyterlab==4.2.5
- matplotlib==3.7.1
- pandas==2.0.1
- numpy==1.23.5
- seaborn==0.12.2
- statsmodels==0.13.5
- scikit-learn==1.2.2
- pydot
- protobuf
- tensorflow==2.15
- tensorflow-hub
- tensorflow-docs

## Installation

### macOS or Linux

1. Update Homebrew and install **hdf5** and **graphviz**:

    ```bash
    brew update
    brew install graphviz
    ```

2. Install the virtual environment and required packages:

    - For macOS with **silicon** chips (other than intel):

        ```bash
        pyenv local 3.11.3
        python -m venv .venv
        source .venv/bin/activate
        pip install --upgrade pip
        pip install -r requirements_silicon.txt
        ```

    - For macOS with **intel** chips:

        ```bash
        pyenv local 3.11.3
        python -m venv .venv
        source .venv/bin/activate
        pip install --upgrade pip
        pip install -r requirements.txt
        ```

### WindowsOS

1. Update chocolatey and install **hdf5** and **graphviz**:

    ```bash
    choco upgrade chocolatey
    choco install graphviz
    ```

2. Install the virtual environment and required packages:

    ```bash
    pyenv local 3.11.3
    python -m venv .venv
    .\.venv\Scripts\activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```

## Usage

To run the project, follow these steps:

1. Fork this repository and clone it to your local machine.
2. Set up a virtual environment as described in the Installation section.
3. Activate the virtual environment.
4. Install the required packages using `pip install -r requirements.txt` (or `requirements_silicon.txt` for macOS with silicon chips).
5. Open JupyterLab by running `jupyter lab`.
6. Navigate to the notebooks in the respective directories (`day_1`, `day_2`, `day_3`, etc.) and execute them.

Each notebook provides a detailed guide on specific topics related to artificial neural networks, from basic concepts to advanced techniques like transfer learning.