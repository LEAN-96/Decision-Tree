# Decision Trees and Random Forests Project
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LEAN-96/Decision-Tree.git/HEAD?labpath=notebooks)

This repository contains a Jupyter notebook for exploring and implementing Decision Trees and Random Forests. The notebook demonstrates data preparation, visualization, model training, and evaluation on a dataset of loan data. 

## Project Structure

- **3-Decision_Trees_und_Random_Forests_Projekt-Loesung.ipynb**: The main notebook that guides you through loading the data, preprocessing, visualizing, training decision tree and random forest models, and evaluating their performance.
- **environment.yml**: Specifies the dependencies required to reproduce the notebook's environment.

## Requirements

You can run the notebook in a variety of ways:

1. **Locally**: Clone the repository and set up a Conda environment based on the `environment.yml` file.
2. **Online via MyBinder**: Directly launch the notebook in your browser without installation.

### Running Locally

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/decision-trees-random-forests.git
    cd decision-trees-random-forests
    ```

2. **Create and activate the environment**:
    Make sure you have [Anaconda](https://www.anaconda.com/) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed.
    ```bash
    conda env create -f environment.yml
    conda activate decision-tree-random-forest-environment
    ```

3. **Launch Jupyter Notebook**:
    ```bash
    jupyter notebook
    ```
    Open `3-Decision_Trees_und_Random_Forests_Projekt-Loesung.ipynb` in the Jupyter interface to run the notebook.

### Running Online via MyBinder

Click the following button to launch the notebook in a MyBinder environment:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LEAN-96/Decision-Tree.git/HEAD?labpath=notebooks)

This will open a Jupyter environment with all necessary dependencies pre-installed.

## Reproducing the Analysis

The notebook walks you through the following steps:

1. **Data Loading**: Reads in a dataset of loan data. Ensure `loan_data.csv` is available in the root directory.
2. **Data Exploration**: Summarizes and visualizes the dataset, providing insights into its structure and characteristics.
3. **Model Training**: Implements decision trees and random forests using `scikit-learn`.
4. **Evaluation**: Compares model performance using evaluation metrics like accuracy and confusion matrices.

## Requirements

- **Python**: Version specified in `environment.yml` (usually compatible with Python 3.8+).
- **Packages**: The main libraries required are:
    - `numpy`
    - `pandas`
    - `matplotlib`
    - `seaborn`
    - `scikit-learn`
    - Additional packages listed in the `environment.yml` file.

## Dependencies

Dependencies are managed in the `environment.yml` file. This setup file installs the necessary libraries when creating the environment.

## Additional Notes

- **nbgitpuller** and **sphinx-gallery** are installed for optional integration with external Git repositories and documentation generation, respectively.
- Ensure you have the necessary permissions to load the data (`loan_data.csv`) if it is not publicly available.

