# PartORG/ds-artificial-neural-networks

[![Python](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/github/license/neuefische/ds-artificial-neural-networks)](LICENSE)
[![GitHub issues](https://img.shields.io/github/issues/neuefische/ds-artificial-neural-networks)](https://github.com/neuefische/ds-artificial-neural-networks/issues)
[![GitHub forks](https://img.shields.io/github/forks/neuefische/ds-artificial-neural-networks)](https://github.com/neuefische/ds-artificial-neural-networks/network/members)

# Artificial Neural Networks

Welcome to the `ds-artificial-neural-networks` repository! This project is designed to help you understand and implement artificial neural networks using TensorFlow, Keras, and other relevant libraries. Whether you're a beginner or an experienced practitioner, this guide will provide you with a comprehensive understanding of how to build, train, and deploy neural networks.

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

### Dense Neural Networks (DNN)

This section covers the basics of building and training dense neural networks using TensorFlow and Keras. You'll learn how to implement DNNs for both regression and classification problems.

### Regularisation & Model Persistence

Explore techniques to prevent overfitting and underfitting, as well as how to save and load trained models for future use.

### Convolutions & Transfer Learning

Dive into convolutional neural networks (CNNs) and learn about transfer learning using pre-trained models from TensorFlow Hub.

## How It Works

The project is structured around a series of Jupyter notebooks that guide you through the process of building, training, and deploying neural networks. Each notebook focuses on a specific aspect of neural network development.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| **TensorFlow** | A powerful library for machine learning and deep learning. |
| **Keras** | A high-level API built on top of TensorFlow, designed to make building and training models easier. |
| **Jupyter Notebook** | An interactive computing environment that allows you to create and share documents containing live code, equations, visualizations, and narrative text. |
| **Matplotlib** | A plotting library for creating static, animated, and interactive visualizations in Python. |
| **Pandas** | A data manipulation and analysis library that provides data structures and functions needed to manipulate structured data. |
| **NumPy** | A fundamental package for scientific computing with Python, providing support for large, multi-dimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays. |
| **Seaborn** | A statistical data visualization library based on Matplotlib that provides a high-level interface for drawing attractive and informative statistical graphics. |
| **Statsmodels** | A Python module that allows users to explore data, estimate statistical models, and perform statistical tests. |
| **Scikit-learn** | A simple and efficient tool for predictive data analysis built on NumPy, SciPy, and matplotlib. |
| **Pydot** | A Python interface to Graphviz's Dot language, which is used for drawing graphs visually. |
| **Protobuf** | Google's protocol buffer library, used for serializing structured data. |
| **TensorFlow-Hub** | A repository of reusable machine learning modules, including pre-trained models and components that can be easily integrated into your projects. |
| **TensorFlow-Docs** | A set of tools to help you document TensorFlow code.

## Requirements

To run this project, you will need the following:

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

To get started, simply open the Jupyter notebooks in the `day_1`, `day_2`, and `day_3` directories. Follow the instructions provided in each notebook to build and train your neural networks.

## Usage

You can run the Jupyter notebooks directly from your local environment or use a cloud-based Jupyter service like Google Colab.

### Example Commands

```bash
jupyter notebook day_1/01_Regression_TensorFlow_Keras.ipynb
```

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

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## Testing

This project does not include automated tests at this time. However, you can manually test the notebooks to ensure they work as expected.

## Limitations

- This project is designed for educational purposes and may not be suitable for production use.
- Some features may require additional setup or configuration depending on your environment.

## License

This project is licensed under the [MIT License](LICENSE).