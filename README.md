# Pytorch_Tree-Species-Mapping

This project implements deep learning models for tree species mapping using PyTorch. It enables the automatic classification of tree species and the generation of spatial distribution maps.

## Project Overview

The purpose of this project is to utilize deep learning models to classify tree species from sentinel-2 time series and create distribution maps. Core functionalities include:

- Preprocessing and loading tree species image datasets
- Training deep learning models using PyTorch
- Evaluating and validating the tree species classification model
- Generating large-scale tree species distribution maps

## Project Structure

```
├── .idea/                  # IDE configuration files
├── __pycache__/            # Python cache files
├── bases/                  # Core components
├── configs/                # Configuration files
├── models/                 # Model architectures
├── utils/                  # Utility functions
├── experiments/            # Experiment results
│   └── forestformer_0927/  # Example experiments
├── data_loader.py          # Data loading module
├── train.py                # Training script
├── evaluate.py             # Validation script
├── mapping.py              # Tree species mapping implementation
└── requirements.txt        # Environment dependencies
```

## Prerequisites

### Install Required Packages

Before running the code, make sure to install all necessary dependencies:

```bash
pip install -r requirements.txt
```

## Usage Guide

### Data Preparation

1. Prepare the training dataset, including tree species images and their respective labels.
2. Organize the dataset structure according to the requirements of the data loader.

### Model Training

To train the model, run the following command:

```bash
python train.py
```

### Model Validation

After training, evaluate the model's performance using:

```bash
python evaluate.py
```

### Tree Species Mapping

Use the trained model to generate large-scale tree species distribution maps:

```bash
python mapping.py
```

## Model Architecture

This project employs an optimized deep learning network ForestFormer tailored for tree species mapping tasks. The detailed architecture can be found in the `models/` directory.

## Experiment Results

Experiment results, including model weights, training logs, and evaluation metrics, are stored in the `experiments/` directory.

## License

This project is licensed under the MIT License.
