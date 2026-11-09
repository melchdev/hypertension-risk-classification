# Hypertension Risk Classification

## Overview

This project explores the use of supervised machine learning techniques to identify patterns associated with hypertension.

Developed as part of the *Principles of Machine Learning* course at Universidad de los Andes, Colombia, the project focuses on building and comparing classification models using Decision Trees and K-Nearest Neighbors (KNN).

The main objective is to analyze how demographic, physiological, and lifestyle-related variables contribute to hypertension classification.

## Objectives

- Explore and assess the quality of the dataset.
- Identify and handle duplicate and invalid records.
- Prepare numerical and categorical features for machine learning.
- Build and optimize Decision Tree and KNN classifiers.
- Compare KNN performance with and without feature scaling.
- Evaluate model generalization and predictive performance.
- Analyze the most relevant features used by the Decision Tree model.

## Dataset

The dataset contains 1,990 initial observations and 13 variables describing demographic, physiological, and lifestyle characteristics.

The target variable is `Hipertension`, which indicates whether an individual has hypertension.

Some of the features include:

- Age
- Salt intake
- Stress level
- Cholesterol
- Sleep duration
- Body Mass Index (BMI)
- Medication
- Family history
- Physical activity
- Smoking status
- Glucose
- Heart disease history

A data dictionary is included to describe the variables and their characteristics.

## Methodology

The project follows a supervised machine learning workflow:

1. Data exploration and profiling.
2. Data quality assessment: uniqueness, consistency, completeness, and validity.
3. Data cleaning and preprocessing.
4. Train/test splitting (80/20).
5. Decision Tree classification and hyperparameter optimization.
6. KNN classification with feature scaling.
7. KNN classification without feature scaling.
8. Cross-validation and model selection.
9. Test-set evaluation and confusion matrices.
10. Feature importance analysis.
11. Bootstrap estimation of accuracy and confidence intervals.

## Models

**Decision Tree Classifier**

Optimized using GridSearchCV and five-fold cross-validation, exploring different splitting criteria, maximum depths, and minimum samples required to split a node.

**K-Nearest Neighbors (KNN)**

Evaluated using different neighborhood sizes and preprocessing strategies. Two approaches are compared: one with numerical feature scaling and another without scaling.

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Macro F1-score
- Confusion matrices
- Cross-validation scores
- Training and test accuracy comparison
- Bootstrap confidence intervals for accuracy

## Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Repository Structure

```text
hypertension-risk-classification/
│
├── data/
│   ├── Datos_hipertension.csv
│   └── Diccionario_Datos_hipertension.xlsx
│
├── notebooks/
│   └── microproyecto2.ipynb
│
├── .gitignore
├── README.md
└── requirements.txt
```

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/MelchDev/hypertension-risk-classification.git
   ```

2. Navigate to the project directory:

   ```bash
   cd hypertension-risk-classification
   ```

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `notebooks/microproyecto2.ipynb` and run the cells.

## Academic Context

Developed as an individual academic project for the Master's program in Artificial Intelligence at Universidad de los Andes, Colombia.

## Acknowledgements

This project was developed using the academic materials and dataset provided for the *Principles of Machine Learning* course at Universidad de los Andes.

## Disclaimer

This project is an academic exercise in machine learning. Its models are intended for educational and analytical purposes and should not be interpreted as medical diagnostic tools.
