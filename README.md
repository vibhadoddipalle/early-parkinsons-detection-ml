# Vocal Acoustic Biomarker Analysis for Early Parkinson’s Disease Detection

## Project Overview
This project applies machine learning techniques to vocal acoustic biomarkers for the early detection of Parkinson’s disease. The goal is to classify voice recordings as either Parkinson’s or healthy using extracted speech signal features.

Two models were implemented and compared:
- Logistic Regression (baseline model)
- Neural Network (nonlinear model)

Model evaluation was performed using stratified grouped 5-fold cross-validation to ensure robust performance and prevent data leakage across subjects.

---

## Repository Structure

```
├── README.md
├── Parkinsons_Disease.csv (dataset)
├── ⭐Final Project Parkinson's Predictor.ipynb (Notebook containing Code, Results, and Tests)
├── Vocal Acoustic Biomarker Analysis for Early Parkinson’s Disease Detection_ A Machine Learning Approach BE175_ Final Report.pdf

````

---

## Installation / Dependencies

To run this project, install the required Python libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow
````

---

## How to Run the Project

### Option 1: Google Colab (Recommended)

1. Open `Parkinsons_Detection.ipynb` in Google Colab
2. Upload the dataset (`Parkinsons_Disease.csv`) when prompted
3. Run all cells sequentially

### Option 2: Local Environment

1. Clone the repository:

```bash
git clone <repository-url>
```

2. Install dependencies (see above)

3. Run the Jupyter notebook:

```bash
jupyter notebook Parkinsons_Detection.ipynb
```

---

## Machine Learning Models

### Logistic Regression

A baseline classification model implemented using Scikit-learn. It outputs probabilities for binary classification of Parkinson’s disease based on vocal features.

### Neural Network

A feedforward neural network implemented using TensorFlow/Keras to capture nonlinear relationships in the dataset.

---

## Evaluation Method

* Stratified grouped 5-fold cross-validation
* Metrics: Accuracy, Precision, Recall, F1-score
* Grouping ensures recordings from the same subject remain in the same fold to prevent data leakage

---

## Notes

* This project was developed using Google Colab
* The dataset contains vocal acoustic measurements derived from voice recordings
