
# Predicting Hazardous Near-Earth Objects (NEOs)

## Project Overview

This project aims to predict whether a Near-Earth Object (NEO) is hazardous using machine learning techniques. The dataset includes various features related to the physical and orbital characteristics of asteroids. The objective is to develop a model that can effectively classify NEOs based on these attributes.

## Dataset

The dataset used for this project contains:

- **Orbital Parameters**: Eccentricity, semi-major axis, perihelion distance, inclination, etc.
- **Physical Characteristics**: Estimated diameter, absolute magnitude, and more.
- **Close Approach Data**: Minimum orbit intersection distance (MOID), Earth close approach distance, and relative velocity.
- **Target Variable**: `hazardous` (binary classification: 1 if hazardous, 0 if not)

## Methodology

1. **Data Cleaning & Preprocessing**:
   - Handled missing values.
   - Encoded categorical variables.
   - Normalized numerical features.
   
2. **Exploratory Data Analysis (EDA)**:
   - Visualized feature distributions.
   - Identified correlations between variables.
   - Analyzed class distribution.
   
3. **Model Training & Evaluation**:
   - Implemented multiple models including:
     - **Random Forest Classifier** with **SMOTE** for handling class imbalance.
     - **Balanced Random Forest Classifier**.
     - Experimented with **Gradient Boosting Classifier**, but it did not yield good results and was discarded.
     - Applied **class reduction for the majority class** with **Random Forest**, but it did not improve results.
   
   - The models were evaluated using accuracy, precision, recall, F1-score, and ROC-AUC.

## Results

- The **Random Forest Classifier with SMOTE** achieved an **ROC-AUC score of 0.82**.
- The **Balanced Random Forest Classifier** performed better, achieving an **ROC-AUC score of 0.88**.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/omari-amina/Predicting-Hazardous-NEOs-Nearest-Earth-Objects.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook "Predicting_Hazardous_NEOs.ipynb"
   ```

## Contributors

- **Amina Omari** - Data Analysis & Model Development



---

