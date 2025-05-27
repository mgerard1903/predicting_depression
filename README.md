# Exploratory Data Analysis of Student Depression Dataset

_A deep dive EDA on student depression risk factors using survey and activity metrics to uncover patterns and insights._

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

This project performs a comprehensive exploratory data analysis on the student depression dataset. We examine distributions, correlations, and relationships among survey responses and activity metrics to identify patterns linked to depression risk.

## Key Features

- **Univariate Analysis**: Histograms, boxplots, and density plots for each feature.  
- **Bivariate Analysis**: Scatter plots, bar charts, and violin plots comparing features against depression status.  
- **Correlation Analysis**: Heatmaps and pairplots to reveal feature interdependencies.  
- **Missing Value Assessment**: Visualization of missingness patterns and imputation strategies.  
- **Dimensionality Reduction**: PCA and t-SNE projections for pattern discovery.  
- **Outlier Detection**: Identification and visualization of anomalous observations.

## Tech Stack

- **Language:** Python 3.8+  
- **Notebook:** Jupyter Notebook (`Assignment_1.ipynb`)  
- **Libraries:** pandas, numpy, matplotlib, seaborn, plotly, scikit-learn  

## Installation

```bash
git clone https://github.com/your-username/student-depression-eda.git
cd student-depression-eda
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate   # Windows
pip install -r requirements.txt
```

## Datasets

- **`student_depression_dataset.csv`**: Survey and activity metrics of students (features include sleep hours, study time, social interaction, past mental health history, etc.)  
- Place the CSV in the `data/` directory before running analysis.

## Usage

1. **Run the EDA notebook**:  
   ```bash
   jupyter notebook Assignment_1.ipynb
   ```  
2. **Explore sections**:  
   - Data overview and summary statistics  
   - Feature distributions and missing value visualizations  
   - Correlation heatmap and pairwise plots  
   - PCA and t-SNE visualizations  
   - Outlier and anomaly detection  

## Project Structure

```
student-depression-eda/
├── README_EDA.md               # This file
├── assignment_1.ipynb          # EDA notebook
├── data/
│   └── student_depression_dataset.csv
├── requirements.txt            # Python dependencies
└── outputs/
    ├── histograms/
    ├── heatmaps/
    └── pca_tsne_plots/
```

## Configuration

- **Visualization Styles**: Modify seaborn themes and plotly templates in the notebook.  
- **PCA Components**: Adjust number of components for dimensionality reduction.  
- **Outlier Thresholds**: Change z-score or IQR parameters for outlier detection.
