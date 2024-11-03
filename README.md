# Decision Trees and Random Forests Project

## 1. Project Overview

This project demonstrates the implementation of **Decision Trees** and **Random Forests**, two popular machine learning algorithms used for classification tasks. The objective is to train models on a dataset, evaluate their performance, and visualize the results. The notebook covers data preprocessing, model building, training, evaluation, and visualization of the performance metrics.


### Dataset
The dataset used in this project is suitable for classification tasks (e.g., Iris or a similar open-source dataset). The data is preprocessed and split into training and testing sets. The notebook walks through the steps of loading the dataset, preparing it for model training, and evaluating the models' performance.

### Machine Learning Methods
The notebook implements:
- **Decision Trees**: A tree-structured classifier where internal nodes represent features, branches represent decision rules, and leaf nodes represent outcomes.
- **Random Forests**: An ensemble method that builds multiple decision trees and merges them to obtain a more accurate and stable prediction.

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
- **Accuracy**: The accuracy metric shows how well each model performs on both training and test datasets.
- **Confusion Matrix**: Visualizes how well each class is predicted by comparing actual vs predicted labels.
- **Feature Importance (Random Forest)**: Shows which features contribute most to the predictions made by Random Forest.

