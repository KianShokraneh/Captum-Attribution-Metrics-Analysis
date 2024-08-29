# Captum Attribution Metrics Analysis

This repository contains a Python script that demonstrates an initial analysis of various attribution methods using the Captum library on a ResNet18 model trained on the CIFAR-10 dataset. The script evaluates and compares the effectiveness of different interpretability techniques by calculating infidelity and sensitivity metrics.

## Overview

The project focuses on applying several attribution methods to understand and interpret the predictions made by the model. The methods include:

- **Integrated Gradients**: Attributes the prediction to its input features by integrating gradients from a baseline to the input.
- **Gradient SHAP**: Combines SHAP values and gradients to attribute the prediction to input features.
- **Saliency**: Highlights the regions in the input that are most important for the model's predictions.
- **Guided Backpropagation**: Provides visual explanations by combining backpropagation with saliency maps.
- **Occlusion**: Systematically removes each feature to assess its importance for the model's prediction.

## Key Features

- **Infidelity Metric**: Measures how much the attributions differ when small perturbations are applied to the input, providing insight into the robustness of the explanations.
- **Sensitivity Metric**: Evaluates how sensitive the attribution method is to changes in the input, indicating how well the method reflects the model's behavior.
- **Comparative Analysis**: The script compares the performance of different attribution methods on CIFAR-10 test samples by calculating and printing overall infidelity and sensitivity scores.
