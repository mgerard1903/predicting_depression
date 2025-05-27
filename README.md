# Predicting Student Depression Risk Using Machine Learning

_A supervised learning pipeline to identify at-risk students for depression based on survey data and activity metrics._

## Table of Contents

1. [Description](#description)  
2. [Key Features](#key-features)  
3. [Tech Stack](#tech-stack)  
4. [Installation](#installation)  
5. [Datasets](#datasets)  
6. [Usage](#usage)  
7. [Project Structure](#project-structure)  
8. [Configuration](#configuration)

---

## Description

This project develops a predictive model to screen for depression in students using survey responses, academic performance, and activity data. We explore data preprocessing, feature selection, and apply classifiers (logistic regression, random forest, SVM) with hyperparameter tuning to achieve accurate risk predictions.

## Key Features

- **Data Preprocessing**: Handling missing values, encoding categorical variables, and scaling numerical features.  
- **Exploratory Analysis**: Visualizations of feature distributions and correlations with depression outcomes.  
- **Feature Selection**: Recursive feature elimination and importance ranking to identify key predictors.  
- **Modeling**: Logistic Regression, Random Forest, SVM with GridSearchCV for hyperparameter optimization.  
- **Evaluation**: Metrics including accuracy, precision, recall, F1-score, ROC AUC, and confusion matrices.  
- **Interpretability**: SHAP value analysis to explain individual risk predictions.

## Tech Stack

- **Language:** Python 3.8+  
- **Notebook:** Jupyter Notebook (`Assignment_2.ipynb`)  
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn, shap  

## Installation

```bash
git clone https://github.com/your-username/student-depression-prediction.git
cd student-depression-prediction
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate   # Windows
pip install -r requirements.txt
```

## Datasets

- **`student_depression_dataset.csv`**: Survey and activity metrics of students (features include sleep hours, study time, social interaction, past mental health history, etc.)  
- Place the CSV file in the `data/` directory.

## Usage

1. **Run the analysis notebook**:  
   ```bash
   jupyter notebook Assignment_2.ipynb
   ```  
2. **Follow sections**:  
   - Data loading and cleaning  
   - Exploratory data analysis  
   - Feature engineering and selection  
   - Model training and evaluation  
   - SHAP interpretability analysis  
3. **View outputs** in `outputs/` folder: plots, model reports, and SHAP visualizations.

## Project Structure

```
student-depression-prediction/
├── README.md                    # This file
├── data/
│   └── student_depression_dataset.csv
├── Assignment_2.ipynb           # Analysis notebook
├── requirements.txt             # Python dependencies
├── outputs/
│   ├── correlation_heatmap.png
│   ├── roc_curves.png
│   └── shap_summary.png
└── models/
    └── best_model.pkl
```

## Configuration

- **Test Size**: Default 20%; adjust in notebook split settings.  
- **Random State**: Set seed for reproducibility.  
- **Hyperparameter Grids**: Modify search spaces for classifiers in GridSearchCV.
