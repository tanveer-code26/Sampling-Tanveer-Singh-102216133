# Credit Card Sampling Assignment using SMOTE

This Project aims to perform various sampling techniques on a dataset, applying machine learning models, and analyzing the results to determine the most effective sampling method for each model. The dataset used is highly imbalanced, and techniques like SMOTE (Synthetic Minority Oversampling Technique) are applied to handle this imbalance. The project evaluates multiple models and sampling techniques to find the best performing combination.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Dataset](#dataset)
- [Usage](#usage)
- [Models and Techniques](#models-and-techniques)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project aims to demonstrate the effectiveness of different sampling techniques on imbalanced datasets. By applying these techniques, we can improve the performance of machine learning models and achieve better accuracy metrics. This project implements:

- Data preprocessing and scaling using `StandardScaler`.
- Oversampling the minority class using SMOTE.
- Comparison of multiple machine learning models.
- Evaluation of sampling techniques for optimal performance.

## Features

- Preprocessing of raw data, including handling missing values.
- Handling class imbalance with SMOTE.
- Sampling different proportions of the dataset.
- Implementation of various machine learning models:
  - Logistic Regression
  - Random Forest Classifier
  - Support Vector Classifier (SVC)
  - K-Nearest Neighbors (KNN)
  - Gradient Boosting Classifier
- Evaluation of model accuracy and comparison of sampling techniques.
- Output of results in CSV format for analysis.

## Installation

To set up the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure `imblearn` is installed:
   ```bash
   pip install imbalanced-learn
   ```

## Dataset

The dataset used is named `Creditcard_data.csv`, which contains:

1. Samples: Different data samples used for training and evaluation.

2. Sampling Methods: Techniques applied to handle imbalanced classes.

3. Models: Machine learning models evaluated.

4. Accuracy: Performance metric for each model and sampling method.

Ensure the dataset is in the root directory or update the file path in the code.

## Usage

1. Prepare the dataset:
   - Place `Creditcard_data.csv` in the project directory.

2. Open the Jupyter Notebook file Sampling.ipynb and execute the cells.

3. Outputs:
   - `best_sampling_per_model.csv`: Contains the best accuracy for each model with the corresponding sampling technique.
   - `sampling_results.csv`: Contains detailed results for all combinations of models, sampling techniques, and samples.

## Models and Techniques

### Models
- **Logistic Regression**
- **Random Forest Classifier**
- **Support Vector Classifier (SVC)**
- **K-Nearest Neighbors (KNN)**
- **Gradient Boosting Classifier**

### Sampling Techniques
- SMOTE is used to balance the classes.
- Different dataset sampling percentages are tested (15%, 25%, 35%, 45%, 55%).
- Random sampling techniques are applied to reduce the size of the training data.

## Results

The performance of each model and sampling technique is evaluated using accuracy as the metric. The results are saved in CSV files for further analysis. Key findings include:
- The best performing model for the given dataset.
- The impact of sampling percentages and techniques on model performance.

The table below summarizes the accuracies obtained for each sampling technique and model:

| Sampling Technique | M1    | M2    | M3    | M4    | M5    |
|--------------------|-------|-------|-------|-------|-------|
| Sampling1          | 50.10 | 59.25 | 90.45 | 78.25 | 81.25 |
| Sampling2          | 52.24 | 65.27 | 72.41 | 56.24 | 12.85 |
| Sampling3          | 63.18 | 68.72 | 32.17 | 47.23 | 57.36 |
| Sampling4          | 69.23 | 28.36 | 42.58 | 33.44 | 32.25 |
| Sampling5          | 70.12 | 30.25 | 41.85 | 40.12 | 52.74 |

Key Observations:
- Sampling3 yielded the highest accuracy for M1.
- Sampling1 was most effective for M3.
- Sampling5 performed better for M2 and M5.

## Contributors
- **[Tanveer Singh]** - [Your Email/LinkedIn/GitHub Profile]

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

