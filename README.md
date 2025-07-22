# Endometriosis Onset Prediction

This repository contains a comprehensive machine learning workflow for predicting the onset of endometriosis in women of reproductive age. The project leverages various classification algorithms and data preprocessing techniques to build a robust predictive model, with a focus on logistic regression.

---

## Table of Contents

- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Requirements](#requirements)
- [Usage](#usage)
- [Modeling Pipeline](#modeling-pipeline)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

---

## Problem Statement

Endometriosis is a chronic gynecological condition affecting millions of women worldwide, often leading to pain, infertility, and reduced quality of life. Early diagnosis is challenging with traditional clinical methods, leading to delayed treatment. This project aims to develop an advanced machine learning system to predict the onset of endometriosis using structured patient data.

---

## Dataset

The main dataset used is `structured_endometriosis_data.csv`, which contains 10,000 rows and 7 columns:

- `Age`: Age of the patient (years)
- `Menstrual_Irregularity`: Binary indicator (1: Yes, 0: No)
- `Chronic_Pain_Level`: Continuous score (severity)
- `Hormone_Level_Abnormality`: Binary indicator (1: Yes, 0: No)
- `Infertility`: Binary indicator (1: Yes, 0: No)
- `BMI`: Body Mass Index
- `Diagnosis`: Target variable (1: Endometriosis, 0: No Endometriosis)

---

## Project Structure

```
Endometriosis/
├── Endometriosis_type_shii.ipynb   # Main Jupyter Notebook (machine learning pipeline)
├── structured_endometriosis_data.csv # Dataset
├── README.md                       # Project documentation
```

---

## Requirements

Install the following Python packages to run the notebook:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

**Python Version:** 3.7 or above is recommended.

---

## Usage

1. **Clone the repository:**

   ```bash
   git clone https://github.com/VindelM/Endometriosis.git
   cd Endometriosis
   ```

2. **Prepare the environment:**
   - Make sure `structured_endometriosis_data.csv` is in the project directory.
   - Install required packages (see [Requirements](#requirements)).

3. **Run the Notebook:**
   - Open `Endometriosis_type_shii.ipynb` in Jupyter Notebook or Google Colab.
   - Execute all cells sequentially.

---

## Modeling Pipeline

### 1. Data Loading and Exploration

- Load the CSV data into a pandas DataFrame.
- Display the first few rows and check for duplicates.

### 2. Data Preparation

- Separate features (`X`) and target (`y`).
- Split the data into training and testing sets (80/20 split).

### 3. Feature Scaling

- Standardize features using `StandardScaler` to improve model convergence.

### 4. Model Training

- Train a logistic regression model on the scaled training data.
- Optionally, other classifiers (Decision Tree, Random Forest, SVM, XGBoost, etc.) are available for experimentation.

### 5. Model Evaluation

- Evaluate model accuracy on the test set.
- Generate a classification report (precision, recall, F1-score).

#### Objective

- Achieve at least **95% accuracy** in predicting endometriosis onset.

---

## Results

- The notebook demonstrates step-by-step how to preprocess data, train, and evaluate a logistic regression model.
- You can experiment with different classifiers and hyperparameters for improved performance.
- Visualization tools (`matplotlib`, `seaborn`) are available for exploratory data analysis and results interpretation.

---

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for enhancements, bug fixes, or new features.


---

## Acknowledgements

- Data is fictional or anonymized for educational purposes.
- This project was inspired by the need for improved diagnostic tools in women's health.

---

## Contact

For questions or collaboration, please contact [VindelM](https://github.com/VindelM).
