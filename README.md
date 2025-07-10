# claude_cplusplus_testB


# Minimal C++ Machine Learning Toolkit

Welcome to the Minimal C++ Machine Learning Toolkit — a lightweight, near dependency-free project offering basic tools for data processing, statistical analysis, and machine learning using modern C++ (C++17+) and only essential libraries like Eigen.

## Overview

The Minimal C++ Machine Learning Toolkit is designed to be simple, portable, and educational. It provides core tools for working with datasets, computing statistics, and training basic machine learning models in modern C++. It is well-suited for:

- **Educational use** — to help understand ML algorithms with transparent, low-level code  
- **Embedded or constrained systems** — where large ML libraries are not an option  
- **Prototyping** — using only STL and lightweight libraries  
- **Developers who value full control over memory, performance, and logic**

No TensorFlow. No PyTorch. No OpenCV. Just modern C++ and minimal dependencies.

## Features

### Data Handling

- Read and parse CSV files (header support, delimiter selection)
- Type inference (int, float, string) and simple missing value detection
- In-memory dataset representation using `std::vector<std::unordered_map<std::string, Value>>`

### Statistics & Preprocessing (with Eigen)

- Compute mean, variance, standard deviation, median
- Min-Max scaling and Z-score standardization
- Categorical encoding (label encoding)
- Missing value handling (drop or fill with mean/default)

### Basic Machine Learning

- **Linear Regression** (using Normal Equation or Gradient Descent)
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- Basic evaluation metrics: accuracy, precision, recall, MSE
- Manual train/test split

### Utilities

- Lightweight CSV and file I/O utilities
- Seeded random number generator for reproducibility
- Command-line driven examples

- Go to https://github.com/aeliamomo/claude_test_scpG and install the rest

## Why This Project?

This toolkit shows how far you can go with just:

- **Modern C++** (C++17+): no macros, clean type-safe code
- **Portability**: run on any system with a C++ compiler
- **Transparency**: fully readable logic with no magic
- **Safety**: no unsafe or overly complex dependencies

It’s an ideal resource for learning or for use in safe, auditable environments.

## Project Structure


minimal-cpp-ml/
├── data/
│ └── sample.csv # Example dataset
│
├── core/
│ ├── csv_reader.hpp # CSV parser
│ ├── preprocessor.hpp # Scaling, encoding, etc.
│ └── statistics.hpp # Mean, stddev, etc.
│
├── models/
│ ├── linear_regression.hpp # Linear regression
│ ├── logistic_regression.hpp # Logistic regression
│ └── knn_classifier.hpp # KNN classifier
│
├── examples/
│ ├── regression_example.cpp # End-to-end regression demo
│ └── classification_example.cpp # End-to-end classification demo
│
├── tests/
│ └── ... # Unit tests (Google Test or Catch2)
│
├── CMakeLists.txt
└── README.md


