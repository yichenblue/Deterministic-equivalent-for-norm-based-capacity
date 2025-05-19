# Random Feature Ridge Regression (RFRR) Project

This project implements and analyzes Random Feature Ridge Regression (RFRR) for real-world datasets and Gaussian design scenarios. The project includes implementations for both theoretical analysis and practical applications.



## Project Structure

```
.
├── src/
│   ├── RFRR_real_world/        # Real-world dataset implementations
│   │   ├── RFRR.py             # Main 
│   │   ├── utils.py            # Utility functions
│   │   ├── models.py           # Model definitions
│   │   ├── DE_utils.py         # Deterministic equivalent utilities
│   │   └── visualize_intro_figure.py  # Visualization tools
│   │
│   └── gaussian_design/        # Gaussian design implementations
│       ├── ridge_regression/   # linear ridge regression
│       └── random_feature_ridge_regression/  # Random feature ridge regression with gaussian design
│
├── requirements.txt            # Project dependencies
└── README.md                   # This file
```

## Introduction

![Introduction Figure](intro_figure.png?raw=true)

## Features

- Implementation of Random Feature Ridge Regression (RFRR)
- Support for real-world datasets (MNIST, FashionMNIST, CIFAR-10, SVHN)

## Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd [repository-name]
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### Real-world Dataset Analysis

To run the RFRR analysis on MNIST dataset:

```bash
python src/RFRR_real_world/RFRR_MNIST.py --dataset MNIST --device cpu
```

### Gaussian Design Analysis

To run the Gaussian design analysis:

```bash
python src/gaussian_design/random_feature_ridge_regression/random_feature_ridge_regression.py
```

## Dependencies

The project requires the following main dependencies:
- PyTorch (>= 2.1.1)
- NumPy (>= 1.26.0)
- SciPy
- Matplotlib
- torchvision
- einops
- vit-pytorch

For a complete list of dependencies, see `requirements.txt`.

## Configuration

The project uses a `config.json` file to specify data and results directories. Make sure to create the necessary directories as specified in the configuration file.

## Results

The results of the experiments are saved in the `results/` directory, including:
- Test error vs features plots
- Norm vs features plots
- Test error vs Norm plots

## Contributing

Feel free to submit issues and enhancement requests.

