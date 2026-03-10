# Supervised Learning System – Heart Disease Binary Classification

This project demonstrates a supervised learning system that predicts whether a patient has **heart disease** or not, using a **Random Forest Classifier** built with **scikit-learn**.

## Dataset

- **Source:** [Kaggle Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- **Records:** 303 patient samples
- **Features:** 13 clinical attributes (age, sex, chest pain type, blood pressure, cholesterol, etc.)
- **Target:** `target` column — `1` = heart disease present, `0` = no heart disease

## How to Run

### Prerequisites

- Python 3.8+
- Jupyter Notebook (or VS Code with Jupyter extension)

### Step 1: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 2: Launch Jupyter Notebook

```bash
jupyter notebook A3_demo.ipynb
```

Or if using VS Code, simply open `A3_demo.ipynb` and select a Python kernel.

### Step 3: Run All Cells

- In Jupyter: Click **Cell** → **Run All**
- In VS Code: Click **Run All** button at the top of the notebook

The notebook will:
1. Load and preview the heart disease dataset
2. Display the class distribution
3. Preprocess, split (80/20 stratified), and scale the data
4. Train a Random Forest model (200 estimators)
5. Evaluate with confusion matrix (TP/TN/FP/FN), average accuracy, balanced accuracy, precision, recall, F1-score, and ROC-AUC
6. Show 3 sample input/output predictions

## Project Structure

```
├── A3_demo.ipynb      # Main notebook with all code
├── heart.csv          # Heart disease dataset
├── requirements.txt   # Python dependencies
└── README.md          # This file
```

## AI Method

- **Algorithm:** Random Forest Classifier (200 trees)
- **Library:** scikit-learn (`sklearn.ensemble.RandomForestClassifier`)
