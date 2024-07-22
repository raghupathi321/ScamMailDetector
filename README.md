

# Scam Mail Classifier

This repository contains a project for classifying scam mails and legitimate mails using a Support Vector Machine (SVM) classifier. The model achieves an accuracy of 98%.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model](#model)
- [Results](#results)

## Introduction

Email scams are a prevalent issue, causing financial and personal losses to individuals and organizations. This project aims to build a classifier that can effectively distinguish between scam mails and legitimate mails using machine learning techniques.

## Features

- **High Accuracy:** The SVM classifier achieves a 98% accuracy rate.
- **Preprocessing:** Includes text preprocessing steps such as tokenization, stemming, and vectorization.
- **User-Friendly:** Easy to use and integrate into other applications.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/raghupathi321/scam-mail-classifier.git
    ```
2. Navigate to the project directory:
    ```sh
    cd scam-mail-classifier
    ```
3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. Prepare your dataset in a CSV format with two columns: `email` and `label`.
2. Place the dataset in the project directory.
3. Run the training script to train the model:
    ```sh
    python train_model.py
    ```
4. Use the trained model to classify new emails:
    ```sh
    python classify_email.py --email "Your email content here"
    ```

## Dataset

The dataset used for training and testing the model should be in CSV format with the following columns:

- `email`: The content of the email.
- `label`: The label indicating whether the email is a scam (1) or legit (0).

Ensure your dataset is properly preprocessed before training the model.

## Model

The model uses a Support Vector Machine (SVM) classifier. The key steps in the pipeline include:

1. **Text Preprocessing:** Tokenization, stemming, and vectorization using TF-IDF.
2. **Model Training:** Training the SVM classifier with the preprocessed data.
3. **Evaluation:** Evaluating the model performance on a test set.

## Results

The SVM classifier achieves an accuracy of 98% on the test set. The performance metrics are as follows:

- **Accuracy:** 0.98
- **Confusion Matrix:** `[[889, 0], [25, 120]]`
- **Precision Score:** 1.0

