# Credit Card Fraud Detection with SMOTE

This project focuses on detecting credit card fraud using various machine learning models. The dataset used is highly imbalanced, and techniques like SMOTE (Synthetic Minority Oversampling Technique) are applied to handle this imbalance. The project evaluates multiple models and sampling techniques to find the best performing combination.

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

Credit card fraud detection is a challenging task due to the imbalanced nature of the data. This project implements:

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

- **Features**: Transaction details (e.g., transaction amount, time, and other numerical data).
- **Target**: `Class` column, where 1 represents fraudulent transactions and 0 represents legitimate ones.

Ensure the dataset is in the root directory or update the file path in the code.

## Usage

1. Prepare the dataset:
   - Place `Creditcard_data.csv` in the project directory.

2. Run the script:
   ```bash
   python fraud_detection.py
   ```

3. Outputs:
   - `best_sampling_per_model1.csv`: Contains the best accuracy for each model with the corresponding sampling technique.
   - `sampling_results1.csv`: Contains detailed results for all combinations of models, sampling techniques, and samples.

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

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

