# Genetic Algorithm-Based Neural Network Hyperparameter Optimization

## Overview

This project investigates the use of a **Genetic Algorithm** for **neural network hyperparameter optimization** and compares its performance against two common baseline methods: **Grid Search** and **Random Search**.

The goal of this study is to determine whether evolutionary search can identify strong neural network hyperparameter configurations more efficiently than traditional tuning strategies when all methods are evaluated under the same computational budget.

## Research Question

Can a **Genetic Algorithm** find high-performing neural network hyperparameter configurations more effectively than **Grid Search** and **Random Search** under a fixed evaluation budget?

## Methods Compared

- **Grid Search**
- **Random Search**
- **Genetic Algorithm**

## Hyperparameters Tuned

The following neural network hyperparameters are explored in this project:

- **Learning rate**
- **Number of hidden layers**
- **Number of neurons per layer**
- **Batch size**
- **Activation function**

## Model and Dataset

This project uses a **fully connected neural network** implemented with `MLPClassifier` from `scikit-learn`.

The experiments are conducted on the **Digits dataset**, a handwritten digit classification dataset included with `scikit-learn`.

## Evaluation Criteria

Each tuning method is evaluated using:

- **Best validation accuracy**
- **Test accuracy of the best configuration**
- **Convergence behavior over evaluations**
- **Runtime performance**
- **Robustness across multiple random seeds**

## Experimental Design

To ensure fairness, all tuning methods are compared under the same evaluation budget. Multiple random seeds are used to improve the reliability of the results and reduce the effect of stochastic variation.

## Repository Structure

```text
.
├── README.md
├── term_experiments.ipynb
├── ref.bib
└── paper/