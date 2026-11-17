# Task 39 — Confusion Matrix Using Python

## Project Overview

This project demonstrates how to generate and interpret a confusion matrix for a classification model using Python and Scikit-learn.

The Breast Cancer Wisconsin Diagnostic Dataset is used to perform binary classification.

A Decision Tree Classifier is trained to predict whether a tumour is benign or malignant.

The confusion matrix is generated to evaluate the classification results and understand True Positive, True Negative, False Positive, and False Negative outcomes.

## Objectives

- Understand the concept of a confusion matrix.
- Load and explore a classification dataset.
- Select input features and target variables.
- Train a Decision Tree classification model.
- Generate predictions on testing data.
- Calculate the confusion matrix.
- Understand TP, TN, FP, and FN.
- Visualize the confusion matrix using Matplotlib and Seaborn.
- Evaluate classification performance.

## Dataset Description

The project uses the Breast Cancer Wisconsin Diagnostic Dataset from Scikit-learn.

- Total observations: 569
- Input features: 30
- Target classes: 2

### Target Classes

| Target Code | Diagnosis |
|---|---|
| 0 | Malignant |
| 1 | Benign |

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Joblib
- Google Colab
- Jupyter Notebook

## Model Used

**Algorithm:** Decision Tree Classifier

**Classification Type:** Binary Classification

**Training and Testing Split:** 80:20

**Maximum Tree Depth:** 4

The model is trained using the `fit()` method and predictions are generated using the `predict()` method.

## Confusion Matrix

A confusion matrix is an evaluation tool used to compare actual class labels with predicted class labels.

This project considers Malignant as the positive class and Benign as the negative class.

The matrix is arranged as:

| | Predicted Benign | Predicted Malignant |
|---|---|---|
| Actual Benign | True Negative | False Positive |
| Actual Malignant | False Negative | True Positive |

### Explanation

- **True Positive (TP):** Actual malignant cases correctly predicted as malignant.
- **True Negative (TN):** Actual benign cases correctly predicted as benign.
- **False Positive (FP):** Actual benign cases incorrectly predicted as malignant.
- **False Negative (FN):** Actual malignant cases incorrectly predicted as benign.

## Visualization

The confusion matrix is visualized using:

- Scikit-learn `ConfusionMatrixDisplay`
- Seaborn `heatmap()`
- Matplotlib

The visualization helps identify correct and incorrect classifications.

## Evaluation Metrics

The project evaluates the classification model using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

The actual evaluation values are available in `evaluation_summary.csv`.

## Project Workflow

1. Import Python libraries.
2. Load the Breast Cancer dataset.
3. Explore dataset information.
4. Select features and target.
5. Split data into training and testing sets.
6. Train Decision Tree Classifier.
7. Generate predictions.
8. Generate confusion matrix.
9. Extract TP, TN, FP, and FN.
10. Visualize confusion matrix.
11. Calculate evaluation metrics.
12. Export CSV files and trained model.

## Project Files

- `Task_39_Confusion_Matrix.ipynb` — Complete notebook.
- `breast_cancer_dataset.csv` — Original dataset.
- `prepared_classification_dataset.csv` — Prepared dataset.
- `classification_features.csv` — Input features.
- `classification_target.csv` — Target variable.
- `confusion_matrix.csv` — Confusion matrix values.
- `confusion_matrix_results.csv` — TP, TN, FP, and FN.
- `classification_predictions.csv` — Actual and predicted values.
- `evaluation_summary.csv` — Evaluation metrics.
- `classification_report.csv` — Detailed classification report.
- `decision_tree_model.joblib` — Saved trained model.
- `requirements.txt` — Required Python libraries.
- `project_report.pdf` — Project documentation.
- `charts/confusion_matrix.png` — Confusion matrix visualization.
- `screenshots/` — Project execution screenshots.

## How to Run

1. Install the required libraries using `pip install -r requirements.txt`.
2. Open the Jupyter Notebook.
3. Execute all notebook cells sequentially.
4. Review the generated confusion matrix.
5. Examine TP, TN, FP, and FN.
6. Review the evaluation metrics.

## Results

The model generates predicted diagnosis values for the testing dataset.

The confusion matrix summarizes correct and incorrect classifications.

The actual TP, TN, FP, FN, accuracy, precision, recall, and F1-score are stored in the respective CSV files.

## Conclusion

This project demonstrates the practical use of a confusion matrix in evaluating classification models.

It provides an understanding of True Positive, True Negative, False Positive, and False Negative outcomes.

The visualization makes it easier to understand the model's classification performance and identify prediction errors.

**Note:** This is an educational machine-learning project and is not intended for medical diagnosis.
