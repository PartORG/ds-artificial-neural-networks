# PartORG/ds-artificial-neural-networks

[![Python](https://img.shields.io/badge/python-3.11-blue.svg)] [![License](https://img.shields.io/github/license/PartORG/ds-artificial-neural-networks)] [![GitHub issues](https://img.shields.io/github/issues/PartORG/ds-artificial-neural-networks)] [![GitHub forks](https://img.shields.io/github/forks/PartORG/ds-artificial-neural-networks)] [![GitHub stars](https://img.shields.io/github/stars/PartORG/ds-artificial-neural-networks)]

# Artificial Neural Networks

Welcome to the **ds-artificial-neural-networks** repository! This project is designed to help you understand and practice artificial neural networks using TensorFlow, Keras, and other essential libraries. Whether you're a beginner or looking to deepen your understanding, this repository provides a structured learning path.

## Table of Contents
- [Features](#features)
- [How It Works](#how-it-works)
- [Technology Stack](#technology-stack)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Quick Start](#quick-start)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Development](#development)
- [Testing](#testing)
- [Limitations](#limitations)
- [License](#license)

## Features

### Artificial Neural Networks
This project covers the basics of artificial neural networks, including dense neural networks (DNN), regularization, model persistence, and convolutional neural networks (CNNs).

### Dense Neural Networks (DNN)
Learn how to implement DNN for regression and classification problems using TensorFlow & Keras.

### Regularisation & Model Persistence
Explore techniques to prevent overfitting and underfitting, as well as methods to save and load models.

### Convolutions & Transfer Learning
Dive into convolutional neural networks (CNNs) and learn about transfer learning with pre-trained models.

### Bonus: DNN from Scratch
A bonus section for those interested in building a deep neural network from scratch. This exercise helps you understand the underlying mechanics of training a neural network.

## How It Works

The repository is structured around a series of Jupyter Notebooks, each building upon the previous one. Each day's content covers specific topics and provides practical examples to help you understand and apply artificial neural networks.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| TensorFlow | A powerful library for machine learning and deep learning. |
| Keras | A high-level neural networks API, written in Python and capable of running on top of TensorFlow. |
| Jupyter Notebook | An open-source web application that allows you to create and share documents that contain live code, equations, visualizations, and narrative text. |
| Matplotlib | A plotting library for creating static, interactive, and animated visualizations in Python. |
| Pandas | A data manipulation and analysis library in Python. |
| NumPy | A library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays. |
| Seaborn | A Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive statistical graphics. |
| Statsmodels | A Python module that allows users to explore data, estimate statistical models, and perform statistical tests. |
| Scikit-learn | A simple and efficient tool for predictive data analysis built on NumPy, SciPy, and matplotlib. |
| Pydot | A Python interface to Graphviz's Dot language. |
| Protobuf | Google's protocol buffer library. |
| TensorFlow-Hub | An open platform for sharing machine learning modules. |
| TensorFlow-Docs | Documentation tools for TensorFlow.

## Requirements

To run this project, you need the following:

- Python 3.11
- Jupyter Notebook
- Matplotlib
- Pandas
- NumPy
- Seaborn
- Statsmodels
- Scikit-learn
- Pydot
- Protobuf
- TensorFlow 2.15
- TensorFlow-Hub
- TensorFlow-Docs

## Installation

To set up your environment, follow these steps:

### macOS or Linux

```bash
brew update
brew install graphviz
brew install hdf5
```

Check the Graphviz version:

```sh
dot -V
```

Install the virtual environment and required packages:

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

### WindowsOS

Update Chocolatey and install Graphviz and HDF5:

```bash
choco upgrade chocolatey
choco install graphviz
```

Check the Graphviz version:

```sh
dot -V
```

Install the virtual environment and required packages:

```bash
pyenv local 3.11.3
python -m venv .venv
.\venv\Scripts\activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Configuration

No specific configuration is required for this project.

## Quick Start

To get started, open the Jupyter Notebooks in the `day_1`, `day_2`, and `day_3` directories. Each notebook provides a step-by-step guide to learning and practicing artificial neural networks.

## Usage

Run the Jupyter Notebooks to explore and experiment with different aspects of artificial neural networks. You can also modify the notebooks to suit your needs or extend them with additional functionality.

## Project Structure

```
ds-artificial-neural-networks/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   ├── feature_request.md
│   │   └── feedback.md
│   └── workflows/
│       ├── REGX_test_import_libraries.sh
│       ├── add_issue_to_done.yml
│       ├── add_issue_todo.yml
│       ├── add_pr_in_progress.yml
│       ├── add_pr_to_done.yml
│       ├── discord-webhook-notify.yml
│       ├── replacement.yml
│       └── testing/
│           └── dnn_utils.py
├── .gitignore
├── README.md
├── bonus/
│   ├── 00_DNN_from_scratch.ipynb
│   └── dnn_utils.py
├── data.zip
├── day_1/
│   ├── 01_Regression_TensorFlow_Keras.ipynb
│   ├── 02_Classification_TensorFlow_Keras.ipynb
│   ├── 02_Classification_TensorFlow_Keras_2.ipynb
│   ├── 02_Classification_TensorFlow_Keras_3.ipynb
│   └── dnn_model/
│       ├── fingerprint.pb
│       ├── keras_metadata.pb
│       ├── saved_model.pb
│       └── variables/
│           ├── variables.data-00000-of-00001
│           └── variables.index
├── day_2/
│   ├── 03_Overfit_Underfit.ipynb
│   ├── 03_Overfit_Underfit_second_run.ipynb
│   ├── 04_Load_saved_Models.ipynb
│   └── saved_model/
│       ├── my_large_model/
│       │   ├── fingerprint.pb
│       │   ├── keras_metadata.pb
│       │   ├── saved_model.pb
│       │   └── variables/
│       │       ├── variables.data-00000-of-00001
│       │       └── variables.index
│       └── my_large_model_2/
│           ├── fingerprint.pb
│           ├── keras_metadata.pb
│           ├── saved_model.pb
│           └── variables/
│               ├── variables.data-00000-of-00001
│               └── variables.index
├── day_3/
│   ├── cnn/
│   │   ├── cnn_keras.ipynb
│   │   └── images/
│   │       ├── Convolution.gif
│   │       ├── cnn_example.png
│   │       ├── cnn_with_pooling.png
│   │       ├── convolved.jpeg
│   │       ├── max_pooling.png
│   │       ├── one_layer.png
│   │       ├── rgb.png
│   │       └── rgb_2.png
│   └── pretrained_transfer_learning/
│       ├── Pretrained_networks+transfer_learning.ipynb
│       ├── data.zip
│       ├── images/
│       │   ├── download.jpeg
│       │   ├── obj.png
│       │   └── object.png
│       └── models/
│           └── wallet_phone.h5
├── images/
│   └── artificial_network_architecture_dnn.png
└── requirements.txt
```

## Development

This project is open-source and contributions are welcome. If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

## Testing

No tests exist for this project at the moment.

## Limitations

- This repository assumes basic knowledge of Python and machine learning concepts.
- The notebooks provide practical examples but may not cover all edge cases.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.