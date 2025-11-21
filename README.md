# Multi-Modal_Identifier
## Overview

This folder contains four Jupyter notebooks focused on multimodal biometric signal processing and machine-learning model development. The workflows include data preprocessing, feature extraction, model training, and evaluation across several algorithms, including Graph Neural Networks (GNNs), Random Forests, and Linear Regression. These notebooks support experimentation with multi-sensor datasets—particularly those incorporating photoplethysmography (PPG) and electrocardiogram (ECG) signals—for tasks such as classification, identification, or re-identification.

Each notebook represents a different modeling approach in the development pipeline.

## Notebook Descriptions
### 1. Multi_Modal_GNN_Training.ipynb

Implements the full Graph Neural Network (GNN) training pipeline for multimodal biosignals.
Typical components include:

Loading and preprocessing multi-sensor datasets (ECG + PPG)

Constructing graph representations of signals or extracted features

Defining the GNN architecture (e.g., GCN, GraphSAGE, GAT)

Training, validation, and testing loops

Computing evaluation metrics and generating performance plots

Saving trained models for further analysis

This notebook serves as the primary GNN-based multimodal training framework.

### 2. Multi_Modal_PPG_GNN.ipynb

Focuses specifically on applying Graph Neural Networks to PPG-only data or PPG-dominant multimodal streams.
Key functionality includes:

PPG preprocessing (filtering, segmentation, normalization)

Graph construction using PPG features or time-series windows

GNN model training targeted toward PPG data characteristics

Evaluation of single-modality GNN performance

This notebook is used to compare PPG-focused models against the fully multimodal GNN approach.

### 3. Multi_Modal_PPG_LR.ipynb

Implements a Linear Regression (LR) modeling pipeline using PPG-based features.
Core components include:

Extracting statistical and morphological features from PPG signals

Preparing structured datasets for linear modeling

Training and testing the regression model

Establishing a baseline against more complex models (GNNs, Random Forests)

This notebook provides a lightweight performance baseline.

### 4. Multi_Modal_PPG_RF.ipynb

Develops and trains a Random Forest (RF) classifier or regressor using PPG features.
Includes:

Preprocessing and feature engineering for PPG data

Hyperparameter tuning for the Random Forest model

Training, validation, and visualization of results

Comparisons to linear and GNN-based models

Random Forests offer a strong, interpretable non-deep-learning benchmark within the multimodal pipeline.

## Intended Use

These notebooks support research and experimentation in multimodal biometric recognition and related tasks. Intended uses include:

Comparative evaluation of multiple machine-learning models

Signal-processing experimentation

Rapid prototyping of biosignal-based ML pipelines

Analysis of ECG/PPG sensor data using classical and modern techniques