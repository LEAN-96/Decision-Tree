# Decision Trees and Random Forests Project

## 1. Project Overview

This project demonstrates the implementation of **Decision Trees** and **Random Forests**, two popular machine learning algorithms used for classification tasks. The objective is to train models on a dataset, evaluate their performance, and visualize the results. The notebook covers data preprocessing, model building, training, evaluation, and visualization of the performance metrics.


### Dataset
The dataset used in this classification problem aims to predict **loan repayment status**. The two classes are:
- **Class 0**: Loan was **repaid**.
- **Class 1**: Loan was **not repaid**.

 The data is preprocessed and split into training and testing sets. The notebook walks through the steps of loading the dataset, preparing it for model training, and evaluating the models' performance.

### Machine Learning Methods
The notebook implements:
- **Decision Trees**: A tree-structured classifier where internal nodes represent features, branches represent decision rules, and leaf nodes represent outcomes.
- **Random Forests**: An ensemble method that builds multiple decision trees and merges them to obtain a more accurate and stable prediction.

The goal is to classify whether a loan will be repaid (class 0) or not (class 1), based on various financial features. Random Forests were chosen alongside Decision Trees to enhance model performance by leveraging the ensemble method's ability to generalize better.

### Notebook Overview
The notebook contains several sections:
1. **Data Loading and Preprocessing**: Loads the dataset and preprocesses it for model training.
2. **Model Building**: Defines both Decision Tree and Random Forest classifiers using scikit-learn.
3. **Model Training**: Trains the models on the training data.
4. **Evaluation**: Evaluates the models on test data using metrics like accuracy.
5. **Visualization**: Plots graphs to visualize model performance.
## Requirements

### Running Locally

1. **Clone the repository**:
    ```bash
    git clone https://github.com/LEAN-96/Decision-Tree.git
    cd decision-trees-random-forests
    ```

2. **Create a virtual environment**:
    Using `venv`:
    ```bash
    python3 -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

    Or using `conda`:
    ```bash
    conda create --name ml-env python=3.8
    conda activate ml-env
    ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Launch Jupyter Notebook**:
    ```bash
    jupyter notebook
    ```
    Open `3-Decision_Trees_und_Random_Forests.ipynb` in the Jupyter interface to run the notebook.

### Running Online via MyBinder

MyBinder is a free service that allows you to run Jupyter notebooks online without needing to install anything locally. It creates an interactive environment where you can execute notebooks directly from your browser

Click the following button to launch the notebook in a MyBinder environment. This will open a Jupyter environment with all necessary dependencies pre-installed.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LEAN-96/Decision-Tree.git/HEAD?labpath=notebooks)

Once MyBinder loads:
1. Navigate to the notebook (`3-Decision_Trees_und_Random_Forests.ipynb`) in the file browser on the left side of your screen.
2. Open the notebook by clicking on it.
3. To run all cells in sequence, click "Cell" -> "Run All" from the top menu or run each cell individually by selecting it and pressing `Shift + Enter`.
4. Wait for each cell to execute; outputs will appear below each code block as they complete.

By using MyBinder, you can explore and run this notebook without installing any software locally.



## 3. Reproducing the Results

To reproduce the results from this project:

1. Open the provided notebook (`3-Decision_Trees_und_Random_Forests.ipynb`) from the Jupyter interface.
2. Run each cell sequentially by pressing `Shift + Enter` or by clicking "Run" in the Jupyter toolbar.
3. Ensure that all cells execute without errors.
4. At the end of execution, observe accuracy metrics and visualizations to evaluate model performance.

### Interpreting Results:

After training the models (e.g., Decision Tree or Random Forest), you will typically evaluate their performance using several key metrics. These metrics help you understand how well the model is performing on both the training and test datasets.

Both models (Decision Tree and Random Forest) are evaluated using the following metrics:

- **Precision**: The proportion of true positive predictions out of all positive predictions made by the model.
  - High precision means fewer false positives.
  
- **Recall (Sensitivity)**: The proportion of actual positives that were correctly identified by the model.
  - High recall means fewer false negatives.
  
- **F1-Score**: The harmonic mean of precision and recall, providing a balance between the two.
  - Useful when dealing with imbalanced classes.
  
- **Support**: The number of actual occurrences of each class in the dataset.

## Confusion Matrix:
The confusion matrix shows the breakdown of correct and incorrect predictions:
- **True Positives (TP)**: Correctly predicted loans that were not repaid (class 1).
- **True Negatives (TN)**: Correctly predicted loans that were repaid (class 0).
- **False Positives (FP)**: Incorrectly predicted as not repaid when they were repaid.
- **False Negatives (FN)**: Incorrectly predicted as repaid when they were not repaid.

## Decision Tree Results:
- **Class 0 (Repaid)**:
  - Precision: 0.85, Recall: 0.82, F1-score: 0.84
- **Class 1 (Not Repaid)**:
  - Precision: 0.19, Recall: 0.24, F1-score: 0.21
- **Overall Accuracy**: 73%

**Confusion Matrix:**

[[1993, 438],
[338, 105]]


## Random Forest Results:
- **Class 0 (Repaid)**:
  - Precision: 0.85, Recall: 1.00, F1-score: 0.92
- **Class 1 (Not Repaid)**:
  - Precision: 0.47, Recall: 0.02, F1-score: 0.04
- **Overall Accuracy**: 85%

**Confusion Matrix:**

[[2421, 10],
[434, 9]]


## Summary:
Both models perform well in predicting loans that will be repaid (**class 0**) but struggle with identifying loans that will not be repaid (**class 1**). Random Forest achieves higher accuracy but still has poor recall for class "1", indicating a need for further tuning or handling of class imbalance.