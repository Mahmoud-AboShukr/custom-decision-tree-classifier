# From-Scratch Decision Tree Classifier

A Python project that implements a decision tree classifier from scratch and evaluates it on synthetic and classical benchmark datasets. The project focuses on the core mechanics of tree-based learning, including dataset partitioning, Gini impurity, information gain, recursive tree construction, prediction, decision boundary visualization, learning curves, and confusion-matrix-based evaluation.

## Overview

This project builds a decision tree classifier without relying on a ready-made tree implementation from a machine learning library. The notebook walks through the full pipeline step by step:

- defining split questions
- partitioning datasets
- computing class counts and Gini impurity
- selecting optimal splits using information gain
- recursively constructing the tree
- making predictions from leaf probabilities
- evaluating performance with accuracy and confusion matrices
- visualizing learning curves and decision boundaries

The implementation is then tested on:
- a synthetic 2D binary classification dataset
- the Iris dataset
- the Wine dataset

## Features

- From-scratch implementation of a decision tree classifier
- Binary and multi-class classification experiments
- Synthetic 2D dataset generation for intuitive visualization
- Learning curve analysis
- Decision boundary plotting
- Confusion matrix reporting using NumPy
- Experiments on Iris and Wine benchmark datasets

## Repository Structure

```text
decision-tree-from-scratch/
├── README.md
├── requirements.txt
└── custom-decision-tree-classifier.ipynb
```

## Installation

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/your-username/decision-tree-from-scratch.git
cd decision-tree-from-scratch
pip install -r requirements.txt
```

## Usage

Open the notebook and run the cells in order:

```bash
jupyter notebook code.ipynb
```

The notebook includes:
1. synthetic data generation
2. decision tree construction from scratch
3. training and prediction
4. visualization of the learned decision boundary
5. learning curve analysis
6. experiments on Iris and Wine datasets

## Main Concepts Implemented

### 1. Question-based splitting
Each candidate split is represented as a question over one feature and a threshold value.

### 2. Impurity and information gain
The model evaluates candidate splits using Gini impurity and information gain.

### 3. Recursive tree growth
The tree is built recursively until no useful split is found.

### 4. Leaf-based prediction
Each leaf stores class probabilities based on the training samples that reach it.

## Datasets

### Synthetic 2D dataset
A randomly generated binary classification dataset used to visualize the behavior of the model and the learned decision boundary.

### Iris dataset
A classic multi-class dataset for evaluating the tree on structured tabular data.

### Wine dataset
A higher-dimensional benchmark dataset used to test the same implementation on another multi-class setting.

## Dependencies

The project relies on:

- numpy
- matplotlib
- scikit-learn
- jupyter

## Possible Improvements

- add support for entropy as an alternative split criterion
- include max depth and minimum samples per split controls
- add train/test split evaluation instead of train-only accuracy
- compare the custom implementation against scikit-learn's `DecisionTreeClassifier`
- refactor notebook code into reusable Python modules

